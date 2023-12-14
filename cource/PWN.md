# PWN軟體安全測試
- 軟體安全測試
- 軟體安全測試系統建置
- 逆向工程技術
- 使用Pwntools進行連線測試
- Buffer overflow漏洞分析1:Buffer overflow
- Buffer overflow漏洞分析2:ret2code
- Buffer overflow漏洞分析3:ret2sc shell code
- Binary Security AND Protection
- return to libc
- ROP(Return-oriented programming)
  - ROP1_rop-emporium-split-64bit
  - ROP2_rop-emporium-callme-64-bit
- lazy binding
- Format_string
  - Format_string_Vulnerability攻擊模式1:
  - Format_string_Vulnerability攻擊模式2:寫入
    - printf 可以使⽤ %n 來寫入指定的位置
    - 可透過 %c 來指定 %n 要寫入的⼤⼩
    - 練習題目
      - Pwn/fmt-2
      - Pwn/fmt-3
      - Level 1.secret
## 軟體安全測試 
- 應用程式安全
  - C/C++ 應用程式安全
  - 手機應用程式安全: Android ios
  - 網站應用程式安全
  - 雲端應用程式安全
- [Secure coding](https://en.wikipedia.org/wiki/Secure_coding#:~:text=Secure%20coding)
  - Secure Coding Best Practices
  - [SEI CERT C Coding Standard](https://wiki.sei.cmu.edu/confluence/display/c/Introduction)
    - [SEI CERT Coding Standards](https://wiki.sei.cmu.edu/confluence/display/seccode/SEI+CERT+Coding+Standards)
    - [The SEI CERT C Coding Standard, 2016 Edition](https://resources.sei.cmu.edu/downloads/secure-coding/assets/sei-cert-c-coding-standard-2016-v01.pdf)
    - [SEI CERT C++ Coding Standard](https://resources.sei.cmu.edu/downloads/secure-coding/assets/sei-cert-cpp-coding-standard-2016-v01.pdf) 
  - [Motor Industry Software Reliability Association (MISRA)](https://en.wikipedia.org/wiki/Motor_Industry_Software_Reliability_Association)
  - [Defensive programming](https://en.wikipedia.org/wiki/Defensive_programming) vs [Offensive programming](https://en.wikipedia.org/wiki/Offensive_programming)
  - [SECURE CODING@tenlong](https://www.tenlong.com.tw/search?utf8=%E2%9C%93&keyword=SECURE+CODING)
  - [Secure Coding in C and C++, 2/e (Paperback) Robert C. Seacord](https://www.pearson.com/store/p/secure-coding-in-c-and-c-/P200000000596/9780132981972)
    - 繁體中譯本  [萬無一失的程式碼－終結 C & C ++ 軟體漏洞]
- [Security bug](https://en.wikipedia.org/wiki/Security_bug) 與Software Vulnerabilities
- Security and Program Analyst

## 軟體安全測試系統建置
- gcc程式編譯技術
  - [GCC online documentation](https://gcc.gnu.org/onlinedocs/)
  - [GCC 編譯器基本使用教學與範例 - G. T. Wang](https://blog.gtwang.org/programming/gcc-comipler-basic-tutorial-examples/)
  - [gcc command in Linux with examples](https://www.geeksforgeeks.org/gcc-command-in-linux-with-examples/)
- nc
  - [8 Netcat (nc) Command with Examples]()
  - [nc Command (Netcat) with Examples](https://phoenixnap.com/kb/nc-command#:~:text=The%20Netcat%20(%20nc%20)%20command%20is,%2C%20ncat%20%2C%20and%20others).) 
- socat 
  - Socat 官方網站[socat - Multipurpose relay](http://www.dest-unreach.org/socat/)
  - [socat 使用手册](https://payloads.online/tools/socat/)
  - [socat技術@gOOGLE]()

## 逆向工程技術
- gdb與強化工具peda
  - 使用checksec檢查程式安全 
- radare2逆向工程技術
- Ghidra逆向工程技術
  - [The Ghidra Book: The Definitive Guide](https://nostarch.com/GhidraBook)
    - [Ghidra 權威指南|楊超](https://www.tenlong.com.tw/products/9787121445514?list_name=srh) 
      - 第21章 混淆代碼分析
  - [Ghidra Software Reverse Engineering for Beginners(2021)](https://www.packtpub.com/product/ghidra-software-reverse-engineering-for-beginners/9781800207974)
    - [GITHUB](https://github.com/PacktPublishing/Ghidra-Software-Reverse-Engineering-for-Beginners) 
## 使用Pwntools進行連線測試
- Pwntools
  - [Exploit利器——Pwntools](http://brieflyx.me/2015/python-module/pwntools-intro/)
  - [pwntools 模块总结](https://leeyuxun.github.io/pwntools%E6%A8%A1%E5%9D%97%E6%80%BB%E7%BB%93.html)
  - [pwntools Documentation](https://docs.pwntools.com/en/stable/) 
    - [簡體中文版](https://pwntools-docs-zh.readthedocs.io/zh_CN/dev/) 
  - [Pwntools Tutorials](https://github.com/Gallopsled/pwntools-tutorial#readme)
- 使用Pwntools解PPC(Professional Program Code)問題
  - 參考 [3.使用Python求解PPC(Professional Program Code)問題](https://github.com/MyFirstSecurity2020/SF2023A3) 

## Buffer overflow漏洞分析1:Buffer overflow [教學影片](https://youtu.be/PbNzjk0yU2c)
- [Buffer overflow-1](./BF1.md)
- DANGER FUNCTION IN C /C++
- 1-1.pass [上課示範解題]
  - gcc -fno-stack-protector -z execstack pass.c -o pass -no-pie
  - socat TCP-LISTEN:20000,fork EXEC:'./pass'
- 2-1.張元_Pwn-1

## Buffer overflow漏洞分析2:ret2code [教學影片](https://youtu.be/JLlhEO4YRo4)
- 1-2.gohome 
- 1-3.registration
- 1-10.Angelboy_Pwn-1
- 1-9.張元_Pwn-8
## Buffer overflow漏洞分析3:ret2sc shell code
- level-1.Angelboy_Pwn-2 
- level-2.張元_Pwn-9
