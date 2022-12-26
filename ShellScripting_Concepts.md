# Debug a script
`bash -x <script_name.sh>`

# Print output
```
printf "Enter your name:\n"
printf "$name $surname"
printf "$arr[0]"  #Print arrays
```
# Loops
## For loop
```sh
for (( i=0; i<= 10; i++))
{
    echo "Hello world; $i"
}
```
# Conditional statements
## If
https://www.geeksforgeeks.org/conditional-statements-shell-script/

# Files
## Read a specific line in a file
`sed -n 2p <file>`
`sed -n 5,10p <file>` to get a range
`sed '2q;d' <file>` This gives best performance, coz `sed` exists after 5th line.

## Read file line by line
Files can be read in difeerent ways, like using for,while,AWK or sed
```sh
file=$(cat proj_sa_details.txt)
for line in $file
do
	#echo "$line\n"
done
```
```sh
file="proj_sa_details.txt"
while read -r line; do 
	echo -e "$line"; 
done < "$file"
```
# sed (stream editor)
Delete a line using sed
https://linuxhint.com/sed-command-to-delete-a-line/#:~:text=To%20delete%20a%20line%2C%20we,will%20delete%20all%20the%20lines.

# Cut
*Cut a string and assign to a variable*
```
arr2= cut -d ':' -f 1 <<< $val
```
# Remove duplicates in a file
`sort file.txt |uniq`
