# Career Select 【学生限定】技術勉強会
Gitが使えなきゃエンジニアになれない？今更聞けないGitの基礎から学びませんか？

## 開催日程
2022.11.29（火）19:00 〜

## 資料
[Google Slides](https://docs.google.com/presentation/d/1WbVd15vvakbYRTfM_9GjZT9O5Z80fb9kf-csTrmUkIE/edit#slide=id.p)

## コマンド
### コマンドを実行するためのターミナル
お使いのPCに合わせて以下のようなターミナルのアプリをご利用ください
```
▶︎　Windows
・コマンドプロンプト / GitBash / VSCodeのターミナル機能

▶︎ Mac
・ターミナル / VSCodeのターミナル機能
```
### Git初期設定
以下のGit初期設定を行なっていない場合は、コマンドを実行してください
```
$ git config --global user.name "ユーザ名"
$ git config --global user.email "メールアドレス"
```

### リポジトリをcloneする作業ディレクトリへ移動（場所は任意）
デスクトップにcloneする場合

#### Windows (コマンドプロンプト）
```
コマンドプロンプトを立ち上げた初期状態で
> cd Desktop

または、
> cd C:¥Users¥ユーザ名¥Desktop
```

#### Mac (ターミナル)
```
$ cd ~/Desktop
```


### clone 〜 push
#### 1. リモートリポジトリからリポジトリをclone
```
$ git clone https://github.com/mizu0715/git-seminar.git
```

#### 2. プロジェクトのルートディレクトリに移動
```
$ cd git-seminar
```

#### 3. 作業用のブランチ作成
※今回、ブランチ名は自分の名前で作成してください test-[自分の名前] 
```
$ git checkout -b [ブランチ名]

ex) git checkout -b test-mizuno 
```

#### 4. ファイルの修正
[issue](https://github.com/mizu0715/git-seminar/issues/1)はこちら

`git-semier/src/sample.html` または、 `git-semier/src/sample.txt` を修正してください

修正ファイルの状態は下記のコマンドで確認
```
$ git status
```


#### 5. ステージングエリアにadd
```
$ git add src/sample.html ・・・htmlを修正した場合
$ git add src/sample.txt  ・・・txtを修正した場合

または

$ git add .　（修正した全ファイルをadd）
```

#### 6. ローカルリポジトリにcommit
```
$ git commit -m '[コミットメッセージ]'

ex) git commit -m 'テキスト修正'
```

#### 7. リモートリポジトリにpush
※ブランチ名は③で作成した自分の名前のものを指定してください 
 ```
$ git push origin [ブランチ名]

ex) git push origin test-mizuno 
```
