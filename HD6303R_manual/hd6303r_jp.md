# HD6303R, HD63A03R, HD63B03R <br>CMOS MPU (Micro Processing Unit) 
HD6303Rは、HD6301V1と完全互換の命令セットを持つ8ビットCMOSマイクロプロセッシングユニットです。128バイトRAM、シリアル通信インタフェース(SCI)、パラレルI/Oポート、マルチファンクションタイマを内蔵しています。HMCS6800とバス互換性があり、最大65kバイトまで拡張できます。HMCS6800ファミリ同様、I/OレベルはTTL互換で50V単一電源です。HD6303RはCMOS MPUであるため、消費電力が非常に小さくなっています。また、低消費電力モードとしてスリープモードとスタンバイモードを備えています。このため、柔軟な低消費電力アプリケーションに対応できます。

<img width=280, src="img/001-6303-package1.png">
<img width=280, src="img/002-6303-package2.png">

## FEATURES 

* HD6800、HD6801、HD6802と上位互換のオブジェクトコード 
* 多重化バス(D0/A0-D7/A7, A8-A15)、非多重化バス(D0-D7, A0-A15) 
* HD6301V1と互換性のある豊富なオンチップ機能: 128バイトRAM、13パラレルI/Oライン、16ビットタイマ、シリアル通信インタフェース(SCI) 
* 低消費電力モード: スリープモード、スタンバイモード 
* 最小命令実行時間: 1us (f=1MHz), 0.67μs (f=1.5MHz), 0.5μs (f=2.0MHz)
* ビット操作、ビットテスト命令 
* エラー検出機能: アドレストラップ、オペコードトラップ 
* 最大65kバイトのアドレス空間 
* 広い動作範囲  
  Vcc 3 to 6V (f = 0.1 ～ 0.5 MHz)  
  f = 0.1 to 2.0 MHz (Vcc  5V ± 10%) 

## TYPE OF PRODUCTS

|Type No.|Bus Timing|
|--|--|
|HD6303R|1.0MHz
|HD63A03R|1.5MHz
|HD63B03R|2.0MHz

<div style="page-break-before:always"></div>

## PROGRAM DEVELOPMENT SUPPORT TOOLS

* IBM PC および互換機用のクロスアセンブラおよび C コンパイラソフトウェア
* IBM PCおよび互換機用インサーキットエミュレーター

##  PIN ARRANGEMENT 

HD6303RP, HD63A03RP, HD63B03RP 

<img width=350, src="img/003-pin-arrangement-DIP40.png">

<div style="page-break-before:always"></div>

HD6303RF, HD63A03RF, HD63B03RF 

<img width=400, src="img/004-pin-arrange-QFP54.png">

<div style="page-break-before:always"></div>

HD6303RCG, HD63A03RCG, 

<img width=400, src="img/005-pin-arrange-XXX40.png">

<div style="page-break-before:always"></div>

HD6303RCP, HD63A03RCP, HD63B03RCP 

<img width=500, src="img/006-pin-arrange-PLCC52.png">

<div style="page-break-before:always"></div>

HD6303RL, HD63A03RL, HD63B03RL

<img width=500, src="img/007-pin-arrange-PLCC44.png">

<div style="page-break-before:always"></div>

## BLOCK DIAGRAM 

<img width=477, src="img/008-block-diagram.png">

###  ABSOLUTE MAXIMUM RATINGS 

<img width=715, src="img/009-table-absolute-maximum-rating.png">

(注)本製品は入力端子に高電圧高電界保護回路を内蔵しています、 

但し、これらの高入力インピーダンス保護回路には最大定格以上の過電圧を印加しないようご注意下さい。正常な動作を保証するために、Vin, Vout:  Vss <= (Vout または Vin) <= Vcc.

##  ELECTRICAL CHARACTERISTICS 

### DC CHARACTERISTICS (Vcc = 5.0V±10%, Vss = 0V, Ta = 0~+70°C, unless otherwise noted.) 

<img width=716, src ="img/010-table-dc-characteristics.png">

\* VIH min = Vcc-1.0V, V11 max = 0.8V 

\*\* 動作時またはスリープ時の許容損失電流は動作周波数に比例します。従って、f = x MHz動作時の許容損失電流のTyp.値またはMax.値は、以下の式に従って決定されます;
```
typ. value (f = x MHz) = typ. value (f = 1MHz) x x
max. value (f = x MHz) = max. value (f = 1MHz) x x 
(both the sleeping and operating) 
```

<div style="page-break-before:always"></div>

###  AC CHARACTERISTICS (Vcc = 5.0V±10%, Vss = 0V,<br> Ta = 0~+70°C, unless otherwise noted.) 

### BUS TIMING 

<img width=738, src="img/011-table-ac-characteristics1.png">

\* これらのタイミングはtcycにほぼ比例して変化する。この特性の数値は、tcycが最小の場合(＝最高速動作時)の数値である。

<div style="page-break-before:always"></div>

### PERIPHERAL PORT TIMING 

<img width=699, src="img/012-table-ac-chacteristics2.png">

### TIMER, SCI TIMING 

<img width=694, src="img/013-table-sci-timing.png">

### MODE PROGRAMMING 

<img width=692, src="img/014-table-mode-programming.png">

<div style="page-break-before:always"></div>

Figure 1 Multiplexed Bus Timing 

<img width=689, src="img/015-multiplexed-bus-timing.png">

<div style="page-break-before:always"></div>

Figure 2 Non-Multiplexed Bus Timing 

<img width=615, src="img/016-non-multiplexed-bus-timing.png">

Figure 3 Port Data Set-up and Hold Times 

<img width=355, src="img/017-figure3-port-data-setup-and-hold-times.png">

<div style="page-break-before:always"></div>

Figure 4 Port Data Delay Times (MPU Write) 

<img width=349, src="img/018-figure4-port-data-delay-times.png">

Figure 5 Timer Output Timing 

<img width=345, src="img/019-figure5-timer-output-timing.png">

Figure 6 Mode Programming Timing 

<img width=390, src="img/020-figure6-mode-programming-timing.png">

Figure 7 Bus Timing Test Loads (TTL Load) 

<img width=716, src="img/021-figure7-bus-timing-test-loads.png">

Figure 8 Interrupt Sequence 

<img width=810, src="img/022-figure8-interrupt-sequence.png">

<div style="page-break-before:always"></div>

Figure9 Reset Timing

<img width=803, src="img/023-figure9-reset-timing.png">

## FUNCTIONAL PIN DESCRIPTION 

### Vcc. Vss 

この 2 つのピンは電源と GND に使用されます。推奨電源電圧は5V±10％で、低速動作(100～500kHz)には3～6Vを使用できます。

### XTAL, EXTAL 

この2ピンに並列共振基本波ATカットの水晶振動子を接続します。例えば、システムクロック1MHzを得るためには、内部の4分周回路を通すので、共振基本波4MHzの水晶振動子を使用する。図10に水晶振動子の接続の例を示します。EXTALはデューティ45%～55%駆動の外部クロック入力を受け付けます。外部クロック入力の場合、XTAL端子はオープンとしてください。水晶振動子とコンデンサは可能な限りピンの近くに実装すること。

Figure 10. Crystal Interface

<img width=428, src="img/024-figure10-crystal-interface.png">

### Standby (STBY) 
MPU をスタンバイ状態にする端子である。"L"レベルになると発振が停止し、内部クロックは Vss または Vcc に固定され、MPU はリセットされる。スタンバイ時に RAM の情報を保持するためには、RAM イネーブルビット(RAME)に "0"を書き込む。RAMEは、アドレス\$0014のRAMコントロールレジスタのビット6です。これにより、RAMは無効となり、RAMの内容は保証されます。スタンバイモードの詳細については、スタンバイのセクションを参照してください。

