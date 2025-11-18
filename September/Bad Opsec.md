# Challenge Statement
<img width="1116" height="198" alt="image" src="https://github.com/user-attachments/assets/f34bd7bd-4885-46ce-8754-e63ce525051a" />

# Solution
First, we extract the zip file with the command: 
```
7z x flagstealer.zip -pinfected -y
```

Using `strings` and `grep`, I was able to get the flag easily. 
```
strings flagstealer | grep MetaCTF{[^}]*}
```

<img width="1001" height="151" alt="image" src="https://github.com/user-attachments/assets/6c5d8912-e23f-474f-bc59-f3a3b1f694be" />
