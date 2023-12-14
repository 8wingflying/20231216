# 環境設定1:virtualbox安裝與設定
- 標準安裝virtualbox ==> 下一步下一步就裝好了
- 使用系統管理員身分啟動cmd
- 切換到VirtualBox 目錄 ==> cd C:\Program Files\Oracle\VirtualBox
- 檢視現有NAT網路 == > VBoxManage list natnetworks
- 新增NAT網路 == > VBoxManage natnetwork add --netname PT --network "10.0.2.0/24" --enable
- 再次檢視現有NAT網路 == >VBoxManage list natnetworks

![A1.png](A1.png)

# 環境設定2:
- 確認攻擊機(Kali linux)與靶機(Metasploitable3)在同一個NAT網路
- 兩台機器都可以ping 到對方 

# 駭客攻防實戰營(1):Kali linux 攻擊與滲透測試技術


# 駭客攻防實戰營(2):如何阻擋駭客攻擊?

## Windows 指令(Windows Commands)
## netstat指令
- netstat -a
- netstat -an
- netstat -ano
## 實作練習
- 1.使用 cmd 開啟notepad
- 2.使用工作管理員|詳細資料 找出notepad 的PID
- 3.行程終止: 使用taskkill /PID XXXX /F 終止notepad
