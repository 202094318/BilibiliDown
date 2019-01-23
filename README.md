# INeedBiliAV - BilibiliDown
**INeedBiliAV** ΪBilibili ��Ƶ����������������Bվ��Ƶ��  
**INeedBiliAV**֧�ָ������������أ������ָ����ʽ������Ҫ�û���¼��Cookies��

[TOC]

## ���
### ʹ�����Լ��ⲿ��
* �ù���Ϊ��Java��д��
* ʹ���Դ���HttpUrlConnection��Ϊ�������ӣ�δ�õ�Okhttp/HttpClient/HtmlUnit/Jsoup���ⲿ�⣻
* ʹ��org.json�����򵥵�Json������
* ʹ��zxing���������Ӷ�ά��ͼƬ��

### ���Ĺ���ʵ��
��ҪΪ**nicelee.bilibili**���µ������ࣺ  

| Module  | Description |
| ------------- | ------------- |
| INeedAV  | ʵ���˸���av�Ż�ȡ�����У���Ƶ��Ϣ��������Ƶ�ȹ��ܡ������ظ�ʽΪflv��֧�ָ��������ȣ�֧��Cookies��  |
| INeedAVbPhone  | ʵ���˸���av�Ż�ȡ����һ������Ƶ��Ϣ��������Ƶ�ȹ��ܡ������ظ�ʽΪmp4���������޷���֤��  |
| INeedLogin  | ʵ���˲����û���Ч�ԡ���ȡ�û���Ϣ��ɨ���¼�ȹ��ܣ���¼�ɹ��󱣴���ͬ��Ŀ¼�µ�cookies.config��  |



### �������װ
���߷���Ϊ**nicelee.util**���£�

| Module            |  Description |
| ----------------- | ----------- |
| HttpCookies       |  �ṩString��HttpCookieList��ת����������һ����̬��ȫ��Cookies������ȫ�ֵ�Cookie��ȡ�����̰߳�ȫ����ע�⣩ |
| HttpHeaders       |  ���ڸ���Http�����ͷ������ |
| HttpRequestUtil   |  ����ʵ�ָ���Get/Post���͵�Http���󣬲������ع������˷�װ |
| QrCodeUtil        |  ���ڶ�ά��ͼƬ������ |


## ʹ�÷�����
### ������ģʽ
��ģʽ�Ƚϴֲڣ���������o((>��< ))o������
* ���ö�ά��ɨ���¼��ȡcookies��������qrcode.jpg����¼�󱣴浽cookies.config��
``` dos
java -cp INeedBiliAV.jar nicelee.bilibili.INeedLogin 1
```

* ����cookies����Ч�ԣ���ȡcookies.config��
``` dos
java -cp INeedBiliAV.jar nicelee.bilibili.INeedLogin 0
```

* ���ص�ǰcookie�������ص�����������
``` dos
java -cp INeedBiliAV.jar nicelee.bilibili.INeedAV "av40877923" 
```

### UIģʽ
��ģʽ��ż���ᱨhttp socket connect/read timeout�쳣��Ŀǰ��δ��������������ٴν��г��ԡ�
* ���г���java/javaw ���ɣ�
``` dos
javaw -Dfile.encoding=utf-8 -jar INeedBiliAV.jar
```
PS������ֱ��˫��jar�ļ����У���Ϊ���ܴ����������룬����Ҫ����file.encoding=utf-8��  
��JVM����������ǰ�Ѿ���ȡ�������������޸���Ч��  
һ������취���޸�ע���   


| ����  | ֵ |
| ------------- | ------------- |
| λ��  | HKEY_CLASSES_ROOT\Applications\javaw.exe\shell\open\command  |
| ԭʼֵ  |"...\bin\javaw.exe" -jar "%1"  |
| ����ֵ  | "...\bin\javaw.exe" -Dfile.encoding=utf-8 -jar "%1"  |
   

* ɨ���¼(��ѡ)   
������������Ͻǵ�¼��ť�����ֻ���ʹ����������appɨ�赯���Ķ�ά��  
![](https://raw.githubusercontent.com/nICEnnnnnnnLee/BilibiliDown/master/release/prelook/qrcode-login.png)
* ��ȡ��Ʒ��Ϣ  
������������������av�Ż���av�������ӣ�����ҷ���ť����  
![](https://raw.githubusercontent.com/nICEnnnnnnnLee/BilibiliDown/master/release/prelook/index.png)
* ����  
����Ʒ��Ϣ��������Ҫ����Ƶ�����Ƚ�������  
![](https://raw.githubusercontent.com/nICEnnnnnnnLee/BilibiliDown/master/release/prelook/avDetails.png)  
![](https://raw.githubusercontent.com/nICEnnnnnnnLee/BilibiliDown/master/release/prelook/download.png)
* ����  
�ر���Ʒ��Ϣҳ�� - ˫��Tab��ǩ������Tab��ǩΪ�л����㣩  


## ����  
GitHub: [https://github.com/nICEnnnnnnnLee/BilibiliDown](https://github.com/nICEnnnnnnnLee/BilibiliDown)  
Gitee����: [https://gitee.com/NiceLeee/BilibiliDown](https://gitee.com/NiceLeee/BilibiliDown)  
LICENSE: [Apache License v2.0](https://www.apache.org/licenses/LICENSE-2.0.html)




