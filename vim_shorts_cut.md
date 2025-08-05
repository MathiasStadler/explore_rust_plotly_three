# hello

## delete empty lines

- :g/^$/d

## bash file sort by  column 3

- sort -k5 -n /tmp/aa.txt
- grep settings.json /tmp/aa.txt  >/tmp/a1.txt
- sort -k5 -n /tmp/a1.txt

## find and ls with full path output

- find .  -name '.vscode'  -exec ls -ltrd {} \;
