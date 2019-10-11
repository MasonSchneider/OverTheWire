# OverTheWire

My solutions and notes for [overthewire](overthewire.org)

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

