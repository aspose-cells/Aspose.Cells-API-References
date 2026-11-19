---
title: "ISmartMarkerCallBack"
second_title: "Aspose.Cells for Java API 参考"
description: "表示处理 smartmarker 的回调接口。"
type: docs
url: /zh/java/com.aspose.cells/ismartmarkercallback/
---
```
public interface ISmartMarkerCallBack
```

表示处理 smartmarker 的回调接口。
## 方法

| 方法 | 描述 |
| --- | --- |
| [process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName)](#process-int-int-int-java.lang.String-java.lang.String-) | 用于处理智能标记的回调。 |
### process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName) {#process-int-int-int-java.lang.String-java.lang.String-}
```
public abstract void process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName)
```


用于处理智能标记的回调。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetIndex | int | 工作表索引。 |
| rowIndex | int | 行索引。 |
| colIndex | int | 列索引。 |
| tableName | java.lang.String | 智能标记的表名。 |
| columnName | java.lang.String | 智能标记的表名。 |

