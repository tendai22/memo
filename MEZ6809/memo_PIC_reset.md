# PICプログラミング時の挙動

A6,A7がICSP端子と共用しているので、SNAP書き込み時にA6,A7をHi-Zにしておきたい。
SNAPは何度かMCLRを上げ下げして、PICにリセットを掛けている。

リセット解除後の最初の設定でMPUをうまく走らせて、確実にA6,A7をHi-Zにさせるために、

* SNAP書き込み時にリセットは何度、どのタイミングでかかるのか?
* 書き込みに先立つリセット解除で、PICプログラムはどの程度の時間処理できるのか?
