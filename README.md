# INeedBiliAV - BilibiliDown
**INeedBiliAV** ΪBilibili ��Ƶ����������������Bվ��Ƶ��  
**INeedBiliAV** ֧�ָ������������أ������ָ����ʽ������Ҫ�û���¼��Cookies��   
**INeedBiliAV** �ṩUI�������棬�ڰ�װ��JDK�����£�ֻ��˫�����г��򼴿ɡ�   
**INeedBiliAV** ��װ��һЩ���ڵ�¼/���ص�API�����赼�����������(org.json��```.java```��ʽ����)��API��ֱ����ȥʹ�á�   

[TOC]

## ���
### ʹ�����Լ��ⲿ��
* �ù���Ϊ��Java��д��
* ʹ���Դ���HttpUrlConnection��Ϊ�������ӣ�δ�õ�Okhttp/HttpClient/HtmlUnit/Jsoup���ⲿ�⣻
* ʹ��org.json�����򵥵�Json������
* ʹ��zxing���������Ӷ�ά��ͼƬ��
* ʹ��ffmpeg����ת��(flv��ʽδʹ��ffmpeg����mp4��ʽ��Ҫ�õ�����������������һ�µ�)

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
#### ����
���Բ��ùܣ�ʹ��Ĭ�����ü��� 
```
# 0: MP4 1:FLV
bilibili.format = 0

#�����ļ�����·���� ���������·����Ҳ�����Ǿ���·��
bilibili.savePath = download/
#bilibili.savePath = D:\Workspace\bilibili\
```

* ֱ��˫��```run-UI.bat``` ��```run-UI-debug.bat```  
* �ű�ԭ��java/javaw ���ɣ�
``` dos
javaw -Dfile.encoding=utf-8 -jar INeedBiliAV.jar
```
PS������ֱ��˫��jar�ļ����У���Ϊ���ܴ����������룬����Ҫ����file.encoding=utf-8��  
��JVM����������ǰ�Ѿ���ȡ�������������޸���Ч��  
* �����ֱ��˫��jar���У�һ������취���޸�ע���   


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
������Ʒ��Ϣ - ����ƷTabҳ������Ҫ���Ƶ�Ŀ������   
�޸�������Ƶ��ʽ - ��```app.config```������```bilibili.format```ѡ��    
���������� - �ҵ�����Ŀ¼�е�```rename.bat```��˫����   

## UPDATE  
* v2.2 
    * ������HTML5����Դ�����ط�ʽ,֧��FLV/MP4���ָ�ʽ 
    * (UI)��������Ż�Ϊ�����������ͬ����Ƶ��������(���ֱ�������)
    * (UI)������Ŀ¼��������������```rename.bat```��Ĭ�ϸ�ʽΪ```avId-qn-p.(flv|mp4)```������ʹ�ø������������ı���Ϊ```��Ƶ����-qn-p.(flv|mp4)```
    * (UI)���������ظ�ʽ����(flv ȡFlash����Դ, mp4 ȡHTML5����Դ)
    * (UI)����������·������
* v2.1 
    * �����˶ϵ����������ع���, ��������ϴ�δ������ɵ�```.part```�ļ�,�����ϴεĻ����ϼ�����������;
    * (UI)������ͣ/�����쳣��������ع���, ��ϵ�����������ƥ��;
    * (UI)����Ʒ����ҳ�������ֿ��Ը�����Ϣ;
    * ���ǹ���һ����Ƶ�ֳɺܶ�Fragment���߳����ص�, �������ƺ��Է��������Ǻܺ�, ���ҿ���Ԥ�����кܶ�bug(�������Ҫ??), �ټ��ϱ����Ѿ��ܹ�ͬʱ���ض����ͬ��av, �ʶ���û�м���;
    * ���ǹ�ʹ��HTML5�Ĳ���Դ, ```.m3u8```��ֱ�Ӻϲ�����, ��������```.m4s```,ľ�о����??. ��ν�����ͷ��**SegmentBase**, ��κϲ�����Ƶ, Ŀǰ����Ǳˮѧϰ��... �ؼ���û�ж�ý�崦����,����ffmpeg
    
* v2.0 
    * �޸�һ��bug,��bug���²�����Чcookies��֤�׳��쳣,�����Ƿ���false;
    * (UI)�޸�һ��bug,��bugʹ��ɨ���¼��δ�ܼ�ʱ�����û�ͷ�����Ϣ;
    * (UI)���Ӷ�ά��ɨ��ʱ����,һ���Ӻ��Զ�����;
    * (UI)���ӵ�¼������̬Ч��,���������������;
    * ����flv������ ```avId-p.flv``` ��Ϊ```avId-qn-p.flv```,���������ȱ�ʶ
    * (UI)�Ż���.bat�ű�,```run-UI.bat```���к�������˳�,```run-UI-debug.bat```���к����������,���ҿɲ鿴�����Ϣ
## ����  
* **���ص�ַ**: [https://github.com/nICEnnnnnnnLee/BilibiliDown/releases](https://github.com/nICEnnnnnnnLee/BilibiliDown/releases)
* **GitHub**: [https://github.com/nICEnnnnnnnLee/BilibiliDown](https://github.com/nICEnnnnnnnLee/BilibiliDown)  
* **Gitee����**: [https://gitee.com/NiceLeee/BilibiliDown](https://gitee.com/NiceLeee/BilibiliDown)  
* **LICENSE**: [Apache License v2.0](https://www.apache.org/licenses/LICENSE-2.0.html)




