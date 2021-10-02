# The `pwd` Command

The `pwd` stands for Print Working Directory. It prints the path of the working directory, starting from the root.

Example:

```
pwd  
```  
Syntax:

```
pwd [OPTION]
```  
### Printing the Symbolic or Actual path with `pwd`:
 
We can use the `-L` (logical) option to print the symbolic path or we can also use the `-P` (physical) for the actual path.
You Can also use `--version` command to print the version of the pwd command. 

Example :

```
w@ichigo:~$  /bin/pwd -L
```
Sample Output:

```
/home/w/example
```

This will Print working directory from environment even if it contains symlinks.

Example :

```
w@ichigo:~$ /bin/pwd -P
```
Sample Output:

```
/var/www/exampleDir
```

If both `-L` and `-P` options are used, option `L` is taken into priority. If no option is specified at the prompt, pwd will avoid all symlinks, i.e., take option `-P` into account.

### The Default Consideration
if no options are given at run-time does `pwd` takes option -P into account or not, automatically.


#### Contributed by
[Vedansh Kumar](https://github.com/IcHiGo-KuRoSaKiI)
