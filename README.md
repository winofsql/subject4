# subject4

[xampp-windows-x64-8.2.12-0-VS16-installer.exe](https://sourceforge.net/projects/xampp/files/XAMPP%20Windows/8.2.12/)

![image](https://github.com/winofsql/subject4/assets/1501327/b682ab09-c687-4efb-ab30-6ede841ae630)

![image](https://github.com/winofsql/subject4/assets/1501327/d830f511-788b-47ce-8a1b-908576d67eef)

![image](https://github.com/winofsql/subject4/assets/1501327/70dfef74-63ef-4b20-9ff1-ece42b3b26b7)

![image](https://github.com/winofsql/subject4/assets/1501327/9a8fb14f-553f-4e9a-a7c3-56c76d455c9f)

xampp-control.exe は いったん終了して、管理者権限で実行します

![image](https://github.com/winofsql/subject4/assets/1501327/df478fc1-7caa-4247-b2c2-f180b3b5e44e)

php-subject-sqlite.bat
```
@echo off
title subject4
if exist c:\Users\%USERNAME%\Downloads\subject4 (
	c: 
	cd \Users\%USERNAME%\Downloads
	ren subject4 subject4-%date:~5,2%%date:~8,2%-%RANDOM%
	git clone https://github.com/winofsql/subject4.git
	cd subject4
	rmdir .git /S /Q 
	Code lightbox.code-workspace
) else (
	c: 
	cd \Users\%USERNAME%\Downloads
	git clone https://github.com/winofsql/subject4.git
	cd subject4
	rmdir .git /S /Q 
	Code lightbox.code-workspace
)
```

![image](https://github.com/winofsql/subject4/assets/1501327/dd0d8022-a4f1-44a8-8b1e-eae13bb5435a)

Visual Studio Code を閉じる

![image](https://github.com/winofsql/subject4/assets/1501327/dcc99fa5-6e73-426d-9957-a398e3259848)

script-download.vbs 実行

code-install-ext.bat 実行

lightbox.code-workspace で Visual Studio Code を実行

![image](https://github.com/winofsql/subject4/assets/1501327/47765f45-1aa6-4f1f-8788-9b97d609b11f)

日本語選択

![image](https://github.com/winofsql/subject4/assets/1501327/e5d4c194-0d7a-435a-a13c-079d994a755c)

![image](https://github.com/winofsql/subject4/assets/1501327/8107844d-f202-434f-8d93-2dae622b4ee8)

![image](https://github.com/winofsql/subject4/assets/1501327/8e8a31fd-0d93-4c0c-ac3c-1052ded46249)

フォルダ作成でそのフォルダを Apache の 仮想パスとして登録\
( "C:\xampp\apache\conf\extra\httpd-lightbox.conf" )
```
<IfModule alias_module>

    Alias /php-0506-01 "C:\Users\lightbox\Downloads\subject4\php-0506-01"
    <Directory "C:\Users\lightbox\Downloads\subject4\php-0506-01">
        Options Indexes ExecCGI
        AllowOverride All
        Require all granted
        ErrorDocument 403 /error/XAMPP_FORBIDDEN.html.var
    </Directory>

</IfModule>
```

![image](https://github.com/winofsql/subject4/assets/1501327/8352e4ab-5cfb-4946-9443-00fef30ff69b)

![image](https://github.com/winofsql/subject4/assets/1501327/2fbf0d7a-44f7-481d-be6c-1ac9ee53a546)

![image](https://github.com/winofsql/subject4/assets/1501327/3afb3379-0fc4-4a38-8a8f-48f31dbe4ef2)

Apache を起動して　仮想パスを有効にする

![image](https://github.com/winofsql/subject4/assets/1501327/26ae9ccb-d527-44ac-9942-5febf4e1242b)

![image](https://github.com/winofsql/subject4/assets/1501327/73db47b8-dab5-45c9-8330-6de83d6dc43f)

![image](https://github.com/winofsql/subject4/assets/1501327/b80c3871-14bb-42ea-8c2c-ba14f5ea292a)

![image](https://github.com/winofsql/subject4/assets/1501327/d13c3177-9f5b-4179-aaea-4135fc31c878)

![image](https://github.com/winofsql/subject4/assets/1501327/6ef1a491-d43a-4a48-ab3f-5b03736e2c1a)
