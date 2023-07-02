# ArduinoUnoR4_kw1281_Test
下記ALEXANDER GRAU様のサイトにて公開されているコードをIDE標準のSoftwareSerialで動くようにしつつ、ArduinoUnoR4で動くように各所を修正し、シリアルで結果を見ることだけに機能を絞ったスケッチです。<br>
主にArduinoUnoR4でKW1281を使用した通信、特にdigitalwriteを使用して無理やり5baud初期化を行う処理がR4でも正常に動くかを検証するために使用しました。<br>
http://grauonline.de/wordpress/?p=74

変更箇所は下記リポジトリ内の変更と併せて、UnoR4ではSoftwareSerialの宣言やら初期化の記述がR3と微妙に異なるようなので、そこをR4用に修正しました。<br>
R4ではobd.write(data);の前にdelay(5);を入れなくても問題なく通信できるようです。<br>
https://github.com/accept/arduino_kw1281_softwareserial<br>

同じくベンチECUでしかテストしていないので実車にて使用する際は自己責任でお願いします。<br>
ALEXANDER GRAU様に謝辞を申し上げます。
