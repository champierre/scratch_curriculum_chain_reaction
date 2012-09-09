# スクラッチでピタゴラスイッチマシーンを作ろう

## LICENSE

<a rel="license" href="http://creativecommons.org/licenses/by-sa/3.0/deed.ja"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="http://i.creativecommons.org/l/by-sa/3.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">スクラッチでピタゴラスイッチマシーンを作ろう</span> by <span xmlns:cc="http://creativecommons.org/ns#" property="cc:attributionName">Junya Ishihara</span> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/3.0/deed.ja">Creative Commons 表示 - 継承 3.0 非移植 License</a>.

## 概要

Scratch@MIT 2012 でおこなわれた [Pre-Conference Workshops](http://events.scratch.mit.edu/conference/workshops.html)
のうちのひとつ、Physical-Digital Chain Reaction: WeDo and Scratch を参考にしたワークショップです。

スクラッチになのぼーどAGをつなげ、光センサとLEDの点灯を制御して光のリレーをおこなうことで、テレビ「ピタゴラスイッチ」にでてくるようなマシーンを参加者全員のスクラッチをつなげて作ります。

光センサで左隣の人の LED の点灯を受け取ったら、例えば画面左上からボールを転がして画面右下にボールが到達したら LED を点灯させるようなプロジェクトをスクラッチで作って、右隣の人のスクラッチに伝えます。

これを全員のスクラッチをつなげておこなうことで、一番左端のマシンから一番右端のマシンまで次々と伝わるピタゴラスイッチマシーンがスクラッチ上に完成します。

## 1. アイスブレイク（10分）

MITのワークショップでおこなわれたアイスブレイクです。

参加者全員が輪になり、手をつなぎあいます。

左手をギュッとつかまれたら、今度は右隣の人の手をギュッと握るよう全員に伝えます。

ファシリテーターがスタートとなり、右手をギュッとにぎります。

左手をつかまれたファシリテーターの右隣の人は、その右隣の人の手を握り、そのまた右隣の人の手を握る… と繰り返していくことで、つぎつぎ連鎖して、最後はファシリテーターの左手が握られ、そこでファシリテーターは左手が握られたことを伝え「ゴール」を宣言します。

これからつくるピタゴラスイッチマシーンは、同じ要領で動くことをイメージさせることができます。

## 2. 明るさセンサをつかった簡単なプロジェクト（20分）

なのぼーどAG とスクラッチをつなげる。

まずは接続テスト。調べる > スライダーセンサの値 の上で右クリックして「ScratchBoard監視板の表示」を選ぶ。

スライダーを動かしたり、明るさセンサの上に手をかざしたりして、各センサーの値が変わることを確認する。

明るさによってオンオフされるスイッチをスクラッチ上につくる。

![](https://raw.github.com/champierre/scratch_curriculum_chain_reaction/master/light_sensor.gif)

![](https://raw.github.com/champierre/scratch_curriculum_chain_reaction/master/light_sensor_costumes.png)

## 3. LED を点灯させる簡単なプロジェクト（20分）
LED を9番ピンとGNDに接続(9番のほうに長い端子)、Motion の motor on と motor off ブロックで LED を on/off できることを確認する。

![](https://raw.github.com/champierre/scratch_curriculum_chain_reaction/master/led_connection.jpg)

<img src="https://raw.github.com/champierre/scratch_curriculum_chain_reaction/master/led_connection.jpg" width="400">

![](https://raw.github.com/champierre/scratch_curriculum_chain_reaction/master/led_connection2.jpg)

![](https://raw.github.com/champierre/scratch_curriculum_chain_reaction/master/led_on_off.gif)

このプロックを利用して、ボタンを押したら LED が点灯する簡単なプロジェクトを作成する。

![](https://raw.github.com/champierre/scratch_curriculum_chain_reaction/master/led_switch.gif)

ボタンのコスチュームには、スクラッチ標準コスチュームから、Things > button と buttonPressed を利用する。 

![](https://raw.github.com/champierre/scratch_curriculum_chain_reaction/master/led_switch_costumes.png)

## 4. 上記2. 3.を組み合わせ、手をかざせば LED が点く「超能力マシーン」をつくる（20分）

![](https://raw.github.com/champierre/scratch_curriculum_chain_reaction/master/force.gif)

## 5. ピタゴラスイッチマシーンをつくる(60分)
参加者全員の机を輪の形に並べ替える。

左隣の人のなのぼーどから LED を伸ばしてきて、自分の明るさセンサに接続する。

自分の LED を伸ばし右隣の人の明るさセンサと接続する。

明るさセンサの値が高くなったら起動し、プロジェクトが終了するタイミングで LED を点灯させるプロジェクトをつくる。

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

