
Loot
====

I wrote `loot` as a replacement for the `fortune` command, to avoid needing
to run manual commands with root access to update my quotation files.
This relies on some GNU `coreutils` such as `shuf`. You may find it useful
for printing other random text besides quotations, just bear in mind
it has not been heavily tested.

Usage
-----

usage: loot [options] [target file or directory]

Print random quotes or text from within the target file/directory specified.
By default entries are delimited by a line containing only the '%' character.
The last entry must be terminated by the delimiter as well.

### Example:

quotes.txt

```
"One original thought is worth a thousand mindless quotings."
 -- Diogenes
%
"You'll find your fortune fallin' all over town
 Be sure that your umbrella is up-up-up-up-up-upside down"
 -- Louis Prima
%
```


### Options

```
--help,-h                Show this help text
--number,-n              Number of random entries to print (Default 1)
--input-delimiter,-i     Delimiter separating entries within the text file(s) (Default '%')
--output-delimiter,-o    Delimiter separating printed entries (Default '' for a blank line)
--glob,-g                Glob pattern for matching files within a target directory (All files by default)
--width,-w               Number of columns until output is forced to line-wrap (Default 80)
```


