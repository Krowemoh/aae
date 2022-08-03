# Alternative Alternative Editor

This is a simple line editor to edit multivalue records in D3. The key function
is the EV command which explodes out multivalue sets.

## Installation

Simply download the AAE file and compile and catalog it in D3.

## Help

```
^           Toggle Up-Arrow mode to print ASCII code of unprintable characters
##			Go to line

P			Display 1 page
T 			Go to top
B 			Go to bottom

EV 			Explode value
EX			Exit multivalue set
FI			Save multivalue set

LOAD 			Load in lines from another file

I 			Insert mode
A any			Append any to current line
A## any		Append any to X number of lines
DE 			Delete the current line
DE##  		Delete X number of lines

R any			Replace current line with any
R//abc		Append abc to the front of the current line
R/123/abc/# 	Replace 123 with abc, X occurances on the current line
R/123/abc/G 	Replace 123 with abc, all occurances on the current line

L any 		Search for any, go to first occurance
L###			Search X number of lines, list all occurances

<			Set block start
>			Set block end
COPY			Copy block and insert at the current line
DROP			Drop the current block

COPY X Y 		Copy lines X to Y and insert at the current line
DROP X Y		Drop lines X to Y

H 			List history
UNDO 			Undo last change - Move back in the history
REDO			Redo change - Move forward in the history

EX/Q 			Exit the editor
FI 			Save the record
FD 			Delete the record
SAVE name 		Save the record in the current file as name
SAVE file name	Save the record in the specified file as name
```
