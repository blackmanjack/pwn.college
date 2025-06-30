# Deleting Characters

tr can also translate characters to nothing (i.e., delete them). This is done via a -d flag and an argument of what characters to delete:
`hacker@dojo:~$ echo PAWN | tr -d A
PWN
hacker@dojo:~$`
Pretty simple! Now you give it a try. I'll intersperse some decoy characters (specifically: ^ and %) among the flag characters. Use tr -d to remove them!

# Solution

/challenge/run | tr -d %^
