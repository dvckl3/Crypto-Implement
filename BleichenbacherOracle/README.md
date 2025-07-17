# Tài liệu
[1] [Chosen Ciphertext Attacks Against Protocols Based on the RSA Encryption Standard PKCS #1](https://archiv.infsec.ethz.ch/education/fs08/secsem/bleichenbacher98.pdf)


# Thuật toán 
## PKCS#1v1.5

Thay vì gửi nguyên msg ban đầu của ta thì ta sẽ pad thêm vào nó để làm cho quá trình mã hóa bằng RSA trở nên non-deterministic. 

Cụ thể: Gọi $\displaystyle k$ là byte-length của modulo $\displaystyle N$. Padding sẽ diễn ra như sau:

- 2 bytes đầu tiên sẽ là `0x00` và `0x02`.
- Sau đó sẽ có ít nhất 8 random bytes theo sau và tất cả các bytes này khác `0x00`.
- Một byte `0x00` duy nhất`
- Và message cần pad.

<img width="783" height="125" alt="image" src="https://github.com/user-attachments/assets/6e90fcc6-2fbd-463e-9266-0735ee74d887" />