### Reset (RES) 
MPU のリセットに使用する。電源立ち上げ時、RES は 20ms 以上 "Low"を保持しなければならない。クロックジェネレータが安定するまでは、クロックがないと MPU をリセットできないため、内部状態や I/O ポートの状態は不確定であることに注意する必要がある。システム動作中に MPU をリセットするには、最低 3 システムクロックサイクル "Low"を保持する必要がある。3サイクル目以降、全てのアドレスバスはハイインピーダンスとなり、RESが "Low"の間継続する。RESが "High"になるとCPUは以下の動作を行う。

1. I/Oポート2の2,1,0ビットがプログラム制御レジスタのPC2,PC1,PCOビットにラッチされる。
2. 2つの開始アドレス、\$FFFE、\$FFFFの内容がプログラムカウンタに書き込まれ、そこからプログラムが開始される(表1を参照)。
3. 割り込みマスクビットが設定される。CPUにマスク可能な割り込みIRQとIRQ2を認識させるには、それらを使用する前にこのビットをクリアする必要があります。

### Enable (E) 
システムクロックを供給する出力端子。出力は単相、TTL 互換、水晶発振周波数の 1/4 のクロックです。2つのLS TTL負荷と40pF容量を駆動します。

### Non Maskable Interrupt (NMI) 
このピンの入力信号の立ち下がりエッジが認識されると、NMIシーケンスが開始される。NMI信号が検出されても、現在の命令は継続して完了します。コンディションコードレジスタの割り込みマスクビットはNMI検出には影響しません。NMI割り込みに応答して、プログラムカウンタ、インデックスレジスタ、アキュムレータ、およびコンディションコードレジスタの情報がスタックに格納されます。このシーケンスが完了すると、プログラムカウンタに内容をロードするために\$FFFCとSFFFDのベクトルアドレスが生成されます。その後、CPUはマスク不可能な割り込みサービスルーチンに分岐します。

###  Interrupt Request (IRQ1) 

このレベルセンシティブ入力は、マスク可能な割り込みシーケンスを要求する。IRQが "Low"になると、CPUは実行中の命令が完了するまで待機する。コンディションコードレジスタの割り込みマスクビットが設定されていなければ、CPUは割り込みシーケンスを開始し、そうでなければ割り込み要求は無視されます。

割り込みシーケンスが開始されると、プログラムカウンタ、インデックスレジスタ、アキュムレータ、コンディションコードレジスタの情報がスタックに格納される。その後、CPUは割り込みマスクビットをセットし、それ以上マスク可能な割り込みが応答できないようにします。

Table 1 Interrupt Vectoring memory map 

<img width=355, src="img/025-table1-interrupt-vectoring-memory-map.png">

サイクルの終了時に、CPUはメモリアドレスの\$FFF8と\$FFF9を指す16ビットのベクタアドレスを生成し、その内容をプログラムカウンタにロードした後、割り込みサービスルーチンに分岐します。

内部割り込みはIRQと全く同じ信号(IRQ2)を発生させますが、ベクタアドレスが\$FFF0～\$FFF7になります。

IRQとIRQ2が同時に発生した場合は、前者が優先されます。コンディションコードレジスタの割り込みマスクビットがセットされていると、両方の割り込みがオフになります。

アドレスエラーまたはオペコードエラーが発生すると、TRAP 割り込みが発生します。この割り込みはRESの次の優先度を持ちます。割り込みマスクビットの状態に関係なく、CPUは割り込みシーケンスを開始します。この割り込みのベクタは \$FFEE、\$FFEFになります。

###  Read/Write (R/W) 
このTTL互換出力は、CPUがリード("High")かライト("Low")かに関わらず、周辺機器やメモリデバイスに信号を送る。通常のスタンバイ状態はリード("High")である。この出力は1つのTTL負荷と90pF容量を駆動します。

### Address Strobe (AS) 
多重化モードでは、アドレスストローブ信号がこのピンに現れます。D0/A0-D7/A7でデータと多重化された下位8ビットのアドレスをラッチするために使用されます。8ビットのラッチは図15に示すようにアドレスストローブによって制御される。これにより、Eパルスの間、D0/A0-D7/A7はデータバスになることができる。この信号のタイミングチャートを図1に示す。

アドレスストローブ(AS)は内部アドレスのメモリアクセスの際も出力されます。

##  PORTS 
HD6303R MPUのI/Oポートは、8ビットと5ビットの2ポートです。各I/Oポートには独立した書き込み専用のデータ方向レジスタがあり、各I/Oピンを入力用または出力用にプログラムすることができます。\*

関連するデータ方向レジスタのビットが "1"の場合、1/0ピンは出力用にプログラムされ、"0"の場合は入力用にプログラムされます。

ポートは2つあります:  ポート1とポート2です。各ポートのアドレスと関連するデータディレクションレジスタを表2に示します。

* 唯一の例外は、ポート2のビット1で、データ入力またはタイマ出力となる。出力ポートとしては使用できない。

Table 2 Port and Data Direction Register Addresses 

|Ports|Port Address |Data Direction<br> Register Address 
|--|--|--|
I/O Port 1 |\$0002 |\$0000 
I/O Port 2 |\$0003 |\$0001

### I/O Port 1 
これは8ビットポートで、各ビットは関連するデータディレクションレジスタによって個別に入力または出力として定義される。8ビット出力バッファは3ステート機能を持ち、入力に使用されるときはハイインピーダンス状態を維持する。正確に読み取るためには、入力ラインの電圧はロジック "1"で2.0V以上、ロジック "0"で0.8V以下でなければなりません。

これらはTTL互換である。MPU がリセットされた後、マルチプレクスモードでは全ての I/O ラインが入力に設定される。非多重モードでは、ポート 1 は低次アドレスライン(A0-A7)の出力ラインとなり、1 つの TTL 負荷と 30pF の容量を駆動することができます。

###  I/O Port 2 
このポートには5本のラインがあり、そのI/O方向はデータ方向レジスタに依存する。5ビットの出力バッファは3ステート機能を持ち、入力として使用されるときはハイインピーダンス状態になる。正確に読み出すためには、入力ラインの電圧はロジック "1"で2.0V以上、ロジック "0"で0.8V以下でなければならない。MPU がリセットされると全ての入出力端子は入力となります。ポート 2 (チップの P20 P22) のこれらのピンは、リセット時の動作モードをプログラムするために使用される。リセット中のこれら 3 つのピンの値は、MODE SELECTION セクションで説明するポート 2 データレジスタの上位 3 ビット(ビット 7、6、5)にラッチされる。

全てのモードにおいて、ポート 2 は I/O ラインとして設定できる。このポートはシリアルI/Oとタイマへのアクセスも提供する。ただし、ビット 1(P21)はデータ入力またはタイマ出力に制限された唯一のピンであることに注意。

##  BUS 

### D0/A0 - D7/A7 
このTTL互換3ステートバッファは、1つのTTL負荷と90 pF容量を駆動することができます。

* **非多重モード**:  このモードでは、これらのピンはデータバス (Do - D7) のみとなります。
* **多重化モード**:  データバス(Do - D7)とアドレスバスの下位ビット(A0 - A7)の両方になります。アドレスがピン上にある場合、アドレスストローブ出力は "High"になります。

### A8 - A15
各ラインはTTL互換で、1つのTTL負荷と90pF容量を駆動できる。リセット後、これらのピンは上位アドレスライン(A8～A15)の出力となる。

## MODE SELECTION 
リセット後の動作モードは、P20,P21,P22 の外部配線により決定される。これら 3 つのピンは、ポート 2 の I/O 0、I/O 1、I/O 2 の下位ビットである。RESが "H"になるとI/Oポート2レジスタの制御ビットPC0、PC1、PC2にラッチされる。I/Oポート2レジスタを以下に示す。

Port 2 DATA REGISTER 

<img width=382, src="img/026-figure-port2-data-register.png">

モード選択に使用される外部ハードウェアの例を図 11 に示します。HD14053Bは、リセット時に周辺デバイスとMPUを分離するために使用します。周辺デバイスとモード生成回路の間でデータが衝突する可能性がある場合に必要である。

