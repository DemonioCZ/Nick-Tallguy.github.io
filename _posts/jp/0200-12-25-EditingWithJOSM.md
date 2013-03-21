---
layout: doc
title: JOSMによるOpenStreetMap編集
permalink: /jp/beginner/editing-with-josm/
lang: jp
category: beginner
---

JOSMによるOpenStreetMap編集
======================

第3章ではJOSMをインストールし、最初のポイントやライン、シェイプの描き方を紹介しました。また、編集したオブジェクトに対して、プリセットを使って情報を追加する方法も紹介しています。これだけの知識でも、JOSMで地図を描くことは可能です。

しかし、第3章で紹介した知識はあくまでも最低限の操作方法だけです。そして、私たちの地図はこのままでは不正確です。私たちはまだ正しい位置情報を把握していないのです。しかし、ここまでの2章の間に、GPSとウォーキングペーパーという2つのツールを紹介しました。どちらも場所が有する位置情報を収集するツールです。位置情報は、2つの数字の組み合わせによって表現されます。

現実世界を紙の地図に描くには、ポイントやライン、シェイプの正しい位置を把握する必要があります。それに関しては、3章で私たちが描いたデジタル地図と紙の地図で変わることはありません。そして、デジタルの地図を描く際には、GPSの移動記録とウォーキングペーパーを使うことで、この地球上におけるそれら地点の正しい位置を知ることができます。

この章では、実際のOpenStreetMapの地図データを修正し、改良する方法について紹介します。まずは、OSM編集の基本的なサイクルは以下のようになります。

​1) 現在OSMデータベースに入力されているデータをダウンロード

​2) GPSやウォーキングペーパー、その他のノートを参考にして、情報を編集

​3) OpenStreetMapへデータをアップロードして保存

この章の内容を理解することで、OSMの地図上で自身が編集した情報を閲覧することができるようになるでしょう。

JOSMの準備
-------

-  コンピュータの画面左下に配置されているスタートメニューからJOSMを選択し、起動します。
-  起動が完了したら、GPSの移動記録gpxファイルとウォーキングペーパーをJOSMへ読み込んでください。2つのデータは同時に読み込んでも読み込まなくてもかまいません。JOSMでのファイル読み込み方法がわからない場合は、前述の2章の記述を参照してください。

  ![]({{site.baseurl}}/images/jp_beg_ch6_image09.png)

OSMデータのダウンロード
-------------

-  この章のイントロダクションで説明したOpenStreetMapの情報編集サイクルを思い出してください。ダウンロード、編集、セーブです。地図を編集可能な状態にするには、まずはあなたが描きたい地域のデータをダウンロードする必要があります。
-  既にGPXファイルやウォーキングペーパーを読み込んでいる場合は、そのデータが画面に表示され、自動的に当該の地域へ表示域が移動しているはずです。ファイルを読み込んだ後に、JOSMの左下を確認してみてください。マウスのある位置の緯度と経度(座標)が表示されます。

  ![]({{site.baseurl}}/images/jp_beg_ch6_image01.png)

-  編集したい地域を既に読み込んでいる場合、その地域のOpenStreetMapデータをダウンロードするのは簡単です。JOSM画面左上の"ファイル"→"OSMからダウンロード"をクリックすると、ダウンロード用の画面がポップアップします。この画面は、以下のダウンロードボタンをクリックすることでも呼び出すことができます。

  ![]({{site.baseurl}}/images/jp_beg_ch6_image08.png)

-  ダウンロード画面には、ピンク色の四角形が描かれた地図が表示されているはずです。地図が表示されない場合は、"スリッピーマップ"と書かれたタブをクリックしてください。

  ![]({{site.baseurl}}/images/jp_beg_ch6_image02.png)

-  ピンク色の四角形で囲まれた部分がダウンロードされ、編集用のデータとなります。GPSファイルやウォーキングペーパーを読み込ませた後、地域を移動させずにダウンロード画面を開いた場合、それらの地域を囲む形でピンク色の四角形が描かれます。もし自分で新しく四角形を描いた場合、より広い地域がダウンロードの対象となります。
-  新しく四角形を描く場合は、マウスを左クリックしたままドラッグしてください。左クリックをやめた地点を終点として、四角形が描かれます。ダウンロードする領域を決定したら、"ダウンロード"ボタンをクリックしてください。JOSMは自動的にその地域のOpenStreetMapデータをダウンロードし、編集用データとして画面に表示させます。

編集
--

