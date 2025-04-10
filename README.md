# テーブル設計

## users テーブル

| Column             | Type   | Options     |
| ------------------ | ------ | ----------- |
| email              | string | NOT NULL, ユニーク制約 |
| encrypted_password | string | NOT NULL |
| name               | string | NOT NULL |
| profile            | text   | NOT NULL |
| occupation         | text   | NOT NULL |
| position           | text   | NOT NULL |


### Association

- 
- 
- 

## prototypesテーブル

| Column       | Type       | Options           |
| ------------ | ---------- | ----------------- |
| name         | string     | NOT NULL          |
| catch_copy   | text       | NOT NULL          |
| concept      | text       | NOT NULL          |
| user         | references | NOT NULL, 外部キー |

### Association

- 
- 
- 

## commentsテーブル

| Column       | Type       | Options           |
| ------------ | ---------- | ----------------- |
| content      | text       | NOT NULL, 外部キー |
| prototype    | references | NOT NULL, 外部キー |
| user         | references | NOT NULL, 外部キー |

### Association

- 
- 
