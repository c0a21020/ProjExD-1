# 第6回
## 迷路 (ex6/maze.py)
### ゲームの概要
- ex13/maze.pyを実行すると、1500x900に迷路が描写され、迷路に沿ってを
   スタートからゴールまで移動させるゲーム
- 実行するたびに迷路の構造は変化する
- 穴掘り法という手法で迷路を作成(穴掘り法の説明はメモ)
### 操作方法
  - 矢印キーで上下左右に移動する
  - 通路を辿ってゴールを目指す

### 追加機能
 - スタートとゴールの設定
 - 答えの表示
 - ゴールすると"ゲームクリア"と表示する
 - スタートからゴールまでの経過時間を、ゴール後にメッセージボックスで表示する（遠藤）
 - 自分の通った道に色が付く   #三島

### ToDo(実装しようと思ったけど時間が無かった)
 - 画像の挿入　＃丸山　
 - コンティニューしたらもう一度迷路生成してゲームを始める #丸山　久保
 - コンティニュークリアしてコンティニューしたら迷路がさらに細かくなる  #迷路のサイズ設定で数値を大きくする #三島
 - 壁の貫通 #久保
 - 時間の表示 #遠藤

 ### メモ

 # 穴掘り法
 - 最初全てのマスを壁と設定し、そこからランダムに穴を掘ることで「通路」を作成していく手法

 # ゲーム表示の流れ
 - ゲームの起動
 - ゲームのプレイ
 - 迷路の解答表示
 
 # 迷路ゲームの起動
 - 壁と穴の設定
 - スタートとゴールの設定
 - 迷路を表示

 # 実装の手順
 - 最初に色や場所の定義
 - class Maze():でゲームを起動するときの関数を設定(値をNoneにする)
 - 