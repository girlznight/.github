# 📝 YellowMemo.
### [Branch 전략 - 꼭 보기!!!](https://github.com/girlznight/Project-GirzDay-react-repo/blob/main/README.md)

[UIシナリオ / UI Scenario](https://www.figma.com/design/bHP3cXgSJ24emyrV1yNXRT/Untitled?node-id=0-1&t=94VpRgeA6CHY3eCb-1)


<img alt="Image" src="https://github.com/user-attachments/assets/d91eb918-1423-4869-a666-5c2476aa4e3e" width="200" height="200"/>

### コミットルール / Commit Rule : [Gitmoji](https://gitmoji.dev/)

```bash
npm i -g gitmoji-cli     
gitmoji -c
```

### 채워 나가야 할 부분 ⬇️
  
## 🔗 リポジトリ / Repositories

- [PROJECT REPO](https://github.com/girlznight/Project-GirzDay-react-repo)
- [기타 관련 레포 / Others](#)

---

## 📖 プロジェクト紹介 / Project Overview

**日本語**  
小さくても、大切なアイデア。
YellowMemo. プロジェクトは、ある日、机の上に置かれた一枚の黄色い付箋から始まりました。
ふと浮かんだ考えや、通り過ぎるアイデアを、どこかに残して共有したいと思ったのです。
このアプリは、複雑な機能ではなく、「記録すること」そのものに焦点を当てて作られました。
ReactとJSON Serverで開発されており、
メモを書いて、直して、消す——そのすべての流れが、自然でシンプルになるように設計されています。
データ構造はシンプルですが、
その中には、「考えを大切にしたい」という小さな哲学が込められています。

**English**  
Small, but essential ideas.
The YellowMemo. project began one day with a single yellow sticky note left on a desk.
We wanted to keep and share thoughts that popped into our minds—ideas that come and go in an instant.
This app was created not to focus on complex features, but to simply honor the act of recording ideas.
Built with React and a JSON server,
It’s designed so that writing, editing, and deleting a memo flows naturally and simply.
Though the data structure is minimal,
It carries a quiet philosophy: to respect every thought, no matter how small.

---

## 🌟 主な機能 / Key Features

- **機能1 / Feature 1**: 日本語の説明 / Description in English  
- **機能2 / Feature 2**: 日本語の説明 / Description in English  
- **機能3 / Feature 3**: 日本語の説明 / Description in English  
（必要に応じて追加）

---

## 🛠 技術スタック / Tech Stack

- **フロントエンド / Frontend**: React.js 
- **バックエンド / Backend**: JSON server

---

## 📚 主なAPI・DB設計 / Main API & DB Design

- **エンドポイント分類 / Endpoint Categories**  
  - `GET /api/xxx`  
  - `POST /api/xxx`  
  - `PATCH /api/xxx`
- **DBテーブル / Database Structure**:  

<details>
<summary>user</summary>

| Field     | Type   | Description                   |
|-----------|--------|-------------------------------|
| id        | number | Unique user ID                |
| loginId   | string | Login ID                      |
| profile   | string | Profile image (Base64 format) |

</details>

<details>
<summary>auth</summary>

| Field     | Type   | Description                       |
|-----------|--------|-----------------------------------|
| id        | number | Unique auth ID                    |
| password  | string | Password                          |
| userId    | number | Linked user ID (foreign key)      |

</details>

<details>
<summary>post</summary>

| Field     | Type   | Description                       |
|-----------|--------|-----------------------------------|
| id        | number | Unique post ID                    |
| userId    | number | Author's user ID (foreign key)    |

</details>

<details>
<summary>textbox</summary>

| Field     | Type   | Description                       |
|-----------|--------|-----------------------------------|
| id        | number | Unique textbox ID                 |
| x         | number | X position                        |
| y         | number | Y position                        |
| postId    | number | Parent post ID (foreign key)      |
| content   | string | Text content                      |

</details>

<details>
<summary>postit</summary>

| Field     | Type   | Description                       |
|-----------|--------|-----------------------------------|
| id        | number | Unique post-it ID                 |
| x         | number | X position                        |
| y         | number | Y position                        |
| z         | number | Z-index (stacking order)          |
| postId    | number | Parent post ID (foreign key)      |
| content   | string | Memo content                      |
| userId    | number | Author's user ID (foreign key)    |

</details>

<details>
<summary>image</summary>

| Field     | Type   | Description                       |
|-----------|--------|-----------------------------------|
| id        | number | Unique image ID                   |
| x         | number | X position                        |
| y         | number | Y position                        |
| z         | number | Z-index (stacking order)          |
| postId    | number | Parent post ID (foreign key)      |
| src       | string | Image source (Base64 format)      |
| userId    | number | Uploader's user ID (foreign key)  |

</details>

---

## 🎯 プロジェクトの目的 / Project Purpose

**日本語:**  
このプロジェクトを通して達成したい目的・意図を記入します。

**English:**  
Describe the purpose and goals of the project in English.

---

## 📎 参考 / References

- [API仕様書 / API Specification](#)
- [DBテーブル設計 / DB Table Design](#)
- [UIシナリオ / UI Scenario](https://www.figma.com/design/bHP3cXgSJ24emyrV1yNXRT/Untitled?node-id=0-1&t=94VpRgeA6CHY3eCb-1)

---
