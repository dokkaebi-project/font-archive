FreeDOS/V 珠洲版 V01L38                                    06/01/02

2006/01/02現在最新の環境と古き良きソフトの組合せで実現したFreeDOS/Vです。
（最近は、さほど熱心にチェックしていないので古いのがあるかもしれません）
GPL若しくはFreeWareで構成しています。ディスケットイメージのみの配布とさせ
て頂き1.44Mメディア用を配布致します。

※：現在構成の組み合わせ上VIMに不具合が出ているので削除しています。
　　代わりにEDLINが入っています…。使い方については、別途記事を起こしま
　　すが差し当たり、当サイトのEDLINパッケージを取得すれば（不完全な）取
　　説が入手できます。

※：なるべく多くの環境で動くようにEMM386.EXEにX=E000-EFFFを定義していま
　　す。E000:0000〜E000:FFFFの間にROMが存在しない場合はこの定義を削除す
　　ることによりUMBメモリを64Kほど増加させることが可能です。
　　（調べる方法については、お問い合わせいただいても解答いたしません）

環境限定：
 IBM AT 100%互換機
 メモリ：4M以上（あくまで目安です/2Mでは起動しなかったとの報告を受けてい
 　　　　　　　　ます。）
 DISPLAY：VGA互換
 FDD：2HD　1基以上
 KEYBOARD：OADG規格 IBM-A01キーボード互換相当品（MicroSoftカスタムでもOK）

内容説明：
 カーネルに2035a、コマンドラインに日本語0.82 PL3J R2を採用。
 FreeDOS Beta9よりも新しい環境でFree DOS/Vをお届け致します。もちろん、
config.sys/autoexec.batをちょちょいといじれば「ライセンスフリーなBIOS書き
換えディスク」が仕上がります。(この記述は、完全に書き換えられる事を保証す
る物ではありません)
 本配布環境はライセンスをすべてクリアしています。

Kernel:V2035a
日本語COMMAND:0.83 PL3J R2 XMS-SWAP
FONTNX/DISPV/CHES <- DOS/V用ドライバ＆ツール
FEP:鳳V0.522P33(べんぜんさん＆石本さんパッチ)、辞書はAkeruさんの版
04GZN16X.FNT:泊何水さんの出水フォント(JIS2004の第一、第二面対応：β5.1)
GURI16X.FNT:ぐりぽん氏特製
GURI19X.FNT:ぐりぽん氏特製
EDLIN:edlin-2.1J2

以下はJIS第四水準化PACKに分けました。
J2KZN16X.FNT:JIS2000対応(PUBLICDOMAIN-FONT:by 伊藤隆幸さん)
JHSLCC16.FNT:SLCCWAC特製フォント
JHSLCC19.FNT:SLCCWAC特製フォント


SLCCWAC特製フォントは、7BIT ASCII部分にはX11のフォントをパッチしてあり、
00〜1Fと80〜FFははずかしながら珠洲デザインです。
そのほかは、FreeDOSのBeta9から頂戴しています。但し、MEM/FDXMS/FDISK/EMM386
は更新してあります。

オリジナルファイル：
日本語COMMAND ： 本ページで公開している日本語メッセージシェルです。

日本語入力の説明：
日本語は、超多段方式で入力します。
起動後、ALT+「半角/全角」キーで鳳が立ち上がります。（画面右下を確認）
その後、読みをローマ字で入れてスペースを入れれば漢字に変換できます。対応
する漢字が配置されているキーを押下してください。
また、ひらがなを入れる場合、ローマ字入力後「ENTER」を押下してください。
片仮名を入れる場合は、ローマ字入力後「カタカナひらがな」を押下してくださ
い。
詳細の説明は、べんぜんエリアを参照してください。
http://www.vector.co.jp/authors/VA000964/
また、FreeDOS/V版の詳細なキーアサインは以下にまとめてあります。
http://homepage1.nifty.com/bible/dos/freedosv.txt
また、本パッケージにかかる質問は、珠洲にお願いします（とはいえ、使いこな
している訳じゃないので、鳳に関する限りお答えしかねる場合があります）
一応、入力アシストページを解説しましたが、若干の不備がございます。
http://homepage1.nifty.com/bible/dos/ohtori/ohtori.html

