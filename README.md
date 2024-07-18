# 制作物No.1　三目並べ
## 遊び方
プログラムを実行すると3×3のボードが表示されるので、プレイヤーは交互にマスをクリックし「x」と「o」を配置していきます。  
先に同じマークを3つ並べたプレイヤーの勝利となります。  
勝敗が決まると結果が表示され、「ok」を押すことで新たなボードが作成され、ゲームを再開することができます。
## ソースコードの説明
__init__()によってゲームの初期化を行い、プレイヤーをXに設定し、ゲームの盤面を作成します。  
create_board()によってGUIを利用するゲームボードを作成します。ゲームボードは3×3のボタンとなっており、各ボタンがクリックされたときにclick()が呼び出されます。  
click()は、x,oを交互にゲームボードに入力していき、ゲームボードの状態を更新したときに勝敗を決定します。  
check_winner(), check_draw()によって勝利条件を満たすプレイヤーを決めます。  
reset_board()によって、ゲームが終了するとゲームボードがリセットされ、プレイヤーxからゲームが始まります。
