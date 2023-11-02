# zuka6

# 課題１
``` mermaid
sequenceDiagram

actor s as 学生
actor r as 受付
participant db as データベース
s->>+ r :図書借り出し依頼
s->> r :図書を提出
s->> r :学生証を提出
r->>+ db :登録依頼
db-->>- r :登録完了
r-->> s:学生証を返す
r-->>- s :図書を渡す
```
# 課題２
``` mermaid
sequenceDiagram

actor s as 学生
actor r as 受付
participant db as データベース
s->>+ r :図書借り出し依頼
s->> r :学生証を提出
r->>+ db :登録依頼
db-->>- r :登録完了
r-->> s:学生証を返す
s->> r :図書を提出
r->>+ db :登録依頼
db-->>- r :登録完了
r-->>- s :図書を渡す
```
