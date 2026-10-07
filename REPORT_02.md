# 第2回 Webエンジニアリング演習 レポート
## 学籍番号
4724219
## コンフリクトが発生した理由
 conflict-a⁠ と conflict-b⁠ の2つのブランチで、⁠README.md⁠ の同じ行に対してそれぞれ異なる変更を行ったため、Gitが自動で統合できず競合が発生した。
## 解決手順
ターミナルで ⁠git pull⁠ 等を行ってコンフリクトを発生させ、エディタで競合記号を削除して両方の意図をまとめた1行に修正したこと、その後 ⁠git add⁠ と ⁠git commit⁠ で解決結果を記録した
## 履歴
*   9d67468 (HEAD -> practice/conflict-b, origin/practice/conflict-b) Resolve README conflict
|\  
| *   f0c7175 (origin/main, origin/HEAD) Merge pull request #1 from 4724219/practice/conflict-a
| |\  
| | *   5e08e25 (origin/practice/conflict-a, practice/conflict-a) Merge branch 'main' of https://github.com/4724219/web-eng-report into practice/conflict-a
| | |\  
| | |/  
| |/|   
| | * 6fad6e1 Add report 01
| | * bc5549f Update goal in conflict A
* | | 439341b Update goal in conflict B
* | | aa7b07c Update goal in conflict B
* | | 3f86b28 Update goal in conflict A
|/ /  
* / 507c183 (origin/feature/add-readme) Add REPORT_01.md
|/  
* 23dfc25 Add index.html
* f1f3d2a Create devcontainer.json
* 4062992 Initial commit