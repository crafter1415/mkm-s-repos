# Enderdragon_pack

**制作協力：Ponpon**

エンドラを強くしたいのと、1.13以降のコマンドを勉強したいのと、  
とにかく何かぶっ飛ばしたいのが混ざってできた本当に謎のデータパック。  
対応ver 1.14.4

## 導入方法

ワールドのフォルダを開いて、datapacksフォルダにzipファイルを時速130kmくらいの勢いでぶち込んでください。  
ピンポンダッシュするときの小学生と同じくらいの勢いでも大丈夫です。  
間違ってもcabファイルのまま入れるなよ？~~そのまま入れたら多分ピンポンダッシュされるぞ？~~  
(そのまま投げても動かないだけです。多分。)

一応、クライアントでやったときは/reloadが必須だったのでそこだけ。

## ワールドフォルダをリセットする場合は

これを実行しないと不具合とか起きるはず。
>/function dragonfight:reset

- - - - - - - - - - - - - - - - - - - - - - - 
[](気合の連打)

#### 以下、ネタバレも含む。
未プレイで、初見プレイを楽しみたい方は、ここから下を見ることをお勧めしません。

- - - - - - - - - - - - - - - - - - - - - - - 
[](迫真の連打)

## 追加仕様

readmeと違って、詳細付き。
>エンドにトラップが追加される  
 - 見た目での判別はほぼ不可能。
 - 踏むとデバフが付くか、バフが消えるか、爆発するか、落雷する。  
   但し確率は一定ではない。爆発が1/5くらい、バフ消去は1/60くらい。~~詳細はソース見て~~
 - 後、踏むと花火のエフェクトが出る。
 - 数は大体中心から半径100mに500個程度。
 - トラップはブロックを壊せば壊れる。
>エンドクリスタルが10分で復活  
 - 復活時間は人数に反比例する。  
>エンドクリスタルが1~2分毎にモンスターを召喚する  
 - ほとんどの敵を召喚するが、一部敵はバランス崩壊とかうるささとかを考慮して湧かないようにしてある。  
   これの確率はどれも一定。コマンドでしか出せない敵も出てくる。
>エンダードラゴンが1分毎(最小20秒毎)にTNTを投下する  
 - 最初は1分毎だが、最大回復した後は40秒毎、HPが1/4になってからは20秒毎になる。
 - システムの都合上、大量投下の間隔は一定。~~変えたかった~~
>エンダードラゴンが1分毎(最小40秒毎？不明)に大量の矢を投下する  
 - 殺意でもあるんかってぐらいの矢が降り注ぐ。  
   当たると盲目と空腹と5ダメージを食らうので意地でも避けよう。
>エンダードラゴンが1分毎(最小20秒毎)に火の玉を発射する  
 - 自機狙い。マルチだとランダムに狙う。
>エンダードラゴンが近づくと毒を付与するようになる  
 - ~~着地時は矢が当たらない仕様のせいで厄介。~~  
   ~~覚悟して攻撃するか矢でちまちま削るしかない。~~  
   **アップデートで着地しなくなったため遠距離攻撃かタックル狙いするしかない。**  
>エンダードラゴンの最大体力が500になる  
 - 全快があるから、実質750。
 - これに関しては唯々長引かせたかった。
>エンダードラゴンの体力が半分以下になったとき全快する (一度のみ)  
 - ゲームとかでよくあるやつ。  
>エンダードラゴンがエンドゲートに着地しなくなる  
 - 文字通り。疲れないんですかね？  
>アイテム化したエンドストーンが10秒で消える  
 - 負荷軽減のため。これがないと120FPSが20FPSくらいまで落ちます
 
## 使用したタグ・スコア・進捗
これもりどーみーの奴と同じ。競合したら見るといいかも
> **使用タグ**：  
>   dftrap, dfmakeTrap, dftick, dfHealed, dfHealing, dfHardend, dfSpawner,  
>   dfActive, dfCrystal, dfCrSeted, dfArrow, dfnotrandomized, dfFireball, dfNotFaced  
> **使用スコアとシステム変数**：  
>   df_EndFlag - #Flag  
>   df_NUM - #1, #12, #67, #100, #1000, #Players, #Time  
>   df_id  
>   df_tick  
> **使用した進捗**：  
>   dragonfight:rebegin  
>   dragonfight:killed  
>   dragonfight:root  

## 最後に
不具合やご感想はtwitterかdiscordのDMまでお願いします。  
 **Twitter @crafter1415  
 Discord @mkm75#1764**  
多分gitでコメントor報告しても見るのは本当に稀なので、期待せずどうぞ。

制作の協力をしてくれた**Ponpon**様にこの場を借りて感謝申し上げます。ありがとう！