-  次は実際に地図を編集し、新しいオブジェクトを追加してみましょう。慣れないうちは大変かもしれませんが、何度か練習して覚えてください。
-  ポイントやライン、シェイプを移動させる際には、"選択"ツールを使います。オブジェクトをクリックし、正しい位置へ移動させてください。こうすることで、誤った位置に配置されたオブジェクトを、正しい位置へ移動させることが可能です。

  ![]({{site.baseurl}}/images/jp_beg_ch6_image05.png)

-  ポイントやライン、シェイプを新しく描き足すには、"描画"ツールを使います。描いたオブジェクトに情報を追加するには、第3章で紹介したプリセットメニューを選択します。
-  GPSやウォーキングペーパーの内容が自動的にOpenStreetMapに保存されるわけではないことに注意してください。それらの情報をOSMへデジタル情報として追加するには、"描画"ツールを使う必要があります。GPS記録やウォーキングペーパーは、編集時の参考画像として背景に読み込まれます。
-  例えばGPSの記録に"030"と記されたポイントがあり、メモ帳には"030は学校"と書いてあるとしましょう。JOSMを使ってこのポイントをOpenStreetMapへ追加するには、まず描画ツールを選択し、地図編集領域に表示された"030"の位置でダブルクリックします。ポイントが作成されます。次にプリセットメニューを選択し、学校のプリセットを選択します。学校の名称を入力し、"プリセットの適用"を選択します。その他、ラインやシェイプについても同様に処理してください。

  ![]({{site.baseurl}}/images/jp_beg_ch6_image04.png)

変更のアップロード
---------

-  編集が終わったら、結果をOpenStreetMapへ保存しましょう。変更を保存するということはOpenSteetMapへ変更をアップロードする、ということでもありますので、インターネットへの接続環境が必要です。
-  トップメニューから"ファイル"を選択し、"データをアップロード"をクリックすると、アップロード画面がポップアップします。この画面は、以下のアップロードボタンをクリックすることでも呼び出すことができます。

  ![]({{site.baseurl}}/images/jp_beg_ch6_image00.png)

-  アップロード画面には、あなたが追加編集したオブジェクトが一覧で表示されています。下部に表示されたボックスには、あなたが行った変更に対するコメントの入力欄があります。行った変更の内容を入力してください。

  ![]({{site.baseurl}}/images/jp_beg_ch6_image03.png)

-  "UploadChanges"をクリックしてください。
-  はじめてOpenStreetMapへ変更を保存する際にはユーザ名とパスワードの入力を求められます。2章で作成したユーザ名とパスワードを入力してください。ボックスにチェックを入れると、ユーザ名とパスワードはJOSMに保存され、以降の操作のたびに入力する必要はなくなります。"認証"をクリックしてください。

  ![]({{site.baseurl}}/images/jp_beg_ch6_image06.png)

-  変更内容がサーバにアップロードされるには、少なくとも数十秒かかります。OpenStreetMapの最初の編集はこれで完了となります。なお、続けて編集を行うことも可能です。変更した内容はJOSMを閉じる前に必ずアップロードするよう、注意してください。

変更結果を地図で確認
----------

-  ブラウザを開き、[openstreetmap.org](http://openstreetmap.org)を表示してください。
-  表示されたら、編集を行った地域まで地図を移動させます。
-  あなたが行った変更は地図に反映されているでしょうか？もしまだ表示に反映されていないときは、Ctrl+Rキーを押してウェブページを更新してください。稀にではありますが、地図の更新が正常に行われず、もう一度アップロードが必要になる場合があります。
-  基本的に、地図に変更が反映されるには数分間かかる場合があります。この動作は正常ですので、安心して下さい。また、JOSM画面で追加分をチェックすることで、更新作業が正常に完了したか確認することができます。一般的な動作として、もしJOSMでポイントが正常に表示されている場合、時間がかかることはありますがOpenStreetMapの地図でも表示されます。

まとめ
---

OpenStreetMapへ追加する方法は把握できたでしょうか。OSMの地図は、時間と更新を経るごとに改善されてゆく、ということを忘れないで下さい。地図に手を加えるごとに、加わった改良はデータとして残り、地図はさらに使い勝手の良い、便利な地図へと更新されてゆきます。そして、他の誰かが更新した内容にあなたが手を加えるのと同じように、あなたの行った変更は他の誰かからも手が加えられます。

次の章では、JOSMの機能についてさらに詳しく紹介します。より便利なシェイプの描き方や、新しいツールの使い方、地図を表示している領域を囲む様々なボタンとパネルについて紹介します。