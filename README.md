>**Shape Attack!!**

>**フォルダについて**

/Asset/MyAssetsの中にゲーム開発で使用するスクリプトや音楽入れる  
/MyAssetsの中には  
/Fonts(テキストのフォントをいれる)  
/Musics(この中には/BGMs,/SEsがある)  
/BGMs(ゲームで使用するBGMをいれる)  
/SEs(ゲームで使用する効果音などをいれる)  
/Prefabs(Prefabをいれる)  
/Scenes(各々のシーンやゲームで使用するシーンをいれる)  
/Scripts(スクリプトをいれる)  
/Sprites(画像などをいれる)  
/DownLoadAssets(入れてるだけで使用できるアセットをいれる。例えばDOTWeen等)  
がある。必要に応じて新しいファイルを作成する。 

>**コーディングルール**

・bool型の頭には動詞、及び助動詞をつける

・メソッド名は動詞始まりにする(どんな動きをするメソッドかわかりやすいように)

・クラス名は基本的に名詞で始める

・ローカル変数、引数はキャメルケース、その他は基本的にパスカルケース(参照:https://qiita.com/TakeshiNishioka/items/501979ad126e9707758c)

・変数名は伝わるようになるべく短く書く

・マジックナンバーをなるべく避ける(マジックナンバーとは:何の数字かわからない数字。例えばspeedの設定をするときに直接数字を打ち込むとほかの人が見たときわからないため、このような場合はspeed変数を使うようにする。)

・変数、メソッドは基本的にprivateを使用する。(ほかのスクリプトなどに用いるときだけpublicを用いること)

・Inspectorで変更を加えたい(Unityの編集画面で直接数字を入力する)private変数には[SerializeField]を使う(Inspectorで変更を加える予定のないpublic変数には[System.NonSerialized]をつける)

・コミットメッセージは「追加：譜面の追加」,「変更：位置の変更」などのように最初にしたことを簡潔に書き,コロンのあとにしたことについて詳しく書く

・スクリプト,関数にはsummaryコメントをつけてそれがどういった処理をするのか説明を書く(summaryコメントは「///」と打つと勝手に打てるようになる)

>**ブランチ命名規則**
ブランチの命名は
feature/#(issueの番号)
のようにする

