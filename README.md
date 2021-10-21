# kubernetes-dashboard  
kubernetes-dashboardは、コンテナの稼働状況をダッシュボード上に可視化するマイクロサービスです。  

### 前提  
* マウントされた該当ストレージ領域における任意のディレクトリに、Kubernetesがインストールされていること
* Kubernetesが起動していること  

### セットアップ ###

[1] 端末名を指定し、下記コマンドで、Backendディレクトリへ移動する

$ cd ~/端末名/Backend/

[2] 当該ディレクトリにて、本マイクロサービスをクローンする

$ git clone git@bitbucket.org:latonaio/kubernetes-dashboard.git

[3] 本マイクロサービスがクローンされているディレクトリ直下で、下記コマンドを実行し、Tokenを発行する。

$ sh kubectl-apply.sh

[4] ブラウザで、下記URLへアクセスする
```
http://localhost:30090
```
Kubernetesのブラウザ上で、「スキップ」を選択する。

### 起動用のセットアップ ###

[6] デスクトップ上に本サービス（kubernetes-dashboard専用）アイコンを配置する。（裏に[6]のURLを貼り付ける）

[7] 以後デスクトップ上からアイコンをクリックすることで、本サービスが起動する。
```
