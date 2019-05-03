# SUMDIF-instruction-Micro-Assembly-Language
Assignment for my Computer Architecture class at Politecnico di Milano.

We used the [MIC-1 architecture](http://www.ontko.com/mic1/) from the book *Structured Computer Organization* by Andrew Tanenbaum.
The assignment was to write an instruction in [Micro Assembly Language](http://www.ontko.com/mic1/mal.html) that performs the sum of the numbers that are different among the top 3 of the stack, and writes the result in place of those top 3 numbers (i.e. (44,3,1,2,2)->(44,3,3)). (See text of the assignment in Italian in Seconda prova 2016-2017.txt)
The code for the instruction is in the .mal file, lines 55-76.

Extra credit was awarded for writing a test program in [IJVM](http://www.ontko.com/mic1/jas.html) (Integer-JVM, subset of the JVM assembly language). This can be found in the .jas file.

Instructions to download the mic1 microarchitecture simulator and run the programs at http://www.ontko.com/mic1/user_guide.html

MIC-1 Architecture:

<img src="https://github.com/GiuliaLo/SUMDIF-instruction-Micro-Assembly-Language/blob/master/MIC-1%20Architecture.png" width="50%" height="50%"></img>

## Reflections
This assignment was particularly challenging because it forced me to understand in depth the data path, how the registers work and the specific function of each one, and the timing of the data path cycle, especially for the write and read instructions.
To understand how to write the code, I started from the microinstructions that were already coded in the mic1ijvm.mal file downloaded with the mic1 simulator. I retraced step by step what each register held at any given moment and what the stack looked like after every step. Then I started experimenting with the instructions I though I needed to use, like iadd and if_icmpeq, tweaking them until I thought I had the right structure for my instruction. From there it still took me a while to fix the bugs and reach the final solution.
The TEST program was way easier to write because the IJVM language is a higher level language and because I had already completed a project for a previous assignment using that language, so I was already pretty comfortable with it. To challenge myself I learned the syntax for writing methods into the program, which I hadn't done in that previous assignment.

The computer science program goals I reached with this assignment are:
- To attain a system-level understanding of the computer


## Copyright notice for mic1
Copyright (C) 1999, Prentice-Hall, Inc.
This program is free software; you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 2 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program; if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307 USA

The file COPYING.TXT, included in this distribution, should contain a verbatim copy of the GNU General Public License.

### Legal Notices

This mic1 software is distributed under the GNU General Public License, a copy of which is included with this distribution in the file COPYING.TXT.

The Mic1 microassembler included here uses CUP, a parser generator program, produced by a third party and distributed under the following license:

CUP PARSER GENERATOR COPYRIGHT NOTICE, LICENSE AND DISCLAIMER.

Copyright 1996 by Scott Hudson, Frank Flannery, C. Scott Ananian

Permission to use, copy, modify, and distribute this software and its documentation for any purpose and without fee is hereby granted, provided that the above copyright notice appear in all copies and that both the copyright notice and this permission notice and warranty disclaimer appear in supporting documentation, and that the names of the authors or their employers not be used in advertising or publicity pertaining to distribution of the software without specific, written prior permission.

The authors and their employers disclaim all warranties with regard to this software, including all implied warranties of merchantability and fitness. In no event shall the authors or their employers be liable for any special, indirect or consequential damages or any damages whatsoever resulting from loss of use, data or profits, whether in an action of contract, negligence or other tortious action, arising out of or in connection with the use or performance of this software.

If you intend to modify or recompile the microassembler program, you will need to download the CUP LALR Parser Generator for Java(TM). For more information about CUP, visit:

   http://www.cs.princeton.edu/~appel/modern/java/CUP/
Java is a trademark of Sun Microsystems, Inc.
