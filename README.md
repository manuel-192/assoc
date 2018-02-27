# assoc
Command line program for associating programs with filename extensions.

<H2>Example:</H2>

1) Create associations like:
- assoc -e "qtcreator -client" cpp c h
- assoc -v mpv mp4

2) Use the associations:
- assoc -re myprogram.cpp sometest.h
- assoc -rv myvideo.mp4

The example above associated file endings cpp, c and h to command "qtcreator -client", and .mp4 files to command "mpv".
Now editing files can be done with command 'assoc -re' and viewing a video with command 'assoc -rv'.
Naturally aliases can be used to make this simpler, and they are provided with the implementation as follows:
alias o='assoc -r'
alias e='assoc -re'
alias v='assoc -rv'

so the second phase of the example above simplifies to:
e myprogram.cpp sometest.h
v myvideo.mp4

# Changes
0.1.43: 2018-Feb-24
- fixed extensionless file association
