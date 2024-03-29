# Browser演習
[スライド１](https://docs.google.com/presentation/d/1emAO8kYDATx3UGa3YF3lxLXXtFi-d29DzJjQMjj-RGA/edit#slide=id.g3880609f79_0_67)
[スライド２](https://docs.google.com/presentation/d/1Bv_ykboY-8pOTNbGafVkYiInl4qHKJXlLd0aVydm044/edit#slide=id.g3880609f79_0_139)


# １日目午前

## ブラウザの内部処理
1. リソースをサーバから読み取る（load）  
2. データの解釈（parse）
3. 画面上に要素を配置（layout）
4. コンテンツを描画して配置（paint）
5. Event Handling

## ブラウザの技術
- フォント
    - [ヒンティング](https://ja.wikipedia.org/wiki/フォントヒンティング)
    - [リガチャ](https://ja.wikipedia.org/wiki/合字)
    - 絵文字
- 文字コード
    - 今は日本語も含めて[UTF-8](https://ja.wikipedia.org/wiki/UTF-8)がほとんど
- SSL
    - 通信の暗号化
    - サーバ・クライアントの証明
- audio/video
    - ハードウェアの機能を使用
    - ソフトウェアでのリアルタイム処理が困難

## 上級編
### JIT
- [Just In Time](https://wa3.i-3-i.info/word17000.html)
- JSなどのコードを実行するCPU専用のネイティブプログラムに変換してから実行
- 関数ごとにコンパイル（全てをコンパイルしない）

### Accelerated Composing
- [説明](https://ginpen.com/2013/12/06/hardware-acceleration/)
- GPUを使ってアニメーションを滑らかにする仕組み

### キャッシュ
- 処理結果を残して再処理を書く

### マルチプロセス
- サンドボックス化
- 処理の高速化

# １日目午後

## 組み込みブラウザ

- non PC/Smartphoneのためのブラウザ
- WebKit or Chrominum

## テレビのブラウザ

- dボタン
    - HTMLアプリを実現
- Hybridcast Connect
    - 放送とアプリの通信連携

- 開発
    - リモコン操作
    - 独自の仕様（JLabやhbb）
    - 大画面むけのチューニング

## ゲーム
- ゲームがブラウザをもつケースとその逆

## 車
- Jaguar Land Rover
- In-Vehicle-Infotaiment(IVI) 
- 開発
    - 安全最優先
    - 走行中の利用制限

## 演習
- WebAssembly
- WebXR
- PresentationAPI
    - powerpointのような機能

# 2日目

## WebRTC
- Peer to Peer
- ビデオチャットの機能
- [アプリ](https://appr.tc/)
- [communication](https://antmedia.io/webrtc-servers/)
    - MESH
    - SFC
    - MCU
- MMU(Memory Management Unit)
    - プロセス間の干渉をブロックする
    - ハードウェアの単位で割り当てられるメモリを制限
    - メモリ破壊の原因を特定できる
- IPC(プロセス間通信)
    - v4l2loopback