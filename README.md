

gcc -g -O0 -no-pie -fstack-protector -fcf-protection=full -Wl,-z,ibt -Wl,-z,shstk <file> 

clang -g -O1 -no-pie -flto -fvisibility=hidden -fsanitize=cfi -fstack-protector-strong <file>
