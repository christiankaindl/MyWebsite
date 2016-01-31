/*
This file is part of my website.

Copyright (C) 2016  Christian Kaindl

This website is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This website is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this website.  If not, see <http://www.gnu.org/licenses/>.
*/


This guide will bring you through all my coding standards and my modularity system. It wants to help anybody who wants to distribute and/or learn from my creations and is part of every repository I make. On the bottom of each page there is a reference in which I will explain all resources I have used.
It will teach you the idea behind things I made as short as possible. Improvements are always welcome at https://github.com/GrisuProjects/MyWebsite
I am am sure you wanna code as fast as possible so let's start right in:

THE SYNTHAX

  Short indroduction into my synthax.

  GENERAL

  * No leading spaces
  * Use blank lines to indicate blocks of related code
  * Use spaces as indentations, not tabs

  CSS/SCSS

    * Use two spaces for indentation
    * Make spaces before {} and after :
    * Use enough lines, don't squeeze too many things in one line
      - Example

        body {
          font-size: 100%;
        }


  HTML

    * Use two spaces for indentation
    * After large related blocks of code make an empty line
    * Use enough lines, don't squeeze too many things in one line
      - Example

      <p>
        Some text.
      </p>


  JavaScript

    * Use four spaces for indentation
    * For all rules submit your file to jslint.com or look at my JS file
      - Example



  THE STRUCTURE

    Short introduction into my file rules.

    GENERAL

      * There is always a copyright notice on top of each file.


    CSS/SCSS

      * The code is divided into sections for better readability
        - There are 4 major ones

          ) General tag declarations (not section specific)
            - like body, h2, a, ...
            - NOT: .class, #id, .class h2, ...

          ) header section
          ) main section
          ) footer section

        Except the first section mentioned above all other sections are outsourced from the index.scss file for better readability.

      * More sections are mediaPortrait and mediaLandscape
        - These are divided with a line of this : /*=======[...]=======*/


    HTML

      * Divide related blocks of code (like the CSS/SCSS sections) by blank lines