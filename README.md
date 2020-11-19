# echo-string-manipulation
Manipulasi string dalam echo unix
<code>
#!/bin/bash
VAR=" 2 1 34 3 2 "
shopt -s extglob # Enable the `+(...)`
expression=${VAR#+(\ )}
expression=${expression%+(\ )}
echo ${expression//+(\ )/+}   
</code>