DOS/V用ドライバ＆ツール説明
FONTNX.EXE  : (株)軟式様の配布されている$FONTX互換ドライバです。
DISPVB.EXE  : Takashi Oyama様の配布されている$DISPV互換ドライバです。
VESAPAT.EXE : Takashi Oyama様の配布されている日本語環境整備ドライバです。
CHES.COM    : Natrium様の配布されているCHEVコマンド互換ツールです。
JIS_A01.COM : binnHood様のA01キーボードドライバです。
PANSI.SYS   : 伊藤省三様の配布されているANSI.SYS互換ドライバです。

DISPV(同梱しているDISPVBとVESAPAT)について：
　同梱しているバイナリ単体での配布は厳禁です。
　DISPVについては次のページを参照してください。
　　　http://www.hmsoft.co.jp/lepton/software/dosv/dispv.htm
　また、オリジナルアーカイブは次のものです。
　　　http://www.hmsoft.co.jp/lepton/software/dosv/disp160a.lzh

PANSI.SYSについて：
　同梱しているバイナリ単体での配布は厳禁です。
　本システムにはご好意によって同梱させていただいております。
　PANSI.SYSについてのライセンスについてはDOS/LICENCE.DOCを参照ください。
　PANSIについては次のページを参照してください。
　　　http://hp.vector.co.jp/authors/VA003655/
　また、オリジナルアーカイブは次のものです。
　　　　pansi103.lzh

注意点：
・昔に比べ大分安定しましたが一部挙動不審です。（突然固まるかもしれません）
・J3100シリーズ(J3100SS001〜V486 FV475他)でも動作するようになりました。

動作確認環境：（多くなってきたので、そのうち分離する可能性があります。）
V01L36
 IBM製Type 5523-JBW (ThinkPad 330)
 CPU:486SLC2 (50Mhz)
 メモリ:8M

V01L29(立ち上げのみ確認)
 東芝製DynaBook V486 FV475 510TWモデル
 CPU：80486DX4 (75Mhz)
 メモリ：8M + 32M(ADTECH)

V01L15(FDが破損のため確認停止)
 東芝製DynaBook TECRA 510CT/2.1 Windows95モデル
 CPU：80586（133Mhz）
 メモリ：48M
 
V01L20RC(破棄のため確認停止)
 東芝製DynaBook Satellite 110CS
 CPU：80586 (100Mhz)
 メモリ：8M + 8M

V01L00(キーボードがJ3100ベースのため確認停止)
 東芝製DynaBook EZ486
 CPU：80486SX (25Mhz)
 メモリ：2M + 8M(TOSHIBA J31MESL2)

V01L28(売り払ったため確認停止)
 富士通製FMV-5200 NA8/X
 CPU：80686 (200Mhz)
 メモリ：32M + 64M + 64M

V01L29(故障のため確認停止)
 IBM製Type 2644-6AJ (ThinkPad 570E)
 CPU:Pentium!!! (500Mhz)
 メモリ:64M + 128M

V01L09
 DOSEmu 1.0.1(VineLinux上)
  xdosでは画面表示に難あり

V01L20B2
 自作PC(blupe)
 CPU：Pentium3 (600Mhz)
 メモリ：256M

V01L20(世代交代のため確認停止)
 自作PC(ooph)
 CPU：K6-2 (266Mhz)
 メモリ：128M

V01L37(解体のため確認停止)
 自作PC(ooph 2代目)
 CPU：Cyrix C3(733MHz)
 メモリ：128M

V01L24(引退のため確認停止)
 自作PC(seelie)
 CPU：80586 (200Mhz)
 メモリ：32M
※：HDDの導入も確認（852M/V01L20B2）