ポート2データレジスタの5,6,7ビットは読み出し専用であるため、ソフトウェアによるモード変更はできません。

HD6303Rのモード選択を表3に示します。HD6303Rは、(1)多重モード、(2)非多重モードの2つの基本モードで動作します。

### Multiplexed Mode (多重モード)
データバスと低次アドレスバスはD0/A0-D7/A7で多重化され、アドレスストローブで分離できる。

ポート2は、5パラレルI/O、シリアルI/O、タイマ、またはそれらの組み合わせ用に構成される。ポート1は8パラレル1/0用に構成される。

### Non Multiplexed Mode (非多重モード)
このモードでは、HD6303RはアドレスラッチなしでHMCS6800ペリフェラルを直接アドレス指定できます。D0/A0-D7/A7がデータバスになり、ポート1がA0-A7のアドレスバスになります。

このモードでは、HD6303Rはアドレスラッチなしで最大65kバイトまで拡張可能です。

### Lower Order Address Bus Latch 
多重化モードでは、Do/Ao～D7/A7でデータバスが下位アドレスバスと多重化されるため、アドレスビットをラッチする必要がある。LSBをラッチするには74LS373トランスペアレント8進Dラッチが必要です。HD6303Rのラッチ接続を図15に示します。

<div style="page-break-before:always"></div>

Figure 11 Recommended Circuit for Mode Selection 

<img width=670, src="img/027-figure11-recommended-circuit-for-mode-selection.png">

Figure 12 HD14053B Multiplexers/De-Multiplexers 

<img width=643, src="img/028-figure12-hd14053b-multiplexers-de-multiprexers.png">

<div style="page-break-before:always"></div>

Figure 13 HD6303R MPU Multiplexed Mode 

<img width=403, src="img/029-figure13-hd6303r-mpu-multiplexed-mode.png">

Figure 14 HD6303R MPU Non Multiplexed Mode 

<img width=382, src="img/030-figure14-hd6303r-mpu-non-multiplexed-mode.png">

Figure 15 Latch Connection 

<img width=805, src="img/031-figure15-latch-connection.png">

Table 3 Mode Selection 

<img width=480, src="img/032-table3-mode-selection.png">

<div style="page-break-before:always"></div>

Table 4 Internal Register Area 

<img width=463, src="img/033-table4-internal-register-area.png">

## MEMORY MAP 
MPUは最大65kバイトのアドレス空間を提供できる。図 16 に各動作モードのメモリマップを示す。各マップの先頭 32 位置は、表 4 に示すように CPU 内部レジスタのみである。

<div style="page-break-before:always"></div>

Figure 16 HD6303R Memory Maps 

<img width=769, src="img/034-figure16-hd6303r-memory-maps.png">

## PROGRAMMABLE TIMER 
HD6303Rは16ビットのプログラマブルタイマを内蔵しており、入力波形を測定することができます。また、出力波形を自ら生成することもできます。入力波形、出力波形ともに、パルス幅は数マイクロ秒から数秒まで変化します。

タイマのハードウェアは次の要素により構成されています。

* 8ビットの制御およびステータスレジスタ 
* 16ビットフリーランニングカウンタ 
* 16ビット出力比較レジスタ 
* 16ビット入力キャプチャレジスタ 

タイマのブロック図を図 17 に示す。

Figure 17 Programmable Timer Block Diagram 

<img width=534, src="img/035-figure17-programmable-timer-block-diagram.png">

### Free Running Counter (\$0009: \$000A) 
プログラマブルタイマのキーエレメントは、E(イネーブル)クロックによって値をインクリメントする16ビットのフリーランカウンタである。カウンタ値は、CPUソフトウェアによっていつでも読み出されるが、カウンタに影響はない。リセットするとカウンタはクリアされます。

このカウンタのMSBが読み出されると、LSBがテンポラリラッチに格納されます。その後のLSBの読み出しによって、このラッチからデータが取り出されます。このようにして、一貫性のある2バイトデータをカウンタから読み出すことができます。

CPUがMSB(\$09)に任意のデータを書き込むと、書き込みデータの値に関係なくカウンタ(\$09, \$OA)に\$FFF8がプリセットされる。次にCPUがLSB(SOA)に任意のデータを書き込むと、そのデータがカウンタのLowバイトにセットされ、同時にMSB(\$09)に先に書き込まれたデータがカウンタのHighバイトにセットされる。

このカウンタにデータを書き込む場合は、2バイトストア命令(STD など)を使用しなければならない。カウンタの MSB だけを書き込むと、カウンタは \$FFF8 に設定されます。

2バイトストア命令を使用してカウンタに書き込まれるカウンタ値を図 18 に示す。

カウンタへの書き込みはシリアル動作の妨げになるため、SCI 使用中は禁止すること。SCI で外部クロックモードを使用する場合は、シリアル動作の妨げにはなりません。

Figure 18 Counter Write Timing 

<img width=473, src="img/036-figure18-counter-write-timing.png">

###  Output Compare Register (\$000B:\$000C) 
このレジスタは 16 ビットのリード/ライトレジスタで、出力波形の制御に使用される。このレジスタの内容はフリーランカウンタの現在値と常に比較される。

内容がフリーランニングカウンタの値と一致すると、タイマ制御/ステータスレジスタ(TCSR)のフラグ(OCF)がセットされ、TCSRの出力レベルビット(OLVL)の現在値がポート2のビット1に転送される。ポート 2 のデータ方向レジスタのビット 1 が "1"(出力)の時、OLVL の値はポート 2 のビット 1 に表示される。その後、出力比較レジスタと出力レベルビットの値は次の比較のために変更することができる。

出力コンペアレジスタはリセット中\$FFFFに設定されます。

出力コンペアレジスタの上位バイトへの書き込みサイクルとその直後のサイクルでコンペア機能が禁止され、 有効なコンペアが保証される。また、フリーランニングカウンタへの書き込みも同様に禁止される。

出力コンペアレジスタにデータを書き込むには、2バイトストア命令(例えばSTD命令)を使用しなければならない。

###  Input Capture Register (\$000D: \$000E) 

入力キャプチャレジスタは16ビットの読み出し専用レジスタで、外部入力信号が適切に遷移したときにキャプチャされるフリーランニングカウンタの現在値を保持するために使用される。

カウンタ転送のトリガに必要な入力遷移の変化は、入力エッジビット(IEDG)によって制御される。

外部入力信号がエッジ検出ユニットに入るためには、ポート2のビット0に対応するデータ方向レジスタのビットがクリア(ゼロに)されていなければなりません。

すべてのケースで入力キャプチャを保証するために、入力パルスの幅は少なくとも2イネーブル(E)サイクルを必要とする。

### Timer Control/Status Register (TCSR) (\$0008) 
これは8ビットのレジスタである。8ビット全ては読み出し可能で、下位5ビットは書き込み可能である。上位3ビットは読み出し専用で、以下に示すタイマのステータス情報を示す。

1. 入力ピン(ICF)で適切な遷移が検出された。
2. フリーランニングカウンタの値と出力コンペアレジスタ(OCF)の値が一致した。
3. \$0000(TOF)までカウントしたとき。

各フラグには、割り込み要求(IRQ2)が発生するかどうかを決定する個別のイネーブルビットがTCSRにあります。コンディションコードレジスタのIビットが事前にクリアされていると、各フラグに対応する先行ベクトルアドレスが発生します。各ビットの説明は以下の通り。

Figure. Timer Control / Status Register 

<img width=400, src="img/037-timer-counter-status-register.png">

**ビット0 OLVL(出力レベル):** OLVL(出力レベル): カウンタと出力コンペアレジスタの値が一致すると、このビットはポート 2 のビット 1 に転送される。ポート 2 のビット 1 に対応する DDR が "1"に設定されている場合、ポート 2 のビット 1 の出力ピンに値が現れる。

