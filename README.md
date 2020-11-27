# LED Block Cipher
## Cryptography Term Paper

### Building binaries
```bash
make main
make faulty
```

### Usage
```bash
./led-64 -p "01234567 89abcdef" -k "01234567 89abcdef" 
# output : fdd6fb98 45f81456

./led-faulty-64 -p "01234567 89abcdef" -k "01234567 89abcdef" 
# output : 51b8ab31 169ac161 

# Make sure you use python3.7
# Format : python attack.py <no_fault_cipher> <faulty_cipher> <your_key>
python attack.py fdd6fb9845f81456 51b8ab31169ac161 0123456789abcdef
```

### Team members :
Aastha Asthana, Aniket Raj, Kumar Shivendu