V01L25(Unistallのため確認停止)
 仮想マシン（VirtualPC 4）
 CPU：Pentium3相当
 メモリ：32M
※：HDDの導入も確認（2048M）

V01L21
 仮想マシン（Bochs 2.0.2. 鯖さん改造もの）
 CPU：不明
 メモリ：16M
※：HDDの導入も確認（10M）

V01L33(退社のため確認停止)
 SonyVAIO PCG-715
 CPU:80586 (166MHz)
 メモリ96M

V01L38
 東芝製DynaBook Satellite 110CT
 CPU：80586 (100Mhz)
 メモリ：8M + 32M

以下：泊何水さん（JDUG）のご報告
V01L20B
 Compaq Contura Aero 4/25
 CPU：80486SX(25MHz)
 メモリ：4M(?/MAX12M)

V01L20B
 IBM PS/55 Note N23SX
 CPU：80386SX(16MHz)
 メモリ：2M(?/MAX16M)

V01L20B
 富士通FMV-NoteBook 450N/S1
 CPU：80486DX2(50MHz)
 メモリ：8M(?/MAX36M)
※：HDDの導入も確認

V01L20B
 富士通FMV-BIBLO 5100NL/Y
 CPU：80586(100MHz)
 メモリ：16M(?/MAX32M)

V01L20B
 富士通FMV-DESKPOWER C
 CPU：PentiumODP-85MHz
 メモリ：32M

動作確認ソフト：
jis_a01：A01用キーボードドライバ
JVIM V3：VI互換日本語対応エディッタ(鳳との組み合わせで不具合アリ)
FD:ファイラー（出井氏）
SE3：エディッタ（京都コンピューター学院：難あり）
日本語FEP鳳：日本語フロントエンドプロセッサ（べんぜん氏）
日本語FEP刀：日本語フロントエンドプロセッサ（（株）アイフォー：挙動不審）
日本語FEP ATOK8：日本語フロントエンドプロセッサ
                                    （（株）ジャストシステム：EMSが必須）
EMM386.EXE：プロテクトモードメモリマネージャ
                       （マイクロソフト（株）：FDXXMSと競合する場合あり）
DOSMINIX（英語モード）：教育用UNIXもどき（AST,Kees J.Bot）(V01L19以前）

最後に：
 FreeDOS(JP)のぐりぽんさん情報提供をありがとうございました。
 また、組み込みご許可をくださいました、軟式の「たかぴゅう」さん、@nifty
内FTOSHIBAのNatriumさん、leptonさん、べんぜんさん、binnHoodさん、伊藤省三
さんありがとうございます。
 FreeCOMに関連して、ぐりぽんさんの多くの助力と、Silphireさんの貴重なご指
摘を頂いております。重ねてありがとうございました。
 DR-DOS UGの泊何水さんの出水フォントを借用させていただいております。すば
らしいデータの公開に多謝。

問い合わせ先：
 本配布PKGはGPLとフリーウェアの混合体です。各ソフトの配布条件に従って、各
ソフトを扱って下さい。また、本配布PKGの組み合わせに関しても、配布者である
珠洲は動作の保証を行いません。何があっても、関知しませんのでシビアな環境
（特に人命や公共サービスに影響のある装置及び準ずるもの）には使用しないで
下さい。
　なお、本PKGに同梱しているフリーウェアに関しては本PKGから抜き出してのバ
イナリ単体における再配布を禁止します。各オリジナルPKGから作者様の許可を
取得してから行って下さい。

 最新版の配布は以下の箇所で行っています。
  FreeDOS/Vページ
　http://homepage1.nifty.com/bible/fdos/

 なお、特にご質問、指摘などある場合、水城珠洲へご連絡下さると幸いです。
 ただし、すべての質問に回答、指摘に対応できる訳じゃありませんので、あらか
じめご了承いただき、過大な期待をしていただかないように切にお願いいたしま
す。
　水城珠洲：minashirojp@yahoo.co.jp
