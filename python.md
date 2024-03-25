### クラスの基本構文
   class ClassName():
    def __init__(self, ):
         hogehoge

- 関数では「def」で定義
- classから始まる構文の内部に「__init__」という関数が定義されている　
　これはコンストラクタと言ってクラスの中で重要な機能

### コンストラクタ
- 特別なメソッドの定義方法
-  上のコードでは「__init__」という名前の部分
　　インスタンスを作成する際に重要な処理を含むもの
-  どのように生成するか、どのようなデータを持たせるかなど、といった情報を定義するのに必要なメソッド
-  第一引数にself　これは必須

例：
class MyClass():
    def __init__(self, message):
        self.value = message
 
myinstance = MyClass("Hello!")
print(myinstance.value)
実行結果
Hello!

このインスタンスのデータにmessageを追加したいので、valueという属性（アトリビュート）を追加し、第二引数のmessageを代入
インスタンスを生成するために、インスタンスを代入する変数名 = クラス名(引数)と、呼び出す

### メソッドとは
- クラス内に定義された関数
- メソッドは定義されたクラスからしか呼び出せない
例
class Example():
 
    def __init__(self, a,b,c):
        self.num1 = a
        self.num2 = b
        self.num3 = c
 
    def print_tot(self):
        tot = self.num1+self.num2+self.num3
        print(tot)
 
myinstance = Example(1,2,3)
myinstance.print_tot()
- Exampleはコンストラクタと　print_totというメソッドを含む
- コンストラクタでは引数に指定したa、b、cを属性num1、num2、num3に代入
  print_totは生成したインスタンスが持つ３つの合計を計算し出力する
