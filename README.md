# スクラッチでピタゴラ装置を作ろう

## LICENSE

<a rel="license" href="http://creativecommons.org/licenses/by-sa/3.0/deed.ja"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="http://i.creativecommons.org/l/by-sa/3.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">スクラッチでピタゴラ装置を作ろう</span> by <span xmlns:cc="http://creativecommons.org/ns#" property="cc:attributionName">OtOMO</span> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/3.0/deed.ja">Creative Commons 表示 - 継承 3.0 非移植 License</a>.

## 概要

Scratch@MIT 2012 でおこなわれた [Pre-Conference Workshops](http://events.scratch.mit.edu/conference/workshops.html)
のうちのひとつ、Physical-Digital Chain Reaction: WeDo and Scratch を参考にし、OtOMO主催でおこなわれた [9月定期ワークショップ「スクラッチでピタゴラスイッチマシーンを作ろう」](http://scratch-ja.org/2012/08/1815)のために用意したワークショップの手引きです。

スクラッチになのぼーどAGをつなげ、光センサとLEDの点灯を制御して光のリレーをおこなうことで、テレビ「ピタゴラスイッチ」にでてくるようなマシーンを参加者全員のスクラッチをつなげて作ります。

光センサで左隣の人の LED の点灯を受け取ったら、例えば画面左上からボールを転がして画面右下にボールが到達したら LED を点灯させるようなプロジェクトをスクラッチで作って、右隣の人のスクラッチに伝えます。

これを全員のスクラッチをつなげておこなうことで、一番左端のマシンから一番右端のマシンまで次々と伝わるピタゴラスイッチマシーンがスクラッチ上に完成します。

## 必要なもの
* なのぼーどAG ([http://tiisai.dip.jp/?page_id=935](http://tiisai.dip.jp/?page_id=935))
* NanoBoardAGWithMotor (ダウンロードとインストール方法は [http://swikis.ddo.jp/WorldStethoscope/46](http://swikis.ddo.jp/WorldStethoscope/46) を参照してください)
* LED。+-両端子にリード線を接続、リード線のもう一方にはピンに刺せるよう針金をつける。LED の先端には切ったストローをかぶせると、となりのぼーどの明るさセンサにちょうど接続できる。

![](https://raw.github.com/champierre/scratch_curriculum_chain_reaction/master/led.jpg)

↑LED の先端には切ったストローをかぶせる

![](https://raw.github.com/champierre/scratch_curriculum_chain_reaction/master/led2.jpg)

↑リード線のもう一方にはピンに刺せるよう針金をつける

## 1. アイスブレイク（10分）

MITのワークショップでおこなわれたアイスブレイクです。

参加者全員が輪になり、手をつなぎあいます。

左手をギュッとつかまれたら、今度は右隣の人の手をギュッと握るよう全員に伝えます。

ファシリテーターがスタートとなり、右手をギュッとにぎります。

左手をつかまれたファシリテーターの右隣の人は、その右隣の人の手を握り、そのまた右隣の人の手を握る… と繰り返していくことで、つぎつぎ連鎖して、最後はファシリテーターの左手が握られ、そこでファシリテーターは左手が握られたことを伝え「ゴール」を宣言します。

これからつくるピタゴラスイッチマシーンは、同じ要領で動くことをイメージさせることができます。

## 2. 明るさセンサをつかった簡単なプロジェクト（20分）

なのぼーどAG とスクラッチをつなげる。

まずは接続テスト。「調べる」> 「スライダーセンサの値」の横のチェックボックスをチェックしてボードを自動検出させる。

「スライダーセンサの値」上で右クリックして「ScratchBoard監視板の表示」を選ぶ。

スライダーを動かしたり、明るさセンサの上に手をかざしたりして、各センサーの値が変わることを確認する。

明るさによってオンオフされるスイッチをスクラッチ上につくる。

![](https://raw.github.com/champierre/scratch_curriculum_chain_reaction/master/light_sensor.gif)

![](https://raw.github.com/champierre/scratch_curriculum_chain_reaction/master/light_sensor_costumes.png)

## 3. LED を点灯させる簡単なプロジェクト（20分）
LED につなげたリード線を9番ピンとGNDに接続(9番のほうに長い端子(+))、動きの「モーターをオンにする」と「モーターをオフにする」ブロックで LED を on/off できることを確認する。

![](https://raw.github.com/champierre/scratch_curriculum_chain_reaction/master/led_connection.jpg)

![](https://raw.github.com/champierre/scratch_curriculum_chain_reaction/master/led_connection2.jpg)

![](https://raw.github.com/champierre/scratch_curriculum_chain_reaction/master/led_on_off.gif)

このプロックを利用して、ボタンを押したら LED が点灯する簡単なプロジェクトを作成する。

![](https://raw.github.com/champierre/scratch_curriculum_chain_reaction/master/led_switch.gif)

![](https://raw.github.com/champierre/scratch_curriculum_chain_reaction/master/led_switch2.gif)

ボタンのコスチュームには、スクラッチ標準コスチュームから、Things > button を利用する。 

![](https://raw.github.com/champierre/scratch_curriculum_chain_reaction/master/led_switch_costumes.png)

## 4. 上記2. 3.を組み合わせ、手をかざせば LED が点く「超能力マシーン」をつくる（20分）

時間が足りない場合は省略可能。

![](https://raw.github.com/champierre/scratch_curriculum_chain_reaction/master/force.gif)

## 5. ピタゴラ装置をつくる(60分)
参加者全員の机を輪の形に並べ替える。

左隣の人のなのぼーどから LED を伸ばしてきて、自分の明るさセンサに接続する。

自分の LED を伸ばし右隣の人の明るさセンサと接続する。

明るさセンサの値が高くなったら左端からボールが転がり始め、右端にボールが着いたら、LED を点灯させるプロジェクトをつくる。

プロジェクト例 明るさセンサの値が高くなると転がり出すボール ↓
![](https://raw.github.com/champierre/scratch_curriculum_chain_reaction/master/rolling_ball.png)

## 6. テスト(40分)
まずは自分のプロジェクトがちゃんと動くまでテスト。

次に左隣の人と接続してテスト。

右隣の人と接続してテスト。

最後に全体で総合テスト。

## 7. 本番(10分)
スタートのプロジェクトが見える位置に参加者全員移動。

つぎつぎプロジェクトが起動していくに従い移動。

できればビデオ撮影してあとでビデオを公開する。

## 8. 自由製作
最初(明るさセンサの値で左端よりボールを転がし始める)と最後(右端にボールがたどりついたらLEDを点灯させる)の部分は変更せず、その間はどんな動きをさせてもよいという条件で自由にプロジェクトを変更する。