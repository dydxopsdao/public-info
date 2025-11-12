# DOS Public Information
Public development information from dYdX Operations Services.

# Signotifier message verification

To verify the signature appended to the message by Signotifier run:

```
openssl dgst -sha256 -verify dydxops-pubkey.pem \
-signature SIGNATURE.sig \
-sigopt rsa_padding_mode:pss \
MESSAGE.txt
```
