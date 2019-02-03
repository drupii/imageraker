-------------------------------------------
About
-------------------------------------------

ImageRaker is an image download toolbar for Internet Explorer which has variety features for saving web images.

It includes:
 - Save images even if mouse right button is blocked in a web page
 - Immediate save
 - Automatic select images to download
 - Filter small size images

You can download offical installation file from below link.

Download:
https://imageraker.googlecode.com/svn/trunk/ImageRakerSetup/Releases/ImageRakerSetup_v0.8.1.msi

Official distribution:
http://ljh131.tistory.com/category/Projects/Image%20Raker

-------------------------------------------
Translated text
-------------------------------------------

readme for pub

-home
http://code.google.com/p/imageraker/


1. Differences from the actual version
Version check and delete url for error transmission.
Delete signing and setup project for deployment

Test sanding (pfx)
test123


2. post build event
Depending on whether os is 32 or 64 bits. The following is a post build event used in Win 7 64-bit.
(We use vs10 for development, but vs8 is required for assembly registration.)

"Microsoft Visual Studio 8 \ SDK \ v2.0 \ Bin \ gacutil" / if "$ (TargetDir) Interop.SHDocVw.dll" C: \ Program Files
"$ (TargetPath)" / if "" C: \ Program Files (x86) \ Microsoft Visual Studio 8 \ SDK \ v2.0 \ Bin \ gacutil "
"C: \ WINDOWS \ Microsoft.NET \ Framework \ v2.0.50727 \ regasm" / unregister "$ (TargetPath)"
"C: \ WINDOWS \ Microsoft.NET \ Framework \ v2.0.50727 \ regasm" / register "$ (TargetPath)"


3. The ie path for debugging is also used on 64-bit as follows.

C: \ Program Files (x86) \ Internet Explorer \ iexplore.exe

-------------------------------------------
Original text
-------------------------------------------
readme for pub

-home
http://code.google.com/p/imageraker/


1. 실제 버전과의 차이점
버전체크 및 에러 전송용 url 삭제.
배포용 사이닝 및 셋업 프로젝트 삭제

테스트용 사이닝(pfx) 비번 
test123


2. post build event
os가 32비트냐 64비트냐에 따라 다름. 다음은 윈7 64비트에서 사용한 post build event임.
(개발용으로 vs10을 사용하지만 어셈블리 등록을 위해 아래와 같이 vs8이 필요.)

"C:\Program Files (x86)\Microsoft Visual Studio 8\SDK\v2.0\Bin\gacutil" /if "$(TargetDir)Interop.SHDocVw.dll"
"C:\Program Files (x86)\Microsoft Visual Studio 8\SDK\v2.0\Bin\gacutil" /if "$(TargetPath)"
"C:\WINDOWS\Microsoft.NET\Framework\v2.0.50727\regasm" /unregister "$(TargetPath)"
"C:\WINDOWS\Microsoft.NET\Framework\v2.0.50727\regasm" /register "$(TargetPath)"


3. 디버깅을 위한 ie경로 역시 64비트에서는 아래와 같이 사용한다.

C:\Program Files (x86)\Internet Explorer\iexplore.exe



