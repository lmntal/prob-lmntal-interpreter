# Prob LMNtal intepreter

確率モデルを表現した LMNtal モデルの状態空間構築を行うインタプリタです。
LMNtal のメタインタプリタをベースにしています。
`prob_interpreter.use` によりモジュールを呼び出すことで使用できます。
使用例は `examples` ディレクトリを参照してください。

## 事前準備

- SLIM (LMNtal 実行処理系)

## 使い方

1. LMNtal プログラム内で `prob_interpreter.use` によりモジュールを呼び出します．
2. SLIM のオプション `-I` で `prob_interpreter` モジュールが定義されたファイルのあるディレクトリを指定します．
3. slim で通常実行を行います．(e.g. `slim --use-builtin-rule path/to/module examples/die.lmn`)
4. [prob-lmntal-translator](https://github.com/lmntal/prob-lmntal-translator) を使用して，実行結果から確率モデル検査ツール [PRISM](https://www.prismmodelchecker.org/) の入力形式 Explicit モデルへの変換が行えます．
