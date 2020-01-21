# Run bash scripts


```r
# should exist
Sys.which("bash")
```

```
##        bash 
## "/bin/bash"
```

```r
Sys.which("sh")
```

```
##        sh 
## "/bin/sh"
```

Does `bash` work?


```bash
echo hello world
echo 'a b c' | sed 's/ /\|/g'
# number of lines
awk 'END{print NR;}' 027-engine-bash.Rmd
```

```
## hello world
## a|b|c
## 23
```

How about `sh`?


```sh
# run wc on all engine examples
ls | grep engine | head -n8 | xargs wc
```

```
##  124  229 1635 023-engine-python.md
##   73  178 1417 023-engine-python.Rmd
##   16   38  161 024-engine-awk.md
##   11   41  252 024-engine-awk.Rmd
##   12   21  127 025-engine-ruby.md
##    7   17  109 025-engine-ruby.Rmd
##   13   37  234 026-engine-haskell.md
##    8   37  267 026-engine-haskell.Rmd
##  264  598 4202 total
```
