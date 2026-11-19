---
title: "IFilePathProvider"
second_title: "Aspose.Cells for Java API 参考"
description: "表示导出文件路径提供程序。"
type: docs
url: /zh/java/com.aspose.cells/ifilepathprovider/
---
```
public interface IFilePathProvider
```

表示导出文件路径提供程序。
## 方法

| 方法 | 描述 |
| --- | --- |
| [getFullName(String sheetName)](#getFullName-java.lang.String-) | 在单独将工作表导出为 HTML 时，根据工作表名称获取文件的完整路径。 |
### getFullName(String sheetName) {#getFullName-java.lang.String-}
```
public abstract String getFullName(String sheetName)
```


在单独将工作表导出为 HTML 时，根据工作表名称获取文件的完整路径。这样可以正确导出工作表之间的引用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetName | java.lang.String | 工作表名称 |

**Returns:**
java.lang.String - 文件的完整路径
