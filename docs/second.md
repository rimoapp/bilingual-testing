## 自動話者分離
自動話者分離（横断話者分離）とは、予め話者のEmbeddingを計算しておき、新しいNoteに対してReference（ここがこの人の発話という人間のアノテーション）無しに話者分離する機能のこと。

## rimoで動いている設定
自動話者分離は以下の3つの機能の組み合わせによって成立している。

- Speaker Embeddingの事前計算
- Noteアップロード時のSpeaker Extraction
- Noteアップロード時のDiarization

### Speaker Embeddingの事前計算
rimo上にあるNoteの中で、人間が話者を付けたアノテーションから、その話者（Speaker）のEmbeddingを計算する。
これはcronで実行され、その時点でアノテーションの更新のあるNotesをデータとして1日1回実行される。
