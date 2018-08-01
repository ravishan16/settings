## Generate SSH Key

### Go to terminal

```bash
ssh-keygen -t rsa -b 4096 -C "email"
```

### Go to terminal

```bash
ssh-keygen -t rsa -b 4096 -C "email"


Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/rsivasubramaniam/.ssh/id_rsa):
Created directory '//.ssh'.
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /...
```

### Add SSH key to agent

```bash
eval $(ssh-agent -s)
ssh-add ~/.ssh/id_rsa
```

### Copy SSH public key
```bash
cat ~/.ssh/id_rsa.pub
```
