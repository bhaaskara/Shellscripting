## single line while loop
```sh
while true; do echo $(date); sleep 5; done
```
> This runs indefinitely.

## Remove headers from a file
`tail +2 file.txt`

**Note:** will print from 2nd line to end of the file. 

## Create a dir, if its not exists
```
if [[ ! -e TEMP ]]
then 
	mkdir TEMP
fi
```
## Print a perticular line 
`sed -n '5p' input.txt`

## command status
```
status=$?
echo $status
if [ $status = 0 ]; then
   echo "Snap shot restoration completed"
fi
```