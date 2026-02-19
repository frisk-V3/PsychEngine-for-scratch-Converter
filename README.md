# PsychEngine-for-scratch-Converter

Psych Engine の譜面 JSON を、Scratch や独自エンジンで扱いやすい  
**TXT フォーマットに変換する Web ツール**です。

ブラウザ上で動作し、インストール不要。  
JSON を選ぶだけで自動変換できます。

---

##  特徴 / Features

- Psych Engine の JSON を TXT に変換
- `song.notes` / `notes` どちらの形式にも対応
- ロングノーツ・特殊ノーツも処理
- ファイル名を自動で引き継ぎ
- ログ表示で変換状況がわかる
- 完全クライアントサイド（安全）

---

##  対応フォーマット

### ▼ 入力（Psych Engine JSON）
```json
[ time(ms), lane, length(ms), type ]
▼ 出力
例：
{0.387} :{2} :{} :{0}
よくあるエラーと原因
JSON の構造が通常と異なる

sectionNotes が空または存在しない

ノーツ配列が [time, lane, length] の3つだけ

JSON にコメントが含まれている

BOM 付き JSON

これらは今後のアップデートで対応予定。
