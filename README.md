# echo-string-manipulation
Manipulasi string dalam echo unix
<pre>
#!/bin/bash
VAR=" 2 1 34 3 2 "
shopt -s extglob # Enable the `+(...)`
expression=${VAR#+(\ )}
expression=${expression%+(\ )}
echo ${expression//+(\ )/+}
</pre> 
# Hasil
<pre>
2+1+34+3+2
</pre>
