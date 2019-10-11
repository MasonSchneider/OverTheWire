# OverTheWire

My solutions and notes for [overthewire](http://overthewire.org/wargames/)

## Safety

In order to prevent leaking answers I'll encrypt each answer file.

### Encryption

```
openssl enc -in Answers.md \
    -aes-256-cbc \
    -pass stdin > answers.enc
```

### Decryption

```
openssl enc -in answers.enc \
    -d -aes-256-cbc \
    -pass stdin > Answers.md
```

