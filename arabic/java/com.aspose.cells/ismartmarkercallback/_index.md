---
title: "ISmartMarkerCallBack"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل واجهة الاستدعاء للمعالجة الذكية للعلامات."
type: docs
url: /ar/java/com.aspose.cells/ismartmarkercallback/
---
```
public interface ISmartMarkerCallBack
```

يمثل واجهة الاستدعاء للمعالجة الذكية للعلامات.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName)](#process-int-int-int-java.lang.String-java.lang.String-) | استدعاء رد لمعالجة علامة ذكية. |
### process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName) {#process-int-int-int-java.lang.String-java.lang.String-}
```
public abstract void process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName)
```


استدعاء رد لمعالجة علامة ذكية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetIndex | int | فهرس الورقة. |
| rowIndex | int | The row index. |
| colIndex | int | The column index. |
| tableName | java.lang.String | اسم الجدول للعلامة الذكية. |
| columnName | java.lang.String | اسم الجدول للعلامة الذكية. |

