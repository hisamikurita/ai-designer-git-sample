# 🌱 AI時代のデザイナーのためのGit・GitHub入門 🌱

Claude Code や Codex や Figma Make を使って、実際に動くプロトタイプを爆速で作り上げていく時代、**AIツールの登場でデザイナーがコードを書く場面は確実に増えています。**

「コミットする」「プルする」「ブランチを切る」といった**操作自体は、AIに指示すれば簡単にできてしまいます**。このドキュメントでは `git add` のようなコマンドはあえて扱いません。それよりも、**Gitの概念を理解すること**に集中してもらえたらと思っています。概念さえわかれば、チーム開発への入りやすさがぐっと変わるはずです。

はじめます！

<img width="1280" height="640" alt="figmadetukutta" src="https://github.com/user-attachments/assets/0de27c35-cfa5-4634-a694-c426b6049908" />

# 概念編

## GitとGitHubは別物

まず最初に、混同されやすいこの2つを整理しましょう。

| | Git | GitHub |
|---|---|---|
| **何？** | 変更履歴を管理する仕組み（ソフトウェア） | Gitの履歴をオンラインで共有できるサービス |
| **誰が作った？** | Linus Torvalds（個人） | Microsoft傘下の企業 |
| **場所** | 自分のPC上で動く | インターネット上（クラウド） |
| **例え** | 日記帳そのもの | 日記帳を預けて共有できる図書館 |

**Gitが土台の技術**で、**GitHubはそれを活かしたWebサービス**です。
GitはGitHubなしでも使えますが、チームで共同作業するためにGitHubを組み合わせるのが一般的です。

<img width="1280" height="640" alt="figmadetukutta02" src="https://github.com/user-attachments/assets/dd65ef5f-367a-473d-8421-5743143801b7" />

## Gitって何？

Gitとはファイルの変更履歴を管理するツールです。デザイナーにとって身近な例で言うと…

```
logo_v1.png
↓
logo_v2.png
↓
logo_v2_final.png
↓
logo_v2_final_本当に最終.png
```
こうなりがちなファイル管理をGitを使うとスッキリ解決できます。
ファイル名を変えなくても「**いつ・誰が・何を変えたか**」を記録してくれます。

<img width="1280" height="640" alt="figmadetukutta03" src="https://github.com/user-attachments/assets/1c54acdf-70f9-4067-bac9-ab4f85194d0b" />

また、複数人で同じプロジェクトを触るときにも力を発揮します。

Figmaでは複数人が同じファイルをリアルタイムで編集できますが、コードファイルはそうはいきません。Gitを使うことで、それぞれがローカルで作業した変更を後からひとつにまとめることができます。

たとえば、あなたがヘッダーを、Aさんがカードコンポーネントを、Bさんがフッターをそれぞれ別々に作業していても、Gitが自動でひとつに統合してくれます。Figmaの共同編集を、コードファイルで実現するイメージです。

<img width="1280" height="640" alt="figmadetukutta13" src="https://github.com/user-attachments/assets/cbac3509-a281-43b6-a05c-8ed92525bc96" />
