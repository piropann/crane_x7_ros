使用方法

動作確認は[README.md](../crane_x7_examples/README.md)参照

実機の場合

①PCにマニピュレータをUSB経由で接続し、次のコマンドを入力

	$ sudo chmod 777/dexv/tty/USB0

	$ roslaunch crane_x7_control crane_x7_control.launch

②プログラムを実行するため、以下のコマンドを入力

	$ rosrun crane_x7_examples crane_x7_pick_and_place.py

プログラムを実行した際の成功動画

https://youtu.be/m2CDxoViR-k


シミュレータを使う場合

①PCでシミュレータを起動するため、以下のコマンドを入力

	$ roslaunch crane_x7_gazebo crane_x7_with_table launch

②プログラムを実行するため、以下のコマンドを入力

	$ rosrun crane_x7_examples crane_x7_pick_and_place.py


※このプログラムでは表示されている物体はつかまないため、動きだけの確認である。また、Move itで動きは計算しているため同じ動きにならない可能性があります。
