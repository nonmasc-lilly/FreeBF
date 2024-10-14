[//]: #
[//]: #   FreeBF, The free brainfuck compiler (README.md)
[//]: #   Copyright (C) 2024 Lilly H. St Claire
[//]: #            This program is free software: you can redistribute it and/or modify
[//]: #            it under the terms of the GNU General Public License as published by
[//]: #            the Free Software Foundation, either version 3 of the License, or (at
[//]: #            your option) any later version.
[//]: #            This program is distributed in the hope that it will be useful, but
[//]: #            WITHOUT ANY WARRANTY; without even the implied warranty of
[//]: #            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
[//]: #            General Public License for more details.
[//]: #            You should have received a copy of the GNU General Public License
[//]: #            along with this program.  If not, see <https://www.gnu.org/licenses/>.

# FreeBF : The Free BrainFuck Compiler
## Lilly H. St Claire
### October 2024

Brainfuck is a popular esolang designed by Urban M&#x00FC;ller in 1993 in order to write
the smallest possible compiler for the Amiga OS. It consists of the following instructions:

- `>` increment the memory register
- `<` decrement the memory register
- `+` increment the byte at the address stored in the memory register
- `-` decrement the byte at the address stored in the memory register
- `.` output the byte at the address stored in the memory register as an ASCII character
- `,` input an ASCII character from the terminal and store it at the address pointed to by
 the memory register
- `[` if the current byte is zero, jump to the instruction following the matching `]`
- `]` if the current byte is non-zero, jump to the instruction following the matching `[`

This compiler has the following beginning goal targets:

- Linux x86\_64                     [ ]
- Windows x86\_64                   [ ]
- 8086 Legacy BIOS                  [ ]
- UEFI Boot Service Enabled x86\_64 [ ]

