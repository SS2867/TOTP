A webpage to generate TOTP codes with given secret and configurations.

Deployed at [https://ss2867.github.io/TOTP](https://ss2867.github.io/TOTP)

- Supports TOTP digits from 4 to 10.
- Supports TOTP period adjustment.
- Supports optional TOTP seed double encryption protection (using a self-defined symmetric encryption algorithm including charwise shift and swap).
- Supports TOTP time retrace.
- Supports otpauth URI parsing.
- Only SHA1 is supported, other hash algorithm is **not** supported
- Parameter passing (by **fragment identifier** `#`) is supported. Example: [https://ss2867.github.io/TOTP#secret=ABCD2345&digits=8&period=20](https://ss2867.github.io/TOTP#secret=ABCD2345&digits=8&period=20)

In most cases, you simply need to specify the secret seed. You can directly input otpauth URI (like `otpauth://totp/test:me?secret=ABCD2345&digits=8&period=20`) to the seed column.
