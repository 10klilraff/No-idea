eraTW4.620proto色々修正＋α

 ERB┬SHOP関連┬BONUS2.ERB
	│		　└UPDATE.ERB
	├イベント関連─情事発覚.ERB
	├ステータス計算関連─COUNTER─COUNTER_SOURCE.ERB
	├ステータス表示関連┬INFO.ERB
	│					└PRINT_STATE2.ERB
	└口上・メッセージ関連┬EVENT_MESSAGE.ERB
						　├EVENT_MESSAGE_COM_セクハラ.ERB
						　└EVENT_MESSAGE_挿入系COM┬EVENT_MESSAGE_その他挿入系.ERB
												　 └EVENT_MESSAGE_対面座位&背面座位.ERB

244スレ>>708の修正(COUNTER_SOURCE.ERB
	カウンターのＡ性交継続時SOURCE追加処理が追記された際に、射精箇所が間違ってたのが原因
	えらい長い間潜在バグとして存在し続けてたっぽい
244スレ>>934の修正(PRINT_STATE2.ERB
	うちでは再現出来なかったけど、おそらくLOCALSを初期化してないのが原因、なのでそこを修正
244スレ>>946の修正＋α(情事発覚.ERB
	最初に発生した(Ver4.542)時に、修正書けようとして出来なかった部分が、やっと理由理解出来たので修正
	非常に単純に言えば、その日最初の顔合わせ時に、依頼状況を確認する方法が変わってTARGETを強制的に置き換えていたから
	あとそれを修正するついでに、おかしなイベントが発生しないよう手を入れて見る
245スレ>>333修正(BONUS2.ERB
	スレ内指摘通りに

＋αその１(UPDATE.ERB
	キャラリセット処理関数が二箇所に存在していたのと、元からある方がゲーム開始時にも使っていて面倒が起きそうだったので、アップデート用追加関数名を変更してみる
＋αその２(INFO.ERB
	睡眠中のイタズラで改行がないので、危険日等の表示がずれ込んでおかしな事になるのを修正
＋αその３(EVENT_MESSAGE.ERB,EVENT_MESSAGE_COM_セクハラ.ERB,EVENT_MESSAGE_その他挿入系.ERB,EVENT_MESSAGE_対面座位&背面座位.ERB
	地の文周りで気になったところに、色々手を入れて見た
	つか、同じような内容の関数が複数存在するってのは、どうにかした方が良いかもしれない


更新が間近と仰っていたので、出さずに保留してた前verのエラー報告の修正と、その他気になった点に手を入れてみた
いい加減、口上関係、書かんとなぁ

そして、とうとうera関連のREADMEが200まで行った
そのほとんどがTWなんだから、飽き性かつ放置癖がある自分としてはよく続いてるなぁと思うことしきり


byさもま
