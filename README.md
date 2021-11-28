# snipet

## DB

### 重複値と件数洗い出し

```SQL
SELECT
  重複値,
  COUNT(重複値)
FROM
  tableName
GROUP BY
  重複値
HAVING COUNT(重複値) > 1
```

### SQLコマンドラインから結果をファイル出力

```SQL
--SPOOL パス¥ファイル名
--  SELECT文など
--  実行
--SPOOL OFF
--例：
SPOOL desktop¥test.csv
SELECT * FROM PERSONAL
SPOOL OFF
```

## 正規表現

