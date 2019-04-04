~~~
①メモに１〜９のランダムな数字を改行を入れて１文字ずつ書く
②そのファイルをプログラムで読み込む
③コマンドラインからパラメータを受け取り、数字を昇順・降順に並び替える

今普通の配列を昇順降順に並び替えることには成功しました。
#include <stdio.h>
  
int main(void)
{
    int b;
    int a[9] = {1,3,5,7,9,2,4,6,8};
    for(int i = 0;i < 9;i++){
		    printf("%d",a[i]);
	}
	for(int j = 0;j < 9;j++){
	    printf("\n");
	    for(int n = 0;n < 9;n++){
	        if(a[j] < a[n]){
	            b = a[j];
	            a[j] = a[n];
	            a[n] = b;
	        }
	        printf("%d",a[n]);
	    }
	}
	return 0;
}
~~~
