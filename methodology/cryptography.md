# Cryptography Cheatsheet

## Online Tools

Cipher Identifier

> [https://www.dcode.fr/cipher-identifier](https://www.dcode.fr/cipher-identifier)

Crypto tools

> [https://www.cryptool.org/en/cto/](https://www.cryptool.org/en/cto/)

Crypto bruteforce tools

> [https://planetcalc.com/search/?tag=1204](https://planetcalc.com/search/?tag=1204)

Subsitution bruteforce tools

> [https://planetcalc.com/8047/](https://planetcalc.com/8047/)



Exif & Metadata viewer

> [https://exifmeta.com/](https://exifmeta.com/)

Whois

> [https://who.is/](https://who.is/)

Steganography
> [https://stylesuxx.github.io/steganography/](https://stylesuxx.github.io/steganography/)

## Caesar cipher

### tr

```bash
tr [OPTION] SET1 [SET2]
```

ROT13 Encode

```bash
echo "abcd" | tr 'A-Za-z' 'N-ZA-Mn-za-m'
```

ROT13 Decode

```bash
echo "abcd" | tr 'N-ZA-Mn-za-m' 'A-Za-z' 
```

ROT47 Encode

```bash
echo "abcd" | tr '\!-~' 'P-~\!-O'
```

ROT47 Decode

```bash
echo "abcd" | tr 'P-~\!-O' '\!-~' 
```

## Base64

### base64

base64 text encode

```bash
echo -n "1234" | base64
```

base64 text decode

```bash
echo -n "1234" | base64 -d 
```

base64 file encode

```bash
base64 /bin/mkdir > mkdir-base64.txt
```

base64 file decode

```bash
base64 -d pix.base64 > pic.jpg
```
