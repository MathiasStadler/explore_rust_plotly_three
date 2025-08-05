# hello

## delete empty lines

- :g/^$/d

## bash file sort by  column 3

- sort -k5 -n /tmp/aa.txt
- grep settings.json /tmp/aa.txt  >/tmp/a1.txt
- sort -k5 -n /tmp/a1.txt

## find and ls with full path output

- find .  -name '.vscode'  -exec ls -ltrd {} \;
- find .  -name '.vscode'  -exec ls -ltrd {} \; | sort -k5 -n
- find .  -name '.vscode'  -exec ls -la {} \; |grep settings.json |sort -k5 -n
- find .  -name '.vscode'  -exec ls -lad {} \;

- find .  -name '.vscode'  -exec ls -lad {} \;|awk '{print $9}'

- find .  -name '.vscode'  -exec ls -lad {} \;|awk '{print $9}'|xargs ls -la {} |grep settings.json | sort -k5 -n

- find .  -name 'settings.json'  -exec ls -lad {} \;

## FINAL

- find .  -name 'settings.json'  -exec ls -lad {} \; |sort -k5 -n
