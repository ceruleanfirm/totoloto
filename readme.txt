
Mon algorithme de randomisation de la complémentaire en image ...

int=2
seed=$$
while true ; do
	nb=$((RANDOM+1))
	echo "RANDOM = $nb"
	echo "seed = $seed"
	res=$(( $nb*$int%$seed))
	echo "Result ==> $nb x $int % $seed = $res"
	[[ $res -ge 1 && $res -lt 13 ]] && break
	((int++))
	((seed++))
done



RANDOM = 28765
seed = 13215
Result ==> 28765 x 2 % 13215 = 4670
RANDOM = 12129
seed = 13216
Result ==> 12129 x 3 % 13216 = 9955
RANDOM = 29304
seed = 13217
Result ==> 29304 x 4 % 13217 = 11480
RANDOM = 31472
seed = 13218
Result ==> 31472 x 5 % 13218 = 11962
RANDOM = 1858
seed = 13219
Result ==> 1858 x 6 % 13219 = 11148
RANDOM = 29084
seed = 13220
Result ==> 29084 x 7 % 13220 = 5288
RANDOM = 11578
seed = 13221
Result ==> 11578 x 8 % 13221 = 77
RANDOM = 12914
...
RANDOM = 26887
seed = 14295
Result ==> 26887 x 1082 % 14295 = 1409
RANDOM = 16889
seed = 14296
Result ==> 16889 x 1083 % 14296 = 6203
RANDOM = 5548
seed = 14297
Result ==> 5548 x 1084 % 14297 = 9292
RANDOM = 15583
seed = 14298
Result ==> 15583 x 1085 % 14298 = 7319
RANDOM = 11772
seed = 14299
Result ==> 11772 x 1086 % 14299 = 1086
RANDOM = 29653
seed = 14300
Result ==> 29653 x 1087 % 14300 = 611
RANDOM = 3245
seed = 14301
Result ==> 3245 x 1088 % 14301 = 12514
RANDOM = 9863
seed = 14302
Result ==> 9863 x 1089 % 14302 = 5
