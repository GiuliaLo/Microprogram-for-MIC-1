# SUMDIF-instruction-Micro-Assembly-Language
Assignment for my Computer Architecture class at Politecnico di Milano.

We used the [MIC-1 architecture](http://www.ontko.com/mic1/) from the book *Structured Computer Organization* by Andrew Tanenbaum.
The assignment was to write an instruction in [Micro Assembly Language](http://www.ontko.com/mic1/mal.html) that performs the sum of the numbers that are different among the top 3 of the stack, and writes the result in place of those top 3 numbers (i.e. (44,3,1,2,2)->(44,3,3)).

Extra credit was awarded for writing a test program in [IJVM](http://www.ontko.com/mic1/jas.html) (Integer-JVM, subset of the JVM assembly language)

Instructions to download the mic1 microarchitecture simulator and run the programs at http://www.ontko.com/mic1/user_guide.html


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
