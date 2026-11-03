# 16-haiku-seasonword-picker — 季語ピッカー（俳句支援）

## 概要
季節（新年/春/夏/秋/冬）タブで季語を切り替え、ランダム表示した5件から選んで俳句を作成・保存するクリエイティブサポートツール。

## 機能
- 季節タブ（新年/春/夏/秋/冬）切り替え
- 各季節20件の季語を内蔵
- ランダム表示ボタンで5件をシャッフル
- 季語クリックで俳句作成エリアに自動挿入
- 俳句をlocalStorageに保存（最大30件）・削除

## 技術仕様
- 静的SPA / Tailwind CDN
- localStorage キー: `haiku_list`
- XSS対策: escapeHtml() 使用
- a11y: aria-label / aria-selected / tabindex 対応
