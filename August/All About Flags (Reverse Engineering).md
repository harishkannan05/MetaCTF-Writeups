# Challenge Statement
<img width="1116" height="242" alt="image" src="https://github.com/user-attachments/assets/e561dee8-fb75-4477-8f18-636ed4972098" />

**Attachment:** [Windows](https://github.com/harishkannan05/MetaCTF-Writeups/blob/9df722aaa467728c56a109236a03c5a7adc66e76/August/Attachments/all-about-flags.exe) | [Linux](https://github.com/harishkannan05/MetaCTF-Writeups/blob/9df722aaa467728c56a109236a03c5a7adc66e76/August/Attachments/all-about-flags)

# Solution
We are given an executable file and asked to find the flag.  
We can find the `file type` first.  

<img width="1261" height="107" alt="image" src="https://github.com/user-attachments/assets/0c3ffa88-3575-4fce-912c-ccbae8749d51" />

Make it executable by given it the right permissions.
```chmod +x all-about-flag```

Running the file, tell use to use the `--help` flag, which then tells us to run `--flag` to get the flag.  

<img width="488" height="86" alt="image" src="https://github.com/user-attachments/assets/075bad0d-d980-43e2-9537-113bd3ef8650" />

## Alternative
We can just use the **strings** and **grep** commands to get the flag.  
```strings all-about-flags | grep 'MetaCTF{[^}]*}'```  

<img width="1267" height="130" alt="image" src="https://github.com/user-attachments/assets/a70c425f-cb27-463f-a46e-1105de956153" />
