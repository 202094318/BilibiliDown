# INeedBiliAV - BilibiliDown
![����java](https://img.shields.io/badge/Require-java-green.svg)
![���԰汾64λWin10ϵͳ, jre 1.8.0_101](https://img.shields.io/badge/TestPass-Win10%20x64__java__1.8.0__101-green.svg)
![֧��ϵͳ Win/Linux/Mac](https://img.shields.io/badge/Platform-%20win%20|%20linux%20|%20mac-lightgrey.svg)
![��ԴЭ��Apache2.0](https://img.shields.io/badge/license-apache-2.0.svg)

**INeedBiliAV** ΪBilibili ��Ƶ����������������Bվ��Ƶ��  
**���¶�ͼ����**
===============================
## ����  
+ ֧��UI����(����Ϊ��ɵ��ʽ����)  
+ ֧��ɨ���¼(���Ҫ�¸���, �����Լ���cookies)  
+ ֧�ָ������ӽ���(ֱ����avXXX/epXXX/ssXXX/epXXX���Լ�������ҳ����)
+ ֧�ֶ�p����!(���˿����ֱ��˵���Ʒ, ��˵�е�ֻ֧�ֵ�p?)  
+ ֧���ղؼ�����!!  
+ ֧��UP����Ƶ����!!!  
+ ֧�ֳ���Ƶ(�����Ӱ)����!!!!  
+ ֧�ֶϵ���������!!!!!(���쳣ԭ���˳���, ֻҪ����Ŀ¼����, ֱ�����ϴλ����ϼ�������)
   
## ʹ�÷���
* ��װ(��ѡ)  
��ʵ����һ����ɫ�������װֻ�Ǵ�����һ����ݷ�ʽ������
![](https://raw.githubusercontent.com/nICEnnnnnnnLee/BilibiliDown/master/release/prelook/install.gif)  
* ɨ���¼(��ѡ)   
������������Ͻǵ�¼��ť�����ֻ���ʹ����������appɨ�赯���Ķ�ά��  
![](https://raw.githubusercontent.com/nICEnnnnnnnLee/BilibiliDown/master/release/prelook/login.gif)
![](https://raw.githubusercontent.com/nICEnnnnnnnLee/BilibiliDown/master/release/prelook/qrcode-login.png)
* ��ȡ��Ʒ��Ϣ  
������������������av�Ż���av�������ӣ�����ҷ���ť����  
![](https://raw.githubusercontent.com/nICEnnnnnnnLee/BilibiliDown/master/release/prelook/index.png)
* ����  
����Ʒ��Ϣ��������Ҫ����Ƶ�����Ƚ�������  
![](https://raw.githubusercontent.com/nICEnnnnnnnLee/BilibiliDown/master/release/prelook/avDetails.png)  
![](https://raw.githubusercontent.com/nICEnnnnnnnLee/BilibiliDown/master/release/prelook/download.png)
Ԥ��
![](https://raw.githubusercontent.com/nICEnnnnnnnLee/BilibiliDown/master/release/prelook/download.gif)
* ����  
�ر���Ʒ��Ϣҳ�� - ˫��Tab��ǩ������Tab��ǩΪ�л����㣩  
������Ʒ��Ϣ - ����ƷTabҳ������Ҫ���Ƶ�Ŀ������   
�޸�������Ƶ��ʽ - ��```app.config```������```bilibili.format```ѡ��    
���������� - �ҵ�����Ŀ¼�е�```rename.bat```��˫����   
ж�� - �ҵ�����Ŀ¼�е�```unistall.bat```��˫����(����ֻ��ɾ�����ļ���)   


## ����
��```config/app.config```�У����Բ��ùܣ�ʹ��Ĭ�����ü��� 
```
# 0: MP4 1:FLV
bilibili.format = 0

#�����ļ�����·���� ���������·����Ҳ�����Ǿ���·��
bilibili.savePath = download/
#bilibili.savePath = D:\Workspace\bilibili\

#����ͬʱ����������
bilibili.download.poolSize = 3
```

## ��������ʹ������
* ʹ��org.json�����򵥵�Json������
* ʹ��zxing���������Ӷ�ά��ͼƬ��
* ʹ��ffmpeg����ת��(��Ƭ��flvδʹ��ffmpeg������flv�ϲ���m4sת��mp4��ʽ��Ҫ�õ�)

## Win32/Linux/Mac�û��뿴����
+ �Դ���```ffmpeg.exe```ΪWIN 64λ��32λϵͳ������ƽ̨������[����](http://www.ffmpeg.org/download.html)���أ��滻Դ����  
+ ���ڷ�WIN�û�����ֱ��ʹ�������е��øó���  
```javaw -Dfile.encoding=utf-8 -jar INeedBiliAV.jar```

## UPDATE  
* v2.6  
    * ���������Ƶ���ز��������� - ���ֵ�Ӱ�Ƿֶβ��ģ�ԭ���ķ�ʽֻ�����ش��ǰ5~6���ӣ�����<https://www.bilibili.com/bangumi/play/ss10007>
    * ��Ϊ����ôʹ�õ�¼����(һ�ε�¼cookies�����úܾ�)����ǰδ���ֲ�������Ϊ����ԭ����ɵ��쳣�����ѽ��
* v2.5  
    * �����ղؼе����ӽ���������<https://space.bilibili.com/3156365/favlist?fid=75463865>(url����ذ���fid����)
    * ����UP������ҳ������ӽ���������<https://space.bilibili.com/5276/video> 
    * ����UP������ҳ���ض�Ƶ�������ӽ���������<https://space.bilibili.com/378034/channel/detail?cid=189>     
    * �޸�ĳЩ���ӵ��쳣����������<https://www.bilibili.com/video/av41515020?from=search&seid=11021327663579949519>
    * ����ж�ؽű�```unistall.bat```(��ʵ����ɾ���ļ��С�����)
    * ��ǰ����ҳ���ȡ��Ϣ˳��Ϊ���·������ҹ̶�Ϊÿҳ5��(����ÿҳ30��)���Է�ֹ������Tabҳ����ࡣ��Ҫ��ȡ���ں������p=[pageNumber]��
    e.g. ��Ҫ����UP��```Hivane```���·����ĵ�31~35����Ƶ(��ȷ������û�пո�)    
    ```https://space.bilibili.com/17154307/video?tid=0&page=2&keyword=&order=pubdate p=7```
* v2.4  
    * ���ӹٷ�����URL���ϵ����ӽ���������<https://www.bilibili.com/bangumi/play/ss25739> 
    * ���ӹٷ�����URL���ϵ����ӽ���������<https://www.bilibili.com/bangumi/media/md134912>     
    * (UI)�Ż����ͬʱ����������ʾ
    * (UI)�޸����Ż�����UI��ʾ
* v2.3 
    * (UI)���������ٶ���ʾ   
    * (UI)����vbs�ű������Դ��������ݷ�ʽ  
    * (UI)�����ļ�ͳһ����config�ļ�����
    * ��ѡ��ΪMP4��Ŀ��Դ������FLVʱ���Ż�Ϊ�Զ��л�FLV  
    * �޸�һ��bug����bugʹ���ڵ���ffmpegת��ʱ���и��ʻ�ʧ�ܿ�ס  
    * ���ӹٷ�����URL(����)�����ӽ���������<https://www.bilibili.com/bangumi/play/ep250435>  
    * �������ط���Ĺ���(��ǰһֱ���Ե�UP���ϴ�����Ƶ��ͻȻ����׷���Ļ��ƺ��е㲻ͬ�������������������)       
    * PS�� ep��תav����ֱ�Ӵ�HTML�����������ģ��������ţ���ʱ��û��ȡ���ṩapi�ӿ�...
* v2.2 
    * ������HTML5����Դ�����ط�ʽ,֧��FLV/MP4���ָ�ʽ 
    * (UI)��������Ż�Ϊ�����������ͬ����Ƶ��������(���ֱ�������)
    * (UI)������Ŀ¼��������������```rename.bat```��Ĭ�ϸ�ʽΪ```avId-qn-p.(flv|mp4)```������ʹ�ø������������ı���Ϊ```��Ƶ����-qn-p.(flv|mp4)```(������������ֻ֧��Windows)
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




