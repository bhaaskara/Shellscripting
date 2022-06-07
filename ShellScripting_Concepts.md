# Debug a script
`bash -x <script_name.sh>`

## For loop
```sh
for (( i=0; i<= 10; i++))
{
    echo "Hello world; $i"
}
```

# Files
## Read a specific line in a file
`sed -n 2p <file>`
`sed -n 5,10p <file>` to get a range
`sed '2q;d' <file>` This gives best performance, coz `sed` exists after 5th line.

# sed (stream editor)
Delete a line using sed
https://linuxhint.com/sed-command-to-delete-a-line/#:~:text=To%20delete%20a%20line%2C%20we,will%20delete%20all%20the%20lines.