**ビット1 IEDG(入力エッジ):** このビットは、ポート 2 ビット 0 の入力のどの遷移がカウンタから入力キャプチャレジスタへのデータ転送をトリガするかを制御する。この機能を使用する前に、ポート 2 ビット 0 に対応する DDR をクリアしておく必要がある。IEDG = 0の時、トリガは負エッジ("High"-"Low"遷移)で起こり、IEDG = 1の時、トリガは正エッジ("Low"-"High"遷移)で起こる。

**ビット2 ETOI (Enable Timer Overflow Interrupt):** このビットがセットされるとTOF割り込みが有効になり、割り込み要求(IRQ2)を生成します。クリアされると割り込みは禁止されます。

**ビット3 EOCI(Enable Output Compare Interrupt):** このビットがセットされると、OCF 割り込みが有効になり、割り込み要求 (IRQ2) が生成されます。クリアされると、割り込みは禁止されます。

**ビット4 EICI (Enable Input Capture Interrupt):** このビットがセットされると、ICF割り込みが割り込み要求(IRQ2)を生成します。クリアされると割り込みは禁止されます。

**Bit 5 TOF (タイマオーバーフローフラグ):** この読み出し専用ビットは、カウンタの\$FFFFから\$0000への遷移時に設定されます。(TOFが設定された状態で)TCSRのCPU読み出しに続いてカウンタのCPU読み出し(\$0009)を行うとクリアされます。

**Bit 6 OCF (出力比較フラグ):** この読み出し専用ビットは、出力比較レジスタとカウンタの値が一致した時に設定されます。このビットは、TCSRのリード(OCFがセットされている状態)に続いて、CPUが出力コンペアレジスタ(\$000Bまたは\$000C)に書き込むとクリアされます。

**ビット7 ICF(入力キャプチャフラグ):** この読み出し専用ビットは、入力の適切な遷移によってセットされ、TCSRの読み出し(OCFがセットされた状態)によってクリアされる。
(ICFが設定された状態で)TCSRを読み出し、次にCPUが入力キャプチャレジスタ(\$000D)を読み出すとクリアされます。

リセットは、タイマ制御およびステータスレジスタの各ビットをクリアする。

<div style="page-break-before:always"></div>

## SERIAL COMMUNICATION INTERFACE 
HD6303Rは、全二重の非同期シリアル通信インタフェース(SCI)を内蔵しています。SCIは、数種類のデータレートを選択することができます。SCIは、同じデータフォーマットと同じデータレートで動作するトランスミッタとレシーバで構成されています。トランスミッタとレシーバの両方は、データバスを介してCPUと通信し、ポート2のビット2、3、4を介して外部と通信する。ハードウェア、ソフトウェア、レジスタの説明は以下の通り。

###  Wake-Up Feature 
一般的なマルチプロセッサアプリケーションでは、ソフトウェアプロトコルは通常メッセージの先頭バイトに指定アドレスを持つ。Wake-Up機能の目的は、非選択MPUにメッセージの残りを無視させることです。そのため、非選択MPUは次のメッセージが始まるまで、それ以降の割り込み処理をすべて禁止することができます。

Wake-Up機能は10回連続の "1"で再有効となり、これは送信ラインがアイドルであることを示す。従って、ソフトウェアプロトコルはメッセージとメッセージの間にアイドル期間を設け、メッセージ内ではそれを防ぐ必要がある。

このハードウェア機能により、非選択 MPU は次のメッセージで再有効化(wake-up)される。

### Programmable Options 
HD6303Rには、以下のプログラマブル機能があります。

* データフォーマット: 標準マーク/スペース(NRZ)
* クロックソース: 外部または内部
* ボーレート: 所定のEクロック周波数または外部クロックの1/8あたり4つのレートのうちの1つ 
* ウェイクアップ機能: 有効または無効 
* 割り込み要求: 送信機と受信機で個別に有効またはマスクされる。
* クロック出力: ポート2ビット2への内部クロック出力の有効/無効 
* ポート2(ビット3、4): 個別にシリアルI/O専用または非専用

### Serial Communication Hardware 
シリアル通信ハードウェアは、図 19 に示すように 4 つのレジスタによって制御される。レジスタには以下が含まれる:

* 8 ビットのコントロール/ステータスレジスタ 
* 4 ビットのレート/モード制御レジスタ(書き込み専用) 
* 8 ビット読み取り専用受信データレジスタ 
* 8 ビット書き込み専用送信データレジスタ

これら4つのレジスタの他に、シリアルI/Oはポート2のビット3(入力)とビット4(出力)を利用する。ポート 2 のビット 2 は、内部クロック出力または外部クロック入力のオプションが選択されている場合に使用できる。

### Transmit/Receive Control Status Register (TRCSR) 
TRCSレジスタは8ビットで構成され、全て読み出し可能であるが、0～4ビットのみ書き込み可能である。レジスタはRESで\$20に初期化される。TRCSレジスタのビットを以下に説明する。

Figure. Transmit / Receive Control Status Register 

<img width=400, src="img/038-transmit-receive-control-status-register.png">

**ビット0 WU(Wake Up):** ソフトウェアによって設定され、10回連続して "1"を受信すると ハードウェアによってクリアされる。このビットが "1"の間、RDRFフラグとORFEフラグは、データを受信してもエラーを検出してもセットされない。従って受信データは無視される。WUフラグがセットされる前にREフラグがセットされていなければならない。

**ビット1 TE (Transmit Enable):** このビットは送信機を有効にする。このビットがセットされると、ポート2 DDRのビット4も強制的にセットされる。TEがクリアされてもセットされたままである。このビットがセットされた直後に10個の連続した "1"のプリアンブルが送信され、送信機はデータ送信のレディになる。このビットがクリアされた場合、送信機は無効となり、シリアルI/Oはポート2のビット4に何も影響を与えない。

**ビット2 TIE(送信割り込みイネーブル):** このビットがセットされると、TDRE(ビット5)はIRQ2割り込みを発生させる。クリアされると、TDRE割り込みはマスクされる。

**ビット3 RE(受信イネーブル):** セットされると、ポート2のビット3は、このビットのDDR値に関係なく、受信の入力として使用できる。クリアされると、受信は無効となる。

**ビット4 RIE(Receive Interrupt Enable):** このビットがセットされると、RDRF(ビット7)またはORFE(ビット6)によりIRQ2割り込みが発生する。クリアされると、この割り込みはマスクされる。

**ビット5 TDRE(送信データレジスタエンプティ):** データが送信データレジスタから出力シフトレジスタに転送されると、このビットはハードウェアによってセットされる。このビットは、ステータスレジスタを読み出し、次の新しいデータを送信データレジスタに書き込むことによってクリアされます。TDREはRESによって1に初期化される。

**ビット6 ORFE(オーバーラン/フレーミングエラー):** オーバーランまたはフレーミングエラーが発生すると(受信のみ)、 このビットはハードウエアによって設定される。オーバーランエラーは、RDRF が "1"の間に新しいバイトを受信データレジスタに転送しようとした場合に発生する。フレーミングエラーは、ビットカウンタが受信ビットストリームのバイトの境界と同期していない場合に発生する。フレーミングエラーが検出されると、RDRF はセットされない。したがって、フレーミングエラーはオーバーランエラーと区別できる。すなわち、ORFE が "1"で RDRF が"1"であれば、オーバーランエラーが検出される。それ以外の場合はフレーミングエラーが発生する。このビットは、ステータスレジスタの読み出しの後に受信データレジスタを読み出すか、 RES によってクリアされる。

**ビット 7 RDRF(受信データレジスタフル):** このビットは受信シフトレジスタから受信データレジスタにデータが転送された時にハードウェアによってセットされる。このビットは、ステータスレジスタの読み出しに続いて受信データレジスタを読み出すか、 RES によってクリアされる。

<div style="page-break-before:always"></div>

