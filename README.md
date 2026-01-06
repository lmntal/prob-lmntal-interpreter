# Prob LMNtal intepreter

確率モデルを表現した LMNtal モデルの状態空間構築を行うインタプリタです。
LMNtal のメタインタプリタをベースにしています。
`prob_interpreter.use` によりモジュールを呼び出すことで使用できます。
使用例は `examples` ディレクトリを参照してください。

## 事前準備

- SLIM (LMNtal 実行処理系)

## 使い方

1. SLIM のオプション `-I` で `prob_interpreter` モジュールが定義されたファイルのあるディレクトリを指定します．
2. LMNtal プログラム内で `prob_interpreter.use` によりモジュールを呼び出します．