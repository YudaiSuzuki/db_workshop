# コーディング規約

読みやすくするため、インデントを適宜行う。  
インデント幅は2とする。また、インデントは半角スペースのみを使用し、タブは使用しない。 
（環境によりタブ幅が異なるため）  

```sql
SELECT
  *
FROM
  table
;
```

予約語で改行を入れ、結合とANDはインデントを下げて記述する。  

```sql
SELECT
  t1.id,
  COUNT(*)
FROM
  table1 t1
    INNER JOIN
  table2 t2
    ON t1.id = t2.table1_id
WHERE
      t1.created_at >= '2013-04-24'
  AND t1.created_at <= '2013-04-30'
  AND t2.type = 2
GROUP BY
  t1.id
;
```

カンマは単語の末尾に書く。  
このスタイルで記述するプログラマーが多いため。  

```sql
SELECT
  col1,
  col2,
  col3,
  col4,
  col5
FROM
  table
;
```