Figure 19 Serial I/O Register 

<img width=439, src="img/039-figure19-serial-io-register.png">

<div style="page-break-before:always"></div>

Table 5 SCI Bit Times and Transfer Rates 

<img width=600, src="img/040-table5-sci-bit-times-and-transfer-rates.png">

Table 6 SCI Format and Clock Source Control 

<img width=600, src="img/041-table6-sci-bit-format-and-clock-source-control.png">

### Transfer Rate/Mode Control Register (RMCR) 
このレジスタは、以下のシリアルI/O機能を制御する:

* ボーレート 
* データフォーマット 
* クロックソース 
* ポート 2 ビット 2 機能

4ビットの書き込み専用レジスタで、RESでクリアされる。4ビットは一対の2ビットフィールドとみなされる。下位2ビットは内部クロックのビットレートを制御し、上位2ビットはフォーマットとクロックセレクトロジックを制御する。

|||
|--|--|
|Bit0 SS0<br>Bit1 SS1|Speed Select 

これらのビットは内部クロックのボーレートを選択する。選択可能なレートはCPUのEクロック周波数の関数である。表5に選択可能なボーレートを示す。

|||
|--|--|
|Bit2 CC0<br>Bit3 CC1|Clock Control/Format Select 

これらのビットはデータフォーマットとクロックセレクトロジックを制御する。表6にビットフィールドを定義する。

### Internally Generated Clock
シリアルI/Oの内部クロックを外部で使用する場合は、以下の要件に注意する必要がある。

* CCI、CCOは必ず "10"に設定すること。
* 最大クロックレートはE/16でなければならない。
* クロックレートはビットレートと等しい。
* REとTEの値は影響しない。

### Externally Generated Clock 
シリアルI/Oに外部クロックを供給したい場合、以下の要件に注意する必要がある。

* CC1、CCOは "11"に設定されなければならない(表6参照)。
* 外部クロックは、希望のボーレートの8倍に設定しなければならない。
* 外部クロックの最大周波数はE/2クロックです。

### Serial Operations 
シリアルI/Oハードウェアは、動作前にソフトウェアによって初期化されなければならない。シーケンスは通常以下のようになる。

* レートモード制御レジスタの希望の動作制御ビットを書き込む。
* TRCSレジスタの希望の動作制御ビットを書き込む。

ポート2のビット3,4をシリアルI/Oに使用する場合、TE,REビットはセットされたままでよい。SCI動作中にTE,REビットがクリアされ、その後再びセットされる場合、TE,REは現在のボーレートの少なくとも1ビット時間 "0"を維持しなければならないことに注意すること。もしTE,REが1ビット時間以内に再びセットされた場合、トランスミッタとレシーバの内部機能の初期化が正しく行われない場合がある。

### Transmit Operation 
データ送信は TRCS レジスタの TE ビットで有効になる。設定されると、送信シフトレジスタの出力はポート 2 のビット 4 に接続され、無条件に出力に設定される。

RES の後、ユーザは RMC レジスタと TRCS レジスタの両方を初期化して望ましい動作にする必要がある。TE ビットを設定すると 10 ビットのプリアンブル "1"が送信される。プリアンブルの後、内部同期が確立され、トランスミッタは動作可能な状態になる。その後、次のいずれかの状態になる。

1. 送信データレジスタが空の場合(TDRE 1)、アイドル状態を示す連続した "1"が送信される。
2. データが送信データレジスタにロードされている場合(TDRE 0)、データは出力シフトレジスタに転送され、データ転送が開始される。

データ転送中、まずスタートビット("0")が転送される。次に(ビット 0 から始まる)8 ビットのデータが転送され、最後にストップビット("1")が転送されます。送信データレジスタの内容が出力シフトレジスタに転送されると、ハードウェアは TDRE フラグビットを設定します:  CPUが適切な時間内にフラグに応答できなかった場合、TDREはセットされたままとなり、データがデータレジスタに供給されるまで、連続した "1"の文字列が送信される。

<div style="page-break-before:always"></div>

### Receive Operation 
受信動作は RE ビットで有効になる。シリアル入力はポート 2 のビット 3 に接続される。受信動作は TRCS と RMC レジスタの内容によって決定される。受信ビットストリームは最初の "0"(スタートビット)によって同期される。10ビット時間中、データは各ビットのほぼ中央でストローブされる。第10ビットが "1"(ストップビット)でない場合、システムはフレーミングエラーと見なし、ORFEが設定される。

第10ビットが "1"であれば、データは受信データレジスタに転送され、RDRFフラグが設定される。次のデータの 10 ビット目が受信され、RDRF がセットされたままであれば、ORFE がセットされ、オーバランエラーが発生したことを示す。

RDRFフラグまたはORFEフラグに対する応答としてCPUがステータスレジスタを読み出した後、CPUが 受信データレジスタを読み出すと、RDRFまたはORFEはクリアされる。

## RAM CONTROL REGISTER 
アドレス\$0014に割り当てられているレジスタは、スタンバイRAMのステータス情報を与える。

Figure. RAM Control Register 

<img width=400, src="img/042-ram-control-register.png">

|||
|--|--|
|Bit 0|Not used.  
|Bit 1|Not used.  
|Bit 2|Not used.  
|Bit 3|Not used.  
|Bit 4|Not used.  
|Bit 5|Not used.  
|Bit 6|RAM Enable (RAME). <br><br>RAMイネーブルビットは、RESのプラスエッジで設定され、RAMが<br>有効になります。プログラムは "1"または "0"を書き込むことが<br>できます。RAMEがクリアされると、RAMアドレスは外部アドレスと<br>なり、CPUは外部メモリからデータを読み出すことができます。
|Bit 7|Standby Power Bit (STBY PWR)<br><br>このビットはユーザプログラムにより読み書き可能である。Vcc電圧が<br>除去されるとクリアされる。通常、このビットはスタンバイモードに入る<br>前にプログラムによってセットされる。CPUがスタンバイモードから復帰<br>したとき、このビットをチェックする必要がある。このビットが "1"で<br>あれば、RAMのデータはスタンバイ中も保持され、有効である。

## GENERAL DESCRIPTION OF INSTRUCTION SET 
HD6303Rは、HMCS6800の全命令セットを利用するため、HD6801と上位互換のオブジェクトコードを持つ。キー命令の実行時間を短縮し、システムスループットを向上させています。また、ビット演算命令、インデックスとアキュムレータの交換命令、スリープ命令が追加されています。本節では、以下の内容を説明する:  

* CPU プログラミングモデル(図 20 参照) 
* アドレス指定モード 
* アキュムレータおよびメモリ操作命令(表 7 参照) 
* 新しい命令 
* インデックスレジスタとスタック操作命令(表 8 参照) 
* ジャンプ分岐命令(表 9 参照) 
* 条件コードレジスタ操作命令(表 10 参照) 
* オペコードマップ(表 11 参照) 
* サイクルごとの操作(表 12 参照)

### CPU Programming Model 
HD6303Rのプログラミングモデルを図20に示します。ダブルアキュムレータは、物理的にはアキュムレータAとアキュムレータBを連結したもので、アキュムレータDの実行操作でAとBの内容が変化します。

<div style="page-break-before:always"></div>

Figure 20. CPU Programming Model

<img width=400, src="img/043-figure20-cpu-programming-model.png">

### CPU Addressing Modes
HD6303Rには、命令の種類とコードによって7つのアドレスモードがあります。 各命令のアドレスモードと実行時間をマシンサイクルで示します(表7～表11)。クロック周波数が4MHzの場合、マシンサイクルはマイクロ秒になります。

### Accumulator (ACCX) Addressing 
アキュムレータ(A または B)のみがアドレス指定されます。アキュムレータ A または B のどちらかを 1 バイト命令で指定します。

### Immediate Addressing 
このモードでは、オペランドは命令の2バイト目に格納されるが、LDSやLDXなどのオペランドは2バイト目と3バイト目に格納される。これらは2バイトまたは3バイト命令である、

