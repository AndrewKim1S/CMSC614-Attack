
### Compile
$ gcc -g -O0 -no-pie -fstack-protector -fcf-protection=full -Wl,-z,ibt -Wl,-z,shstk <file> 
$ clang -g -O1 -no-pie -flto -fvisibility=hidden -fsanitize=cfi -fstack-protector-strong <file>

### Setup
$ chmod +x <binary>
$ sudo chown root <binary>
$ sudo chmod 4755 <binary>

### Execute Instructions
$ ls
$ ls -l target
$ readelf -n target | grep -E "IBT|SHSTK"
$ python3 solve.py
  whoami

