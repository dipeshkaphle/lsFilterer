# ls tool with some filtering capabilities

A small script I made so that i can list out just the directories or files in a certain directory. 
* use `ruby lsImproved.rb --help` to get info about all the flags
* `ruby lsImproved.rb`  would be the same as doing `ls` on the present working directory
* `-a` or `-l` or `-la` flags can also be used in the same way as `ls`
* `-d 'Directory'` can be used to `ls` on the desired directory
* `-t` accepts three values <br>
    * `-t files` used for listing out all files
    *  `-t dirs` used for listing out the directories in specified path
    * `-t all` does the same thing as `ls`. Lists all
    * The default behaviour is `ls` like.
* If you dont provide the `-d` or `-t` flag the program resorts to default behaviour i.e `ls` on the present working directory

## Example

`ruby lsImproved -la -t files -d '~/Downloads'` lists all the files in Downloads directory including all the hidden ones and in listed format

## Suggestion
I would suggest using alias like such as
`alias lsf='ruby path/to/lsImproved.rb -t files` so that it would be more convenient  