### Direct Addressing 
このモードでは、命令の2バイト目がオペランドが格納されているアドレスを示す。ダイレクトアドレス指定では、マシンの最下位256バイト(0～255番地)を直接アドレス指定できます。これらの場所にデータを格納することで、実行時間の向上が達成される。システム構成上、これらの場所はRAMとし、ユーザーのデータ領域に利用することが推奨される。AIM、OIM、EIM、TIMが3バイトである以外は、これらは2バイト命令である。

### Extended Addressing 
このモードでは、2バイト目がオペランドが格納されている上位8ビットのアドレスを示し、3バイト目が下位8ビットのアドレスを示す。これはメモリ上の絶対アドレスである。これらは3バイト命令である。

### Indexed Addressing 
このモードでは、2バイト目の内容がインデックスレジスタの下位8ビットに加算される。AIM、OIM、EIM、TIMの各命令では、3バイト目の内容がインデックスレジスタの下位8ビットに加算されます。さらに、結果の "キャリー"が インデックスレジスタの上位8ビットに加算されます。その結果がメモリのアドレス指定に使用される。変更されたアドレスは一時アドレスレジス タに保持されるため、インデックスレジスタに変更はない。これらは2バイト命令ですが、AIM、OIM、EIM、TIMは3バイト命令です。

### Implied Addressing 
このモードでは、命令自体がアドレス、スタックポインタ、インデックスレジスタなどを与える。これらは1バイト命令である。

### Relative Addressing 
このモードでは、2 バイト目の内容がプログラムカウンタの下位 8 ビットに加算される。その結果、キャリーまたはボローが上位8ビットに加算される。これにより、ユーザーは現在の実行命令から-126～+129バイトの範囲内のデータをアドレス指定することができる。これらは2バイト命令である。

<div style="page-break-before:always"></div>

Table 7 Accumulator, Memory Manipulation Instructions 

<img width=700, src="img/044-instruction-table1.png">

<div style="page-break-before:always"></div>

Table 7 Accumulator, Memory Manipulation Instructions (cont) 

<img width=700, src="img/045-instruction-table2.png">

### New Instructions 
HD6303Rでは、HD6801命令セットに加え、新たに以下の命令が追加されました: 

|||
|--|--|
AIM|(M) · (IMM) → (M)<br>即時データとメモリの AND を評価し、結果をメモリに配置する。 
OIM|(M) + (IMM) → (M)<br>即値データとメモリのORを評価し、結果をメモリに格納。
EIM|(M) ✪ (IMM) → (M)<br>即値データとメモリのEORを評価し、結果をメモリに格納。
TIM|(M) · (IMM)<br>即値データとメモリのANDを評価し、関連する<br>コンディションコードレジスタのフラグを変更する。
|||

各命令は3バイトあり、1バイト目がオペコード、2バイト目が即値データ、3バイト目がアドレス修飾子である。

|||
|--|--|
XGDX|(ACCD) → (IX) <br>アキュムレータとインデックスレジスタの内容を交換します。
SLP|MPU をスリープモードに移行させます。スリープモードに<br>ついては、「スリープモード」の項を参照してください。
|||

Table 8 Index Register, Stack Manipulation Instructions 

<img width=700, src="img/046-table8-index-register-stack-manipulation-instructions.png">

<div style="page-break-before:always"></div>

Table 9 Jump, Branch Instruction 

<img width=700, src="img/047-table9-jump-branch-instructions.png">

<div style="page-break-before:always"></div>

Table 10 Condition Code Register Manipulation Instructions 

<img width=700, src="img/048-table10-cc-register-manipulation-instruction.png">

[NOTE 1] Condition Code Register Notes: (Bit set if test is true and cleared otherwise) 

1. Test: Result = 10000000? 
2. (Bit C) Test: Result * 00000000? 
3. (Bit C) Test: BCD Character of high-order byte greater than 9? (Not cleared if previously set) 
4. (Bit V) Test: Operand = 10000000 prior to execution? 
5. (Bit V) Test: Operand = 01111111 prior to execution? 
6. (Bit V) Test: Set equal to N®C=1 after the execution of instructions 
7. (Bit N) Test: Result less than zero? (Bit 15=1) 
8. (All B1t) Load Condition Code Register from Stack. 
9. (Bit 1) Set when interrupt occurs. If previously set, a Non-Maskable Interrupt is required to exit the wait state. 
10. (All Bit) Set according to the contents of Accumulator A. 
11. (Bit C) Result of Multiplication Bit 7=1 of ACCB? 

[NOTE 2] CLI instruction and interrupt.  
If interrupt mask-bit is set (I="1") and interrupt is requested (IRO, = "0" or IRQ2 = "0"), and then CLI instruction is executed, the CPU responds as follows. 

1. The next instruction of CLI is one-machine cycle instruction.  Subsequent two instructions are executed before the interrupt is responded. That is, the next and the next of the next instruction are executed. 
2. The next instruction of CLI is two-machine cycle (or more) instruction.  Only the next instruction is executed and then the CPU jump to the interrupt routine. 

Even if TAP instruction is used, instead of CLI, the same thing occurs. 

Table 11 OP-Code Map 

<img width=700, src="img/049-table11-op-code-map.png">

<div style="page-break-before:always"></div>


### Instruction Execution Cycles 
HMCS6800シリーズでは、各命令の実行サイクルは、現在の命令フェッチ開始から後続命令フェッチ開始直前までのサイクル数となります。

HD6303Rでは、命令フェッチにパイプライン制御の仕組みを採用しており、後続命令フェッチは現在の命令実行中に行われます。

従って、HD6303RのMULT、PULL、DAA、XGDXなどの命令サイクルには、HMCS6800シリーズで採用されている命令サイクルのカウント方法は適用できません。

表12に、各命令実行時のサイクル毎のアドレスバス、データバス、R/Wステータスの各データの関係を示します。

<figure>
<img width=700, src="img/050-table12-cycle-by-cycle-operation.png">
</figure><figure>
<img width=700, src="img/051-table12-cycle-by-cycle-operation2.png">
</figure><figure>
<img width=700, src="img/052-table12-cycle-by-cycle-operation3.png">
</figure><figure>
<img width=700, src="img/053-table12-cycle-by-cycle-operation4.png">
</figure><figure>
<img width=700, src="img/054-table12-cycle-by-cycle-operation5.png">
</figure><figure>
<img width=700, src="img/055-table12-cycle-by-cycle-operation6.png">
</figure>

<div style="page-break-before:always"></div>

## LOW POWER CONSUMPTION MODE 
HD6303Rには、スリープモードとスタンバイモードの2つの低消費電力モードがあります。

### Sleep Mode 
SLP 命令を実行すると MPU はスリープモードに移行する。スリープモードでは CPU は動作を停止しますが、CPU 内のレジスタの内容は保持されます。このモードでは、CPU の周辺回路はアクティブのままである。そのため、SCIデータの送受信やカウンタなどの動作は継続されます。このモードでは、消費電力は通常動作時の1/6程度に抑えられる。

このモードからの復帰は割り込み、RES、STBYです。RESはMPUをリセットし、STBYはMPUをスタンバイモード(後述)に移行させる。割り込みが CPU に要求され受け付けられるとスリープモードが解除され、CPU は動作モードに入り割り込みルーチンにジャンプする。CPUが割り込みをマスクすると、スリープモードから復帰した後、SLPの次の命令の実行が開始される。ただし、タイマ側でタイマ割り込みが禁止されている場合は、CPUへの割り込み要求がないため、スリープモードを解除できない。

このスリープモードは、HD6303Rを常時動作させないアプリケーションにおいて、平均的な消費電力を削減するために使用できます。

### Standby Mode 
STBYを "Low"にするとCPUがリセットされ、HD6303Rの全てのクロックが非アクティブになります。スタンバイ状態になります。このモードはHD6303Rの消費電力を著しく低減します。

