# Cryptography Cheatsheet

## Online Tools

**Cipher Identifier**

> [https://www.dcode.fr/cipher-identifier](https://www.dcode.fr/cipher-identifier)

**Crypto tools**

> [https://www.cryptool.org/en/cto/](https://www.cryptool.org/en/cto/)

**Exif & Metadata viewer**

> [https://exifmeta.com/](https://exifmeta.com/)

**Whois**

> [https://who.is/](https://who.is/)

**Steganography**
> [https://stylesuxx.github.io/steganography/](https://stylesuxx.github.io/steganography/)


## Caesar cipher

**tr**
```
tr [OPTION] SET1 [SET2]
```

ROT13 Encode
```
echo "abcd" | tr 'A-Za-z' 'N-ZA-Mn-za-m'
```

ROT13 Decode
```
echo "abcd" | tr 'N-ZA-Mn-za-m' 'A-Za-z' 
```

ROT47 Encode
```
echo "abcd" | tr '\!-~' 'P-~\!-O'
```

ROT47 Decode
```
echo "abcd" | tr 'P-~\!-O' '\!-~' 
```

## Caesar cipher

**base64**

base64 text encode
```
echo -n "1234" | base64
```

base64 text decode
```
echo -n "1234" | base64 -d 
```

base64 file encode
```
base64 /bin/mkdir > mkdir-base64.txt
```

base64 file decode
```
base64 -d pix.base64 > pic.jpg
```


