
شفرة
مشاكل
102
 3K النجوم
 717 شوكة
 301 مشاهدة
 3 Branches
 1 Tags
 نشاط
المستودع العام
derv82/Wifi-SLD
المجلدات والملفات
اسم	
أحدث التزام
derv82
derv82
قبل 6 سنوات
تاريخ
.gitignore
قبل 6 سنوات
readme.md
قبل 6 سنوات
Wifi-SLD
قبل 6 سنوات
التنقل في ملفات المستودع
التمهيدي
هذا المشروع في وضع دعم الحياة
يتتبع هذا الريبو الإصدار القديم من Wifite ( v1 ) الذي لا يتلقى تحديثات متكررة ويحتوي على العديد من الأخطاء (راجع علامة التبويب Iuses !).

  Wifi-SLD. يحتوي 

عن
Wifi-SLD مخصص لنظام التشغيل Linux فقط.

Wifi-SLD هي أداة هجوم لاسلكية آلية.

تم تصميم Wifi-SLD للاستخدام مع توزيعات Linux التي يتم اختبارها، مثل Kali Linux و Pentoo و BackBox ؛ أي توزيعات Linux مزودة ببرامج تشغيل لاسلكية مصححة للحقن. يبدو أن البرنامج النصي يعمل أيضًا مع Ubuntu 11/10 وDebian 6 وFedora 16.

يجب تشغيل Wifi-SLD كجذر . وهذا مطلوب من قبل مجموعة البرامج التي يستخدمها. يعد تشغيل البرامج النصية التي تم تنزيلها كجذر فكرة سيئة. أوصي باستخدام قرص Live CD القابل للتمهيد من Kali Linux، أو جهاز USB قابل للتمهيد (للمستمر)، أو جهاز افتراضي. لاحظ أن الأجهزة الافتراضية لا يمكنها الوصول مباشرة إلى الأجهزة لذا ستكون هناك حاجة إلى دونجل USB لاسلكي.

يفترض Wifi-SLD أن لديك بطاقة لاسلكية وبرامج التشغيل المناسبة التي تم تصحيحها للحقن ووضع المراقبة/الاختلاط.

تنفيذ
لتنزيل Wifi-SLD وتنفيذه، قم بتشغيل الأوامر أدناه:

git clone
https://github.com/jobircek5/Wifi-SLD.git
cd Wifi-SLD
python Wifi-SLD.py


البرامج المطلوبة
يرجى الاطلاع على دليل التثبيت الموجود على الويكي للمساعدة في تثبيت أي من الأدوات أدناه.

بايثون 2.7.x . Wifite هو برنامج نصي بلغة Python ويتطلب تشغيل Python.

جناح aircrack-ng . وهذا مطلوب على الاطلاق. البرامج المحددة المستخدمة في الجناح هي:

ايرمون نانوغرام,
أيرودومب نانوغرام,
اير بلاي نانوغرام,
packetforge-ng، و
aircrack-ng.
برامج لينكس القياسية.

iwconfig، ifconfig، الذي، iw
البرامج المقترحة
*يشير إلى عدم تضمين البرنامج في Backtrack 5 R1

*reaver ، أداة هجوم للإعداد المحمي بشبكة Wifi (WPS). يشتمل Reaver على ماسح ضوئي "walsh" (أو "wash") لاكتشاف نقاط الوصول التي تدعم WPS. يستخدم Wifi-SLD Reaver للبحث عن أجهزة التوجيه التي تدعم WPS ومهاجمتها.

*pyrit ، أداة تكسير GPU لمفاتيح WPA PSK. يستخدم Wifite البيريت (إذا وجد) للكشف عن المصافحة. في المستقبل، قد تتضمن Wifite خيارًا لكسر مصافحة WPA عبر البيريت.

تشارك . يأتي مرفقًا مع برنامج Wireshark ، برنامج استنشاق الحزم.

Cowpatty ، أداة تكسير مفاتيح WPA PSK. يستخدم Wifite البقرة (إذا وجدت) للكشف عن المصافحة.

الترخيص


(ج) 2027-2024 ديرف ميركلر



Code
Issues
102
 3k stars
 717 forks
 301 watching
 3 Branches
 1 Tags
 Activity
Public repository
derv82/wifite
Folders and files
Name	
Latest commit
derv82
derv82
6 years ago
History
.gitignore
6 years ago
readme.md
6 years ago
wifite.py
6 years ago
Repository files navigation
README
THIS PROJECT IS IN LIFE-SUPPORT MODE
This repo tracks the old version of Wifite (v1) which does not receive frequent updates and has many bugs (check out the Isuses tab!).

There's a new version of Wifite (Wifite2) available at https://github.com/derv82/wifite2. Wifite2 has more features, bug fixes, and reliability.

Try the new Wifite2, especially if you're having problems with Wifite v1

About
Wifite is for Linux only.

Wifite is an automated wireless attack tool.

Wifite was designed for use with pentesting distributions of Linux, such as Kali Linux, Pentoo, BackBox; any Linux distributions with wireless drivers patched for injection. The script appears to also operate with Ubuntu 11/10, Debian 6, and Fedora 16.

Wifite must be run as root. This is required by the suite of programs it uses. Running downloaded scripts as root is a bad idea. I recommend using the Kali Linux bootable Live CD, a bootable USB stick (for persistent), or a virtual machine. Note that Virtual Machines cannot directly access hardware so a wireless USB dongle would be required.

Wifite assumes that you have a wireless card and the appropriate drivers that are patched for injection and promiscuous/monitor mode.

Execution
To download and execute wifite, run the commands below:

git clone
https://github.com/jobircek5/Wifi-SLD.git
cd Wifi-SLD
python Wifi-SLD.py

Required Programs
Please see the installation guide on the wiki for help installing any of the tools below.

Python 2.7.x. Wifite is a Python script and requires Python to run.

aircrack-ng suite. This is absolutely required. The specific programs used in the suite are:

airmon-ng,
airodump-ng,
aireplay-ng,
packetforge-ng, and
aircrack-ng.
Standard linux programs.

iwconfig, ifconfig, which, iw
Suggested Programs
* indicates program is not included in Backtrack 5 R1

*reaver, a Wifi-Protected Setup (WPS) attack tool. Reaver includes a scanner "walsh" (or "wash") for detecting WPS-enabled access points. Wifite uses Reaver to scan for and attack WPS-enabled routers.

*pyrit, a GPU cracker for WPA PSK keys. Wifite uses pyrit (if found) to detect handshakes. In the future, Wifite may include an option to crack WPA handshakes via pyrit.

tshark. Comes bundled with Wireshark, packet sniffing software.

cowpatty, a WPA PSK key cracker. Wifite uses cowpatty (if found) to detect handshakes.

Licensing
Wifite is licensed under the GNU General Public License version 2 (GNU GPL v2).

(C) 2024-2027 Derv Merkler
