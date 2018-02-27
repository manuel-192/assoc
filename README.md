# assoc
Command line program for associating filename extensions to programs.
MS Windows provides a similar command line application that associates extensions to file types instead of programs.
Associating directly to programs is simpler and more straightforward.

<H2>Example:</H2>

1) Create your preferred associations:
<pre>
$ assoc -e "qtcreator -client" cpp c h
$ assoc -e libreoffice doc xls odt ods
$ assoc -v mpv mp4
</pre>

2) Use the associations:
<pre>
$ assoc -re myprogram.cpp sometest.h finance.xls
$ assoc -rv myvideo.mp4
</pre>

The example above associated file endings <i>cpp</i>, <i>c</i> and <i>h</i> to command <b>"qtcreator -client"</b> (note the usage of quotes!), and <i>mp4</i> files to command <b>mpv</b>.<br>
Now <i><b>e</b>diting</i> files can be done with command <b>assoc -re</b> and <i><b>v</b>iewing</i> a video with command <b>assoc -rv</b>.
Naturally aliases can be used to make this simpler, and they are provided with the implementation as follows:
<pre>
alias o='assoc -r'
alias e='assoc -re'
alias v='assoc -rv'
</pre>

so the second phase of the example above simplifies to:
<pre>
e myprogram.cpp sometest.h finance.xls
v myvideo.mp4
</pre>

Examples of some preferred associations:
<pre>
assoc -v firefox htm html
assoc -e bluefish htm html
assoc -e libreoffice odt ods doc docx xls xlsx
assoc -v evince pdf
assoc -e emacs bash sh
assoc -e qtcreator pro
assoc -e "qtcreator -client" c cpp h
</pre>

# Changes
0.1.43: 2018-Feb-24
- fixed extensionless file association
