# テーブル設計

## usersテーブル
| Column            |  Type  |  Options   |
| ----------------- | ------ | ---------- |
| emails            | string | null:false |
| encrypted         | string | null:false |
| name              | string | null:false |
| profile           | text   | null:false |
| occupation        | text   | null:false |
| position          | text   | null:false |


## prototypesテーブル
| Column            |  Type  |  Options   |
| ----------------- | ------ | ---------- |
| title             | string | null:false |
| catch_copy        | text   | null:false |
| concept           | text   | null:false |
| user              | referenccexs| null:false |

## commentsテーブル
| Column            |  Type  |  Options   |
| ----------------- | ------ | ---------- |
| content           | text   | null:false |
| prototype         | references | null:false |
| user              | references | null:false |