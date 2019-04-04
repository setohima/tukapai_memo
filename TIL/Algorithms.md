
## Luhnアルゴリズム

Luhnアルゴリズムはチェックディジットの一種で、クレジットカードや、IMEI番号などの数字が正しいかを確認するためのアルゴリズム

最終的に10で割り切れるかを確認するためのものなので”MOD-10アルゴリズム”とも呼ばれている。

アルゴリズムの手順は以下

1. 右端のチェックディジットを1番目として、偶数番目の桁を2倍にする。
2. 2倍にしていない桁も含め、各数字の総和を求める（2倍にした桁が2桁になった場合は、それぞれを別々の数字として加える）。
3. この総和の下1桁が0なら（つまり、10で割り切れる場合）、この番号はLuhnアルゴリズムでは正しく、そうでない場合は正しくない。

TODO:Rubyで動くものを書いてみる