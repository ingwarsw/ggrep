Glassfish Application server log helper
=======================================

# Basics

This litlle script helps searching for information in application log files.
Its basicly written for Glassfish but can by any logs.


# Usage


```
Usage for script:
    ggrep [opts] <search string>

    --revert        -v          revert match (show only not matching records)
    --icase         -i          ignore case
    --only-matching -o          print only the matched (non-empty) parts of a matching line
    --unbzip        -b          unbzip log (for ggrep only)
    --noasci        -n          no ansi colors
    --quiet         -q          do not print any extra informations
    --count         -c          print count of matching elements instead of printing them
    --date          -t date     date of file to search in format yyy-mm-dd
    --domain        -d name     domain name to search (without domain prefix)
    --ignore        -I regexp   records containing regexp will be ignored
    --max           -m int      max record length
    --session       -s int      glassfish session id

    <search string>         regexp string to search for

```

# Instalation
```
# Go into place where you want to heve them as binaries (/usr/local/bin or $HOME/bin)
cd ~/bin

# download script
wget https://raw.githubusercontent.com/ingwarsw/ggrep/master/ggrep

# add executable bit
chmod a+x ggrep

# make link so all "flawors" of command will work
ln -s ggrep gtail
ln -s ggrep gless
ln -s ggrep gstats

```
