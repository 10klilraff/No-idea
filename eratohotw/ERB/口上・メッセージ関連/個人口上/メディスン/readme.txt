eraTheWorld　メディスン・メランコリー口上 ver0.01
作者：すし（小町、はたて口上作者）
執筆開始日03/08/08
リリース日03/10/17
最終更新日03/10/17

三作目です。前二作にはない機能にチャレンジしてみました
技術のない人間が慣れないことするものじゃないですね
eraTW4.793〜4.811環境下で執筆したメディスン口上です
申し訳ないですがバグ発生時は報告お願いします

■謝辞
　=====================================================================================================================
　本口上を作成するにあたり主に参考にさせていただいた口上・バリアント等
　・諏訪子口上内「祟りカウンターシステム」
　・「eratohoЯeverse」内「ぱにめーしょん」
　・eratohoスレ内で助言をくださった皆様
　・最後に、本口上を使用してプレイしてくださった皆様に感謝を。ありがとうございます

■キャラコンセプト
　=====================================================================================================================
・原作通り人間嫌い。問答無用で攻撃したりはしないがあなたのことを警戒しており、心を許す気はない
・邪魔になったら毒で殺せばいいや、と子供らしい短絡的な考えを持っている
・その一方で敵である人間を知ろうと、あなたから人間の知識を得ようとする
・序盤はあなたに対して興味がない。興味があるのは人間についてのみ
・好感度が高まってくると人間→あなたに興味がシフトしていく
・毒人形のため、接触すると体力を削られていく。諏訪子様の「祟りカウンターシステム」が常時発動しているような感じ
・接触が濃密であればあるほどダメージが大きい
・あなたへの愛が深まるにつれて毒を制御する能力が高まっていく
・人形のため、基本性器にあたるものはついていない
・うふふ時は基本あえがない。むしろマグロといえなくもない。ただしボディ自体は感じているのか濡れる
・愛がないときは人間の行動として観察し、愛が深まっているときはあなたが気持ちよくなる様を優しく見守ってくれる
・好感度が上がる（陥落素質を得る）と、ボディの質感が変化
・無知を失うと、ウフフのときＳっ気が強くなります
・恋慕だと、罵倒（？）しながらも全肯定してくれる感じです。こういうの、なんてジャンルなんですかね…メスガキママ？
・「幼稚」は虚無りました
・女あなた、ふたなりあなたは想定していません
・「我が儘なお姫様」をイメージしながら書きました
・我が儘といっても、小さな我が儘で相手の反応を楽しんでるようなイメージです
・小さな子が親に抱っこをおねだりするとか、お風呂上りにパジャマに着替えないで裸で部屋を走り回ってる、そんな感じ
・口調は大人びています。もっと幼稚な方がメディスンらしいのかもしれないですが、原作も幼稚とは違う感じなのでまあ…
・奉仕系は一通り書いてますが、性交系は現状正常位、対面座位のみです
■メディスンの毒について
　=====================================================================================================================
　まずはじめに、参考にさせていただいた諏訪子口上作者様に感謝を

・先に述べましたが、諏訪子様の「祟りカウンターシステム」とほぼ同じです
・まだ生まれて間もなく、毒も完全に制御しきれていないという公式設定に準じています
・祟りとの大きな違いは、時姦、睡姦時だけでなく、通常の「抱き付く」のようなセクハラ行為でもガリガリ体力を削られることです
・濃密な行為（特に押し倒し中のコマンド）になればなるほど減少値が大きいです
・キスとかかなりヤバいことになるので気を付けてください
・陥落素質および愛情経験などプラスのステータスが増えれば増えるほど、減少値が緩やかになっていきます
・あなたを愛すれば愛するほど毒が制御できるようになる、というイメージです
・何のパラメータが毒ダメージに影響するかは「ユーザー関数」に書かれています

■メディスンのウフフ仕様について
　=====================================================================================================================
・メディスンは人形の身体なので、初期状態ではクリトリス、アナル、ヴァギナが存在しません（という口上内設定）
・eratenの機械の乙女にさらに制限を加えた状態です
・加えて、ほぼすべての行為に対して感じません。時止め、睡眠中も同じです
・陥落前はもちろん、陥落後も同様です
・メディスンとディープな性行為を行う、絶頂させるためにはイベントをこなす必要があります
・イベントを進めるためのヒントはプロフィル画面に表示されます
・アナルがないのに食べたものはどうしているんだ？という問題は、毒で跡形もなく消化しているという設定で
・コミカライズ（茨歌仙？）では綿菓子を食べている描写があったと思います
・ウフフ可イベントは書いてて自分でもビックリのトンデモ理論のバーゲンセールです
　
■自分用メモ
　=====================================================================================================================
・メディスンは[幼稚]で[初潮]を迎えていないので、性器が実装されてもすぐには孕まない
・メディスンは[人形]持ちなので、妊娠確率はひじょうに低い（[人形孕ませ]で軽減）
・起床時間は6時。就寝時間は21時
	女性器不在（性別のbit0が0）もしくは[幼児／幼児退行][幼稚]で[初潮]未取得であれば周期を設定しない
	IF ((TALENT:LOCAL:150 || TALENT:LOCAL:151) && !TALENT:LOCAL:初潮) || !GETBIT(TALENT:LOCAL:性別,0)
		CFLAG:LOCAL:900 = 0
・無知消失の条件
・TARGETが無知かつＨな本読みかつMASTERがTARGETより教養が高くTARGETの教養が2以上かつ五分の一だと無知消失
	SIF !RAND:5 && TALENT:TARGET:無知 && TFLAG:193 >= 6 && TFLAG:193 <= 8 && ABL:MASTER:教養 > ABL:教養 && ABL:教養 >= 2	TFLAG:194 = 2
	EVENTMESSAGE_COM500.ERBの462行目以降参照
・自慰経験が（調教自慰経験より多く）一定以上だと保護者に報告して無知消失
	AFTERTRA.ERBの510行目以降参照

■更新履歴
2021/10/17（ver.0.02）
コマンド関連の実行判定に誤りがあったのを修正

2021/10/17（ver.0.01）
とりあえずリリース



















■ネタバレ
　=====================================================================================================================
メディスン改造イベント発生条件
・恋慕＆恋人取得、または恋慕もしくは恋人を取得した状態で好感度1万以上、信頼度5000以上、愛情経験1000以上
・さらに、以下の４人と面識があり、信頼度が一定値以上に達しているとイベントが発生する
　青娥…信頼度250以上
　アリス…信頼度500以上
　永琳…信頼度750以上
　紫…信頼度1000以上
　誰を選んでも性交が解放されるが、キャラによってメリット、デメリットが発生する
