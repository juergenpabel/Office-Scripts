# XTEA

This script encrypts or decrypts data with XTEA in CBC-mode using PKCS#7 padding.

The required parameters are:
- xtea_op: string
- xtea_key_hex: string
- xtea_iv_hex: string
- xtea_data_b64: string
The script returns a base64-enoded string.

The xtea_op must either be "encpryt" or "decrypt", or the script will just exit. The xtea_key_hex must contain a hex encoded 128bit key and the xtea_iv_hex a hex encoded 64bit initialization-vector. The to-be-en/decrypted data must be provided as a base64 string.

The implementation has been validated against XTEA test vectors (but was implemented in a very short time, so there oughta be some bugs).

