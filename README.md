# Unityで作ったゲームをWebGLでBuildしてGitHubでプレイする
## 動作環境
1. Windows 10 Home 21H2
2. Unity version 2021.1.21f1  

![image](https://user-images.githubusercontent.com/93690866/153183424-a7ce9019-366a-4128-8972-56ba412e9192.png)
## Unityで作ったゲームをWegGLでBuildする
Unityを開いて操作します。
### 1. 「Edit」->「Project Setting...」  
![image](https://user-images.githubusercontent.com/93690866/153186084-b1c2c69c-4573-468f-ab7b-f631b72f9e70.png)  

### 2. 「Publishing Settings」->「Compression Format」をDisabledに変更する。  
![image](https://user-images.githubusercontent.com/93690866/153187485-6952e43c-4ebd-4a87-aa95-cdafed1ca24b.png)  

### 3. 「File」->「Build Settings...」  
![image](https://user-images.githubusercontent.com/93690866/153189212-78c7b840-1c33-497b-bb24-15c01c2fd82f.png)  

### 4. 「WebGL」に設定->「Build」  
![image](https://user-images.githubusercontent.com/93690866/153189567-57ea7926-e5d3-4cc6-ba35-0537ad756c8d.png)  

### 5. 保存先フォルダを指定。ここでは新規フォルダ「Buildgithub」を作成して保存先に指定  
![image](https://user-images.githubusercontent.com/93690866/153190449-18f0500e-4ae4-4a24-b52d-7f0ad64e5fae.png)  

## BuildしたデータをGitHubにアップする
### 1. GitHubで新しいRepositoriesを作成  
![image](https://user-images.githubusercontent.com/93690866/153192382-016b1bd4-c72b-467b-a7e8-ac26f0328905.png)  

### 2. Repositoriesの名前と公開設定などを指定。「Public」にしないとうまくいかなかった（後で詳細について説明あり）  
   「Repository name」を入力（->「Description」の記入はどっちでも）->「Public」->「Create repository」  
![image](https://user-images.githubusercontent.com/93690866/153193243-ee074af4-8f68-4ff1-b246-178dd86f2167.png)  

### 3. GitHub Desktopを使用してBuildしたファイルをクローンする  
   HTTPSを選択し「Set up in Desktop」をクリック
![image](https://user-images.githubusercontent.com/93690866/153194348-16eb26d1-5c25-41a3-9f4c-330c4d100d6c.png)  
   「clone」をクリック
![image](https://user-images.githubusercontent.com/93690866/153196934-369097fb-5fca-4495-9ae5-da1c14e7262b.png)  

### 4. cloneしたrepositoryにBuildしたファイルをアップする  
   Buildしたデータ（1.Build, 2.TemplateData, 3.index）をコピー（or切り取り）して、gitHubのフォルダ貼り付ける  
![image](https://user-images.githubusercontent.com/93690866/153191574-22092c6c-ed92-4ff4-aed7-8c2a3b8064fc.png)  


