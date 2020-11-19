# echo-string-manipulation
Manipulasi string dalam echo unix
<code>
#!/bin/bash
VAR=" 2 1 34 3 2 "
shopt -s extglob # Enable the `+(...)`
expression=${VAR#+(\ )} # Remove leading spaces.
expression=${expression%+(\ )} # Remove trailing spaces.
echo ${expression//+(\ )/+}   # Replace strings of spaces by pluses
</code>
