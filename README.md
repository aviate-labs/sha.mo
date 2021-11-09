**MOVED/DEPRECATED**: use the [crypto](https://github.com/aviate-labs/crypto.mo) package instead!

# SHA

Provides the SHA256 hash algorithm as defined in FIPS 180-4.

## Usage

```motoko
SHA256.sum256(Blob.toArray(Text.encodeUtf8("hello world\n"))
// "A948904F2F0F479B8F8197694B30184B0D2ED1C1CD2A1EC0FB85D299A192A447"

let h = SHA256.Hash(false);
h.write(Blob.toArray(Text.encodeUtf8("hello world\n")));
h.sum([]);
// "A948904F2F0F479B8F8197694B30184B0D2ED1C1CD2A1EC0FB85D299A192A447"
```
