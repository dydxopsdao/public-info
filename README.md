# public-info
Public, DOS-related development information

# Signotifier message verification

To verify the signature appended to the message by Signotifier run:

```
openssl dgst -sha256 -verify dydxops-pubkey.pem \
-signature SIGNATURE.sig \
-sigopt rsa_padding_mode:pss \
MESSAGE.txt
```
