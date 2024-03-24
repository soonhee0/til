### クラスの基本構文
   class ClassName():
    def __init__(self, ):
         hogehoge

- 関数では「def」で定義
- classから始まる構文の内部に「__init__」という関数が定義されている　
　これはコンストラクタと言ってクラスの中で重要な機能

### コンストラクタ
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
