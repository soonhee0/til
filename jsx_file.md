## JSファイルとJSXファイルの違いについて
-JSXはJavascriptの拡張構文であるため、通常のJavaScriptファイル（拡張子が.js）とは異なります。
-JSXファイルの拡張子は.jxsであり、通常のJavaScriptファイルとは区別される
-JSXファイルはreactコンポーネントを定義するために使用される
例 JSXファイルの例
```const Welcome = (props) => {
  return <h1>Hello, {props.name}</h1>;
}```

これを通常の.jsファイルを使用すると
```function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}```

##JSXの基本的な書き方とソースコード例
###一つのルート要素を使う
Reactのコンポーネントは、常に1つのルート要素で囲まれている必要がある
例
```const App = () => {
  return (
    <div>
      <h1>タイトル</h1>
      <p>説明文</p>
    </div>
  );```
};
この例では、<div>がルート要素で、<h1>と<p>がその中に含まれている

###classではなくclassNameを使う
JSXでは、HTMLのclass属性の代わりにclassNameを使用する
```const MyComponent = () => {
  return <div className="myClass">こんにちは、世界！</div>;
};```
このコードでは、div要素にclassName属性を使用している

###コメントは{/ /}で囲む
###属性値は””で囲む
```const MyComponent = () => {
  return <a href="https://example.com">リンク</a>;
};```
この例では、a要素のhref属性にURLをダブルクオートで囲んで指定している

###すべてのタグを閉じる
例
```const MyComponent = () => {
  return (
    <div>
      <img src="image.jpg" alt="説明" />
      <input type="text" />
    </div>
  );
};```
この例では、imgタグとinputタグが自己終了タグとして適切に閉じられている

###複数の要素を1つで囲む
複数の要素を返す場合、それらを<>（フラグメント）で囲むか、別の要素でラップする
```const MyComponent = () => {
  return (
    <>
      <h1>見出し</h1>
      <p>説明文</p>
    </>
  );
};```
