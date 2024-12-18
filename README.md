# OANC37k - 日本の英語学習者向け英単語リスト

このリポジトリは、Open American National Corpus (OANC) を基に作成された、日本の英語学習者向けの英単語リストです。

37000語の語彙を例文やその和訳、読み上げ音声つきで収録しています。

## 特徴
- **ライセンス**: ODC-PDDL
- **対象**: 日本の英語学習者
- **語義や例文**: 部分的に AI (Gemini) を用いて生成
- **注意事項**: これを用いた結果の不利益には責任を持ちません
- **データ形式**:
  - **CSV形式**: 英単語リスト
  - **MP3形式**: 英語例文とその和訳の音声ファイル

## データ構成
### mp3の形式
- `Example` フォルダ: 英語例文の読み上げ音声
- `Example_JP` フォルダ: 例文和訳の読み上げ音声

これらはStyle-Bert-Vits2の以下モデルを利用して生成されました。
https://huggingface.co/kokuren/RinneElu

### CSVの形式
以下の形式でデータを提供しています。
```csv
"word","CEFR","Japanese","Example","Example_JP"
"know","A1","知っている","I know the answer.","私は答えを知っている。"
```

- `word`: 英単語
- `CEFR`: 難易度ランク
- `Japanese`: 日本語訳
- `Example`: 英語例文
- `Example_JP`: 例文和訳
