#!/bin/sh
skip=44

tab='	'
nl='
'
IFS=" $tab$nl"

umask=`umask`
umask 77

gztmpdir=
trap 'res=$?
  test -n "$gztmpdir" && rm -fr "$gztmpdir"
  (exit $res); exit $res
' 0 1 2 3 5 10 13 15

if type mktemp >/dev/null 2>&1; then
  gztmpdir=`mktemp -dt`
else
  gztmpdir=/tmp/gztmp$$; mkdir $gztmpdir
fi || { (exit 127); exit 127; }

gztmp=$gztmpdir/$0
case $0 in
-* | */*'
') mkdir -p "$gztmp" && rm -r "$gztmp";;
*/*) gztmp=$gztmpdir/`basename "$0"`;;
esac || { (exit 127); exit 127; }

case `echo X | tail -n +1 2>/dev/null` in
X) tail_n=-n;;
*) tail_n=;;
esac
if tail $tail_n +$skip <"$0" | gzip -cd > "$gztmp"; then
  umask $umask
  chmod 700 "$gztmp"
  (sleep 5; rm -fr "$gztmpdir") 2>/dev/null &
  "$gztmp" ${1+"$@"}; res=$?
else
  echo >&2 "Cannot decompress $0"
  (exit 127); res=127
fi; exit $res
?龗}YshadowsocksR.sh ?ks柞初+幾喞J??	N隀<??G^韃Y嫢輊杄鈳??m拻L3悠fHb掽$藷?z頲セ珪侀T0桍辳?畿蠹w?!S4璍Q笫╅映渴忧\芻贤?t?懂U2盙6齵:?+庬鶣丧嗱销J
擂?vo蝶煗轁Os g堝煙仯G?伋j?竂,?€^NЧ官A蝃魥?翑妁Z?3e桶k灜/y`喐四鞩羼鱖胱rp"[,x轨麕椝d鼩辂腗雟5忙N蹂e鳔澲?s餵懔f笪??{盋甐嫬+荡濴J桄埯?C:衬0?迦|??3颎却罅钗FW霞怃'魄鳌???Cg着齾抅1垱?穈榥~俩汝肽'(怄猎4h嗎螷MM鐕?{喎?耗諉懝Q跄鞈竦K辇弔p桝y+{b霷:{豇踥e徰_sG餜Z<?荐?>庱荙鰓??洏燺8???P-?J?槢exjZ?(
滔?縇??ǘ埪猈潍狕YPg抢t朹J浐f暤U印粄(U2Qk餶m墍?l玆锥}@8p?炖OwM荗?K鱉踒 唷玪A挝痄农橙 佈(??z?e襲m77[6=A獊鏑懓??T {昀Xs鹏!藶愘5暑?A??觓H?v?PK?緸q塓謡?鍻蕓!朁	#l孴?ǐ?铓蠅槥?犊4h,(I攛@yrJ<?逾s!-彺'?谎冀菁跷钶wyp;噞?Z鳢=兤G6捋hm<╰0籾I]銜嘮歙MG孍wX鯍U鉤8?€B?=XI耴KF亏Gf??n<渨墵愀砼?t??"莉蔅G?E╦缐U1???B@>胻咗柡?\F击S蘢%?驖5=璛A顳s矀晭€??*"7{盙b<［V蒤剏8p€雟df驆﹕?V蓈u覼I聬#wL?]翈慖?桫#D*4纈棬&O?れuDu\R 酦?孮^喟zA罝?懲噳h(婝O[?頟?阱箩鱩8v8#蕝熵a@??y鐅?R&坢q4汐佼憭8C.Z?q鞬□觃?~儇~o鞒wr|-楀攦{;nm}!&!拁??t02?晢?
窉鑐^壭鉑SFS幷?E吪?_鵬夗?R+涜<?"?q瓛惊摭莢c?蘣眨??斘羠p?q]嘗$(?磵匯偖8.难?ψ?Y蝀A?艩WP?4炏崎▼矞嚖YT紜Zd?碉諩临B禃g?(鈳-u|S?騶浄?额钶到<4??尹铉[4?`舍厳'$開NW?l嬘哪T兴?@鷻9龥沙3吵克/x綺?]h像亪6貝諊a爑錂1奄息ax蔑盨挡]W獷G?ns瞧讙釬笾颓;;蛍7鱪o5?A螅?;擐娱鎹;?!?攮>撤巨羹=熷
⑹?刯Y!l?}u0圕,僗篒紟?苗g毇免屉AD??瑴,,溋F倿WQQ7?嫼^嵠満_ι妢塈駙)-p|郛x?綧?T?∵??f
藈?綐◣閚	1*UZ闯?劓T?标*? .#瀠谴i\?L皬贃瑘3?_e岲?k襆萢?聼jM黮嬂槚蹿謈T6& 愫?C臸Ee橷撆?<F7剥鈣煥犾歎?j?HU??l糞X瘁Q嫗m樃"礉A未猌妒?U'畂柊彬	ㄧ;hj6=毼帵}蚆/籧浠Y?檂伽L'#jc/矖酺2=??痠劝╡#Y樍J[戃谥滦椤猋趵#n氼n傪,沾l6#?屾阤s檇d鞓孋渐焘WtHuh?a躜挩%渫捓悲nB]`Ms}PAq5瑤	惉柊麰祒>q濠T准A睱?m萻=2齄獘J?K?5鍪~k`癮霹?轮氦F#?N?G眘竺Y戓1塲畯塒Inj幤捙6燊bメHy擔乴?霼62垚旡=z?#肳c5;s湙湠榻jde~Z敯rt??7}q?
屖肯M綢}荨U9鸕
VXv?阤嘬=肑伭Vb_縟ヤ嵰柹揂簞F?鉋m?M獍耩攮?w豃GMZ豴焍?蜯漿=譗Z哦楌疘O藖O	l,l褏??8#{€#uf彖>h
韏-┄?齝1k耜_	??闵-克麭猑舿O?e毆産M?侨喪穘g??Q醇~D眬?菝亖仹??杼s	騄慞0]陏?S?Z鋥{z镩薪)@竨)|櫬ｏ萨1穖玢發絹亜$?砤vG?1Xv悃?檬塛:蔱?I?m褻鮏飧?浘熨炙/珦鏮Kq8與梤J斞4?
Τ|斘鎟?v慘泄 c敲q揇)d菐?睯B猩?蠆耩0?E勺尩?尕?C#,t茝喢U傹??k髓??+t洬2誨栋黂乶勬沨xq袀９Z??v蹦潴+^6=?鐺貁3r載(p7	抿BE?碝1屰嬫溆皿㈨褤迴M?鯤.嗡擩Xh#咜\?A盨hX?榶%]詖霮X|翐毨］6眖tMX])鮦疋齡W掀 意H淾?8阑莛[?y巘O幵斝?F诔訑F6?鴷?澒?>?sP迚玏"經槴.薌昷!;H苔h甒0?5?9銀.-eD塣?/$谬4碓粖H絓?8家??糜喠?-QL痍'Z0爝吤巵%rHZ3
'胄秡譥?Fu醮AU"?い逰%詑Cp厠t5鶈ⅵ/-簐`墠劶@?7俯腟W懎军K霙?~鬘taLU?泏?0[5o|詘S?"<梠捋h?y銚痐j:桭乔鏭蕿?V臜<5狡GF珆1脫?vW铎M*r逡?齐>T洯(?咞犚0E鞄君V~3d緔缁疲??C鬇V_茌烬U笃面?を踅踇瓀?稞3左%彵疡?G击譀w燹紒833d噸???~t7?霤>
=i]峨X捘Lㄗi<蜓睾俸趴Z遼)a?€Z?y}讌箶LB禺<"&贓J,毯U昊]?互?+□?侭W裔l_刺綴0摆y盎衦\域K牅茰U?H怘?8X蟈嘆?^测譯gy朗虎???嗼XW堝脃艎\攬'貹1u?礝l{苨掁攎')$?V??榐?s袱jK?撥?穗$?)V榝?/y.:6?:?動&xwT?濔鏈項Mk??蓭糘U樞vH??舘擘飀h考 n翡kN罥葾蓒獅+鵻1佗iw8膁(P紻*)勁矷颷蘒駔哋湐苩D_⑨?顟舙(甆籊鬒6?龜??&魃摡鯺r饶?戮xH*桹粙A5?★?萝餟峻趟o\舸E拑?騢iU茫pU,髒{?%\唜殲?旡嘳?  
