---
title: "ISmartMarkerCallBack"
second_title: "Aspose.Cells for Java API Referansı"
description: "Smartmarker işleme geri çağırma arayüzünü temsil eder."
type: docs
url: /tr/java/com.aspose.cells/ismartmarkercallback/
---
```
public interface ISmartMarkerCallBack
```

Smartmarker işleme geri çağırma arayüzünü temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName)](#process-int-int-int-java.lang.String-java.lang.String-) | Akıllı işaretleyiciyi işlemek için geri çağırma. |
### process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName) {#process-int-int-int-java.lang.String-java.lang.String-}
```
public abstract void process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName)
```


Akıllı işaretleyiciyi işlemek için geri çağırma.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetIndex | int | Sayfa indeksi. |
| rowIndex | int | Satır indeksi. |
| colIndex | int | Sütun indeksi. |
| tableName | java.lang.String | Akıllı işaretleyicinin tablo adı. |
| columnName | java.lang.String | Akıllı işaretleyicinin tablo adı. |

