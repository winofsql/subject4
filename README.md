# subject4

[xampp-windows-x64-8.2.12-0-VS16-installer.exe](https://sourceforge.net/projects/xampp/files/XAMPP%20Windows/8.2.12/)

![image](https://github.com/winofsql/subject4/assets/1501327/b682ab09-c687-4efb-ab30-6ede841ae630)

![image](https://github.com/winofsql/subject4/assets/1501327/d830f511-788b-47ce-8a1b-908576d67eef)

![image](https://github.com/winofsql/subject4/assets/1501327/70dfef74-63ef-4b20-9ff1-ece42b3b26b7)

![image](https://github.com/winofsql/subject4/assets/1501327/9a8fb14f-553f-4e9a-a7c3-56c76d455c9f)

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

![image](https://github.com/winofsql/subject4/assets/1501327/dcc99fa5-6e73-426d-9957-a398e3259848)

