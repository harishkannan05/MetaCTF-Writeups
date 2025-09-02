# Challenge Statement
<img width="1112" height="180" alt="image" src="https://github.com/user-attachments/assets/0ae772c3-2fe8-4ecc-a8ca-39c92eb742ac" />

**Attachment:** https://github.com/harishkannan05/MetaCTF-Writeups/blob/b2af664ac06cd0a0570adf58f7a06c252c1fd9e2/August/Attachments/babysomething.pcap

# Solution
We are given a `.pcap` capture file and asked to recover the flag.  
We can just open it using **Wireshark** and **Follow TCP Stream.**  
<img width="1273" height="547" alt="image" src="https://github.com/user-attachments/assets/04bd385a-2a9c-4df3-aee1-3c707bf0aba5" />


## Alternative
Since the traffic is unencrypted, we can just use the **strings** command to get the flag.  
```strings babysomething.pcap | grep 'MetaCTF{[^}]*}'```  
<img width="1015" height="87" alt="image" src="https://github.com/user-attachments/assets/84040962-9800-45c9-b6c3-2a2227fc8aec" />
