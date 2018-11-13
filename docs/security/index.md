# Security

## SSH

### How to check if RSA/DSA key pair matches

The following command displays the matching public key for a given private one:

```
ssh-keygen -y -e -f <private key>
```

To check if the public key matches the private one, use:

```
diff <( ssh-keygen -y -e -f id_rsa ) <( ssh-keygen -y -e -f id_rsa.pub )
```
