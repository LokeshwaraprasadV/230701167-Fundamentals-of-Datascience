```python
from cryptography.fernet import Fernet
key=Fernet.generate_key()
f=Fernet(key)
token=f.encrypt(b"Rajalakshmi Engineering College")
token
b'...'
f.decrypt(token)
b'Rajalakshmi Engineering College'
key=Fernet.generate_key()
cipher_suite=Fernet(key)
plain_text=b"Rajalakshmi Engineeing College."
cipher_text=cipher_suite.encrypt(plain_text)
decrypted_text=cipher_suite.decrypt(cipher_text)
print("Original dat:",plain_text)
print("Encrypted Data:",cipher_text)
print("Decrypted Data:",decrypted_text)
```

    Original dat: b'Rajalakshmi Engineeing College.'
    Encrypted Data: b'gAAAAABmwrWXxeMm58oFF-_cmOWbjFcOiInD2d1zxWi5PSA7OHWcQcJEMdyJnvsQJQpH1xGpbYSKxqp2XPskE8zvGYwOLqMSeSQWHUtmMwjPlwEg7Ch3DEI='
    Decrypted Data: b'Rajalakshmi Engineeing College.'
    


```python

```
