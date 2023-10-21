# Collect Wordlist to make abs-path

Better wordlists for lfi-linux.

```bash
cat fulllist.txt | sort | uniq | grep -v "^??" | grep -v "^?\." | grep -v "^0x2" | grep -v "^#" | grep -v "^%" | grep -v "^.%"| grep -v "^\." | grep -v "\.\." | grep -v "^/0x" | grep -v "//" | grep -v '\\\\' | less > lfi-linux-full.txt
```