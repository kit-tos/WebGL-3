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
![image](https://user-images.githubusercontent.com/93690866/153203754-3b54d9b7-cef4-41d4-9d5f-5e27e83234b6.png)  

### 2. Repositoriesの名前と公開設定などを指定。「Public」にしないとうまくいかなかった（6.で詳細について説明あり）  
   「Repository name」を入力（->「Description」の記入はどっちでも）->「Public」->「Create repository」  
![image](https://user-images.githubusercontent.com/93690866/153193243-ee074af4-8f68-4ff1-b246-178dd86f2167.png)  

### 3. GitHub Desktopを使用してBuildしたファイルをクローンする  
   HTTPSを選択し「Set up in Desktop」をクリック
![image](https://user-images.githubusercontent.com/93690866/153194348-16eb26d1-5c25-41a3-9f4c-330c4d100d6c.png)  
   「clone」をクリック
![image](https://user-images.githubusercontent.com/93690866/153196934-369097fb-5fca-4495-9ae5-da1c14e7262b.png)  

### 4. cloneしたrepositoryにBuildしたファイルをアップする  
   Buildしたデータ（1.Build, 2.TemplateData, 3.index）をコピー（or切り取り）して、gitHubのフォルダ貼り付ける  
![image](https://user-images.githubusercontent.com/93690866/153198046-bdaa241d-74a1-4c97-8f94-0a41ef36ecc9.png)   
![image](https://user-images.githubusercontent.com/93690866/153197846-c5c81205-dd45-45f8-beb4-8e672bb455da.png)  

### 5. GitHub Desktopでmainにcommitする  
   Summary (required)に何か記入する。ここではtestと入力 -> 「Commit to main」
![image](https://user-images.githubusercontent.com/93690866/153198631-b977f061-b7ad-40e8-affc-00f0c7bf18d8.png)  
   「Publish branch」をクリック  
![image](https://user-images.githubusercontent.com/93690866/153198874-9dc10f27-2f00-4184-977b-82c734d299ed.png)  

### 6. GitHubでBuildしたゲームのURLを取得する
   「Settings」->「GitHub Pages」->「Chenk it out here!」※2.でPublicにしないとGitHub Pagesから次に進まなくなる
![image](https://user-images.githubusercontent.com/93690866/153199619-fbe7701a-5449-4b6b-82c0-b38e47cc1c17.png)  
![image](https://user-images.githubusercontent.com/93690866/153199801-2513be98-af7c-4d0c-9828-8082e4abd623.png)  

   「GitHub Pages」->「Source」->「None」を「main」に変更->「Save」
![image](https://user-images.githubusercontent.com/93690866/153200506-e1b2d483-4fb1-4150-80cf-c9e4f94e3995.png)  

   得られたURLをコピーする。ちなみにクリックしたら遊べます
![image](https://user-images.githubusercontent.com/93690866/153201120-b6b5b7a9-acc5-4753-a3a0-c768865176de.png)  

### 7. GitHubのCode画面にゲームのURLを貼り付ける
   「Code」->「About ⚙」->「Descriptin」にコメント記入->「Website」に取得したゲームのURLを張り付ける->「Save Changes」
![image](https://user-images.githubusercontent.com/93690866/153203204-14bd3a48-1990-4f97-8f50-22c1a8063637.png)  

### 終了

## 実際に遊んでみる
「About ⚙」欄のURLをクリック
![image](https://user-images.githubusercontent.com/93690866/153203417-92cac98d-328b-433e-ab44-8af262600147.png)





   


