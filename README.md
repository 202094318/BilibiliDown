# INeedBiliAV - BilibiliDown
**INeedBiliAV** ΪBilibili ��Ƶ����������������Bվ��Ƶ��  
**INeedBiliAV**֧�ָ������������أ������ָ����ʽ������Ҫ�û���¼��Cookies��
**INeedBiliAV**�ṩUI�������棬�ڰ�װ��JDK�����£�ֻ��˫�����г��򼴿ɡ�
**INeedBiliAV**��װ��һЩ���ڵ�¼/���ص�API��û�е������⣬��ֱ����ȥʹ�á�

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

## UPDATE  
* v2.1 
    * �����˶ϵ����������ع���, ��������ϴ�δ������ɵ�```.part```�ļ�,�����ϴεĻ����ϼ�����������;
    * (UI)������ͣ/�����쳣��������ع���, ��ϵ�����������ƥ��;
    * (UI)����Ʒ����ҳ�������ֿ��Ը�����Ϣ;
    * ���ǹ���һ����Ƶ�ֳɺܶ�Fragment���߳����ص�, �������ƺ��Է��������Ǻܺ�, ���ҿ���Ԥ�����кܶ�bug(�������Ҫ??), �ټ��ϱ����Ѿ��ܹ�ͬʱ���ض����ͬ��av, �ʶ���û�м���;
    * ���ǹ�ʹ��HTML5�Ĳ���Դ, ```.m3u8```��ֱ�Ӻϲ�����, ��������```.m4s```,ľ�о����??. ��ν�����ͷ��**SegmentBase**, ��κϲ�����Ƶ, Ŀǰ����Ǳˮѧϰ��... �ؼ���û�ж�ý�崦����,����ffmpeg
    * ��: ������Ƶ��Ϣ, �л����֨һ��
```
{
    "duration": 83,
        "minBufferTime": 1.5,
        "video": [{
        ...
        
        "id": 80,
        "baseUrl": "http://upos-hz-mirrorkodou.acgvideo.com/upgcxcode/42/19/78601942/78601942-1-30080.m4s?e=ig8euxZM2rNcNbdlhoNvNC8BqJIzNbfqXBvEqxTEto8BTrNvN0GvT90W5JZMkX_YN0MvXg8gNEVEuxTEto8i8o859r1qXg8xNEVE5XREto8GuFGv2U7SuxI72X6fTr859r1qXg8gNEVE5XREto8z5JZC2X2gkX5L5F1eTX1jkXlsTXHeux_f2o859IB_\u0026deadline=1551413836\u0026gen=playurl\u0026nbs=1\u0026oi=3728813686\u0026os=kodou\u0026platform=pc\u0026trid=28f5dc24eae8486794b7ce58e2887103\u0026uipk=5\u0026upsig=5d9bde6c9ab8aba0875b3262cd741050",
        "backupUrl": null,
        "bandwidth": 2442010,
        "mimeType": "video/mp4",
        "codecs": "avc1.640028",
        "width": 1920,
        "height": 1080,
        "frameRate": "25",
        "sar": "1:1",
        "startWithSap": 1,
        "SegmentBase": {
            "Initialization": "0-975",
            "indexRange": "976-1211"
        },
        "codecid": 7
    }],
    "audio": [{
        "id": 30280,
        "baseUrl": "http://upos-hz-mirrorkodou.acgvideo.com/upgcxcode/42/19/78601942/78601942-1-30280.m4s?e=ig8euxZM2rNcNbdlhoNvNC8BqJIzNbfqXBvEqxTEto8BTrNvN0GvT90W5JZMkX_YN0MvXg8gNEVEuxTEto8i8o859r1qXg8xNEVE5XREto8GuFGv2U7SuxI72X6fTr859r1qXg8gNEVE5XREto8z5JZC2X2gkX5L5F1eTX1jkXlsTXHeux_f2o859IB_\u0026deadline=1551413836\u0026gen=playurl\u0026nbs=1\u0026oi=3728813686\u0026os=kodou\u0026platform=pc\u0026trid=28f5dc24eae8486794b7ce58e2887103\u0026uipk=5\u0026upsig=449ec944995095c74727a44392c704ec",
        "backupUrl": null,
        "bandwidth": 124909,
        "mimeType": "audio/mp4",
        "codecs": "mp4a.40.2",
        "width": 0,
        "height": 0,
        "frameRate": "",
        "sar": "",
        "startWithSap": 0,
        "SegmentBase": {
            "Initialization": "0-919",
            "indexRange": "920-1155"
        },
        "codecid": 0
    }
```
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