スタンバイモードでは、HD6303Rに電力を供給し続けるとRAMの内容が保持されます。スタンバイモードは、リセットスタートにより解除されます。このモードの典型的な応用例を示します。

まず、NMIルーチンでCPUの内部情報とSPの内容をRAMにスタックし、RAMコントロールレジスタのRAMEビットをディセーブルにしてスタンバイビットをセットし、スタンバイモードに入ります。リセットスタート時にスタンバイビットがセットされたままであれば、スタンバイモード中に電源が保持され、RAMの内容が正常に保証されていることを意味します。SP を復帰させ、スタンバイモードが開始する前の状態にすることで、システムの復旧が可能な場合がある。本アプリケーションにおける各ラインのタイミング関係を図 21 に示す。

Figure 21 Standby Mode Timing 

<img width=400, src="img/056-figure21-standby-timing.png">

## ERROR PROCESSING 
HD6303Rは、未定義の命令をフェッチしたり、使用不可能なメモリ領域から命令をフェッチすると、最高優先度の内部割り込みを発生させ、ノイズやプログラムエラーによるシステムの混乱を防ぎます。

### Op-Code Error 
未定義のオペコードをフェッチすると、HD6303Rは通常の割り込みの場合と同様にCPUレジスタをスタックし、2番目に優先度の高い(RESが最高)TRAP(\$FFEE、\$FFEF)にベクタします。

<div style="page-break-before:always"></div>

### Address Error 
常駐RAM以外、かつ外部メモリ領域以外から命令をフェッチした場合、CPUはオペコードエラーと同じ割り込みを開始します。外部メモリ領域から命令をフェッチした場合で、その領域が使用できない場合は、アドレスエラーを検出できません。

アドレスエラーが発生するアドレスを表 13 に示す。

この機能は命令フェッチにのみ適用され、通常のデータアクセスの読み出し/書き込みには適用されない。

アクティブモード、スリープモード、スタンバイモード、リセット間の遷移を図 22 に示す。

図23、24にシステム構成を示します。
HD6303Rのシステムフローチャートを図25に示します。

Table 13 Address Error 

<img width=250, src="img/058-table13-address-error.png">

<div style="page-break-before:always"></div>

Figure 22 Transitions among Active Mode, Standby Mode, Sleep Mode, and Reset 

<img width=418, src="img/057-figure22-tansition-amoung-several-modes.png">


<div style="page-break-before:always"></div>

Figure 23 HD6303R MPU Multiplexed Mode 

<img width=397, src="img/059-figure23-hd6303r-mpu-multiplexed-mode.png">

<div style="page-break-before:always"></div>

Figure 24 HD6303R MPU Non-Multiplexed Mode 

<img width=402, src="img/060-figure24-hd6303r-mpu-non-multiprexed-mode.png">

Figure 25 HD6303R System Flow Chart 

> 画像省略

### PRECAUTION TO THE BOARD DESIGN OF OSCILLA. TION CIRCUIT 
図26に示すように、発振回路の近くに信号線を置くと、クロストークによって正常な発振が阻害される場合があります。基板設計の際には、この点に注意してください。水晶振動子やCLはできるだけHD6303Rの近くに配置する必要があります。

Figure 26 Precaution to the boad design of oscillation circuit 

<img width=315, src="img/061-figure26-precaution-to-the-boad-design-of-oscillation-circuit.png">

Fig. 27 Example of Oscillation Circuits in Board Design 

> 画像省略

### PIN CONDITIONS AT SLEEP AND STANDBY STATE 

### Sleep State 
電源端子、クロック端子、入力端子、Eクロック端子の条件は動作時と同じです。その他の端子条件は表14を参照してください。

### Standby State 
電源端子と STBY 端子のみがアクティブとなる。クロック端子 EXTAL は入力が内部で固定されており、MPU は端子状態の影響を受けない。XTAL は "1"出力である。その他の端子は全てハイインピーダンスである。

<div style="page-break-before:always"></div>

<figure style="text-align: center">
<figcaption>Table 14 Pin Condition in Sleep State </figcaption>
<img width=746, src="img/001-table14-pin-condigiton-in-sleep-state.png">
</figure>

<img width=835, src="img/062-table15-pin-condition-during-reset.png">

(注) 多重モードでは、E="1"の時にデータバスが "1"出力となり、外部メモリの出力と競合します。このコンフリクトを回避するために以下の1、2を行う必要があります； 

1. リセット時に外部メモリを無効にするシステムを構築する。
2. AS端子に4.7KΩのプルダウン抵抗を追加し、E="1"時にAS端子を "0"レベルにする。この操作により、データバスはハイインピーダンス状態になる。


## DIFFERENCE BETWEEN HD6303 AND HD6303R 
HD6303RはHD6303のアップグレード版である。HD6303とHD6303Rの違いを表16に示す。

Table 16 Difference between HD6303 and HD6303R 

<img width=458, src="img/063-table16-difference-between-hd6303-and-hd6303r.png">

|Item|HD6303|HD6303R|
|--|--|--|
|Operatiing<br>Mode|モード2: 定義なし|モード2: 多重モード<br>(モード4と同等)|
|Electrical<br>Character-<br>istics|2MHzバージョン(Bバージョ<br>ン)の電気的特性は規定<br>されていません。|一部の特性が改善されています。<br> 2MHz版は保証されます。
|Timer|出力コンペア機能に問題あり。<br>(ソフトウェアで回避可能)|解決済み
||||

<div style="page-break-before:always"></div>

## RECEIVE MARGIN OF THE SCI 
HD6303Rに内蔵されているSCIの受信マージンを表17に示します。  
注: SCI = シリアル通信インターフェース

Table 17

<img width=433, src="img/064-table17-receive-margin.png">

<img width=770, src="img/065-receive-margin-of-the-sci.png">

## APPLICATION NOTE FOR HIGH SPEED SYSTEM DESIGN USING THE HD6303R 
このノートでは、HD6303Rを使用したシステムで発生する可能性のあるノイズによる問題の解決方法について説明します。低消費電力、高耐ノイズ性を特長とするCMOS ICやLSISは、電源とGNDラインを設計するだけで十分と考えられています。

しかし、高速システムや高速部品で構成されるアプリケーションではそうはいきません。このような高速システムでは、スイッチング時に発生する過渡電流によるノイズのために、誤動作する可能性がある。その一例として、HD6303RがHM6264などの高速メモリに直接アクセスするシステムがあります。この場合、スイッチング時の過電流(ピークで数百mAになることもあります)によるノイズの発生により、データの書き込みエラーが発生することがあります。

このノイズは、HD6303Rの拡張モード(Mode 1, 2, 4, 5, 6)でのみ発生することがあります。

HD6303RをCPUとして使用する場合を想定しています。

#### I. Noise Occurrence 
If the HD6303R is connected to high speed RAM, a write error may occur. As shown in Fig. 28, the noise is generated in address bus during write cycle and data is written into an unexpected address from the HD6303R. This phenomenon causes random failures in systems whose data bus load capacitance exceeds the specification value (90 pF max.) and/or the impedance of the GND line is high. 

Fig. 28 Noise Occurrence in address bus during write cycle 

<img width=600, src="img/066-fig28-noise-occurence-in-address-bus-during-write-cycle.png">

If the data bus Do - D7, changes from "FF" to "00", extremely large transient current flows through the GND line. Then the noise is generated on the LSI's Vss pins proportioning to the transient current and to the impedance [Zg] of the GND line.

Fig. 29 Noise Source 

<img width=300, src="img/068-fig29-noise-source.png">

Fig. 30 shows the dependency of the noise voltage on the each parameter. 

Fig. 30 Dependency of the noise voltage on each parameter 

<img width=300, src="img/067-fig30-dependency-of-the-noise-voltage-on-each-parameter.png">

### II. Noise Protection 
To avoid the noise on the address bus during the system operation mentioned before, there are two solutions as follows.

