#  WinUI 3를 사용하여 간단한 사진 뷰어 만들기
  
![image](https://github.com/gryrryfh/SimplePhotos/assets/50912987/9c46ce1a-574f-43a7-ae28-39e96cf377e8)  
  
## 프로젝트 설명  

 WinUI 3를 사용하여 간단한 사진 뷰어 만들기
   
Visual Studio WinUI3(빈앱, 패키지됨)  
![image](https://github.com/gryrryfh/SimplePhotos/assets/50912987/9814767a-bfe7-456c-9387-b848c6486895)  
프로젝트 이름 : SimplePhotos, 솔루션 및 프로젝트를 같은 디렉터리에 배치 해제  

Asserts아래에 Samples필터를 만들고 Assets\Samples폴더에 사진 추가 후 사진들 기존항목 추가  
![image](https://github.com/gryrryfh/SimplePhotos/assets/50912987/c688809e-fb1b-4e00-842e-a01c618b3cb6)  

솔루션탐색기-추가-새항목추가-Visual C++ - 코드 - Midl파일(.idl) ImageFileInfo.idl로 추가(이미지 파일의 모델)  
![image](https://github.com/gryrryfh/SimplePhotos/assets/50912987/5bb8a470-14c0-47be-92d1-aa72194a680d)  

Generated Files\sources의 ImageFileInfo.h, ImageFile.cpp파일 \SimplePhotos\SimplePhotos\에서 프로젝트에 포함  
![image](https://github.com/gryrryfh/SimplePhotos/assets/50912987/9c518b1b-252a-420c-bed6-a840cda985c4)  

GridView와 같은 항목 컨트롤과 관련된 또 다른 개념은 항목 컨테이너다.
항목 컨테이너는 항목을 Content 속성의 값으로 표시하는 콘텐츠 컨트롤
항목 컨트롤(GridV View)은 언제든지 화면에 보이는 항목을 표시하기 위해 필요한 만큼 항목 컨테이너를 만든다.
항목 컨트롤은 항목 컨테이너를 항목 패널 내부에 배치
일회성 바인딩은 런타임에 변하지 않는 데이터에 적합, 고성능, 쉽게 만들수 있음

ImageFileInfo.h, pch.h, ImageFileInfo.cpp, Mainwindow.idl, Mainwindow.xaml.cpp, Mainwindow.xaml 코드 추가  



### 출처 : https://learn.microsoft.com/ko-kr/windows/apps/get-started/simple-photo-viewer-winui3?tabs=cpp