The one method is to isolate the HD6303R from peripheral devices so that peripherals are not affected by the noise. The other is to reduce noise level to the extent of not affecting peripherals using analog method. 


#### 1. Noise Isolation 

Addresses should be latched at the negative edge of the AS signal or at the positive edge of the E signal. The 74LS373 is often used in this case. 

Figure Additional Latch

<img width=400, src="img/069-additional-latch.png">

#### 2. Noise Reduction 
As the noise level depends on each parameter such Cd,Vcc, Zg, the noise level can be reduced to the allowable level by con. trolling those analog parameters. 

#### a.  Transient Current Reduction 
1. Reduce the data bus load capacitance. If large load capacitance is expected, a bus buffer should be inserted. 
2. Lower the power supply voltage Vcc within specifi 
cation. 
3. Increase a time constant at transient state by inserting a resistor (100 ~ 2005) to Data Buses in series to keep noise level down.  Table 18 shows the relationship between a series resistor and noise level or a resistor and DC/AC characteristics. 

<img width=400, src="img/070-damping-registers.png">

Table 18. 

<img width=700, src="img/071-table18-noise-characteristics.png">

Fig. 31 shows an example of the dependency of the noise voltage on the load capacitance of the data bus.\*

<img width=400, src="img/072-fig31-load-capacitance-vs-noise.png">

\*Note: The value of series resistor should be carefully selected because it heavily depends on each parameter of actual application system. 

Fig. 32 shows the typical wave form of the noise. 

<img width=300, src="img/073-fig32-waveform-of-the-noise.png">

#### b. Reduction of GND line impedance 

1. Widen the GND line width on the PC board. 
2. Place the HD6303R close by power source. 
3. Insert a bypass capacitor between the Vcc line and the GND of the HD6303R. A tantalum capacitor (about 0.1uF) is effective on the reduction. 

Fig. 33 Layout of the HD6303R on the PC board 

<img width=500, src="img/074-fig33-layout-of-the-hd6303r.png">

## WARNING CONCERNING POWER START-UP 

RES must be held low for at least 20 ms when the power starts up. In this case, the internal reset function is not effective until the oscillation begins at power-on. The RES signal is input to the LSI in synchronism with the internal clock φ(shown in Figure 34.) 

RESは電源起動時に20ms以上Lowに保持する必要がある。この場合、電源投入時に発振が始まるまで内部リセット機能は有効になりません。RES 信号は内部クロックφに同期して LSI に入力される(図 34)。

Therefore, after power starts up, the LSI conditions such as its I/O ports and operating mode, are unstable. Fix the level of I/O ports by means of an external circuit to determine the level for system operation during the oscillator stabilization time. 

そのため、電源立ち上げ後、LSIのI/Oポートや動作モードなどの状態が不安定になります。I/Oポートのレベルを外部回路で固定し、発振器安定時間中のシステム動作レベルを決定する。

Figure 34 RES circuit 

<img width=400, src="img/075-fig34-res-circuit.png">

## WRITE-ONLY REGISTER 
CPUが書き込み専用レジスタを読み出す場合、書き込み専用レジスタの値に関係なく、読み出されるデータは常に\$FFとなる。従って、AIM、ADD、ROLのように、書き込み専用レジスタを読み込んで、その内容に対して算術演算や論理演算を行う命令を実行した場合、必ず\$FFのデータで算術演算や論理演算が行われるため、その結果には注意が必要です。特に、AIM、OIM、EIM命令でPORTのDDRビットを操作しないでください。

<div style="page-break-before:always"></div>

## NOTICE ON HD6303R 
HD6303RはHD6301 V1と同じダイです。オンチップマスクROMはマスクオプションにより無効にされています。そのため、HD6303Rではすべての動作モードが使用できるわけではありません。HD6301 V1と記載されている場合は、HD6303Rにも適用されます。

## NOTICE ON HD6303R1 
HD6303RはHD6303R1にバージョンアップしました。両者の差異については以下の表を参照ください。その他の特性は変わりません。

<div style="page-break-before:always"></div>

## DIFFERENCES BETWEEN HD6301V1, HD6303R,<br> HD6303R1, HD63P01M1, AND HD63701V0
<figure>
<img width=711, src="img/076-difference-between-several-chips.png">
</figure>
<figure>
</figure>
<figure>
<img width=703, src="img/077-difference-between-several-chips2.png">
</figure>
<figure>
<img width=710, src="img/078-difference-between-several-chips3.png">
</figure>
<figure>
<img width=719, src="img/079-difference-between-several-chips4.png">
</figure>

|Item|HD63P01M1|HD6301V1,HD6303R,<br>HD6303R1,HDR63701V0|
|--|--|--|
|AS<br>(Address<br>Strobe)|拡張多重モード(モード0,2,4,6)<br>では、ASはリセット中に1/2E<br>クロックサイクルの間ハイ<br>インピーダンス状態になる。|リセット中もASは正常に<br>機能する。
|SCI|フレーミングエラーが発生した<br>とき、受信データは受信シフト<br>レジスタから受信データレジスタ(RDR)<br>に転送されない。|フレーミングエラーが発生した<br>場合でも、受信シフトレジスタ<br>から受信データレジスタへの<br>転送は行われる。|

|Item|HD6301V|HD63701V0|
|--|--|--|
|RAM|RAM容量: 128バイト<br>Address: \$0080 - \$00FF|RAM容量: 196バイト<br>Address: \$0040 - \$00FF|
|Port<br>Reset|ポートのDDRはEクロックと同期<br>してリセットされる。電源投入<br>からクロック発振が開始するまで<br>の間(最大20ms)、I/Oの状態は<br>不定である。|ポートのDDRはEクロックと同期<br>しない。RESをLowにすることで、<br>CPUはハイインピーダンス状態に<br>なる。リセット解放とMCU内部<br>のリセットはEクロックと同期して<br>行われる。|
|Timer|電源電圧供給後、出力コンペア<br>レジスタの内容がフリー<br>ランニングカウンタの内容と一致<br>するまでは出力レベルは不定<br>(0または1)となる。出力レベル<br>レジスタはリセットによって<br>初期化されない。|出力レベルレジスタはリセットに<br>より0にリセットされます。
|Address<br>Delay<br>Time|1. tAD1とtAD2は動作周波数と<br>独立に決まる定数です。<br>HD63B01V(HD6301VのBバー<br>ジョン)の場合、0.1MHzから<br>2MHzまででtAD1とtAD2は最大<br>160nsです。<br>2. tADLは動作周波数に関係<br>します。(tADLは1/fに比例し、<br>f=動作周波数となる。)|tAD1、tAD2、tADLは動作周波数に<br>関係します(1/f.f動作周波数に比例<br>します)。従って、HD637B01Vが低い<br>動作周波数で動作した場合、tAD1、<br>LAD2、IADLは160ns以上となり<br>ます。<br>tAD1, tAD2, tADLは以下の式で<br>計算されます。<br>tAD(f MHz) = 250ns(1MHz) ×<br> 1/f (MHz)| 
|GND<br>Noise|各データ線の負荷容量とGNDイン<br>ピーダンスが大きい場合、MCUの<br>ライトサイクルでノイズが<br>アドレスバスに出現し、RAMへ<br>データが正しく書き込まれない<br>ことがあります。データバスがH<br>からLに遷移する際に大量の電流<br>がGNDインピーダンスに流れ<br>込む際に、GNDインピー<br>ダンスが大きくなることに<br>由来するものです。|ノイズはHD6303R1, HD63P01M1で<br>35%削減され、HD63700V0で<br>50%削減されています。

* HD6301Vは、HD63701V0とはチップ設計および製造プロセスが異なります。したがって、HD6301VとHD63701V0とは実際の仕様、マージンは異なる。自分のシステムにHD6301やHD63701V0を適用する前に、自分のシステムを注意深く調べてください。

