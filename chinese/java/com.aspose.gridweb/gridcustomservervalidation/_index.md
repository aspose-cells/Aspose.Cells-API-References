---
title: "GridCustomServerValidation"
second_title: "Aspose.Cells for Java API 参考"
description: "当使用服务器端验证时，需要实现的接口。"
type: docs
url: /zh/java/com.aspose.gridweb/gridcustomservervalidation/
---
```
public interface GridCustomServerValidation
```

在使用服务器端验证时需要实现的接口。CustomServerFunction。
## 方法

| 方法 | 描述 |
| --- | --- |
| [validate(GridWorksheet sheet, int row, int col, String value)](#validate-com.aspose.gridweb.GridWorksheet-int-int-java.lang.String-) | **备注** |
### validate(GridWorksheet sheet, int row, int col, String value) {#validate-com.aspose.gridweb.GridWorksheet-int-int-java.lang.String-}
```
public abstract String validate(GridWorksheet sheet, int row, int col, String value)
```


**Remarks**

如果返回 string.empty，则验证通过；否则可以返回任何相关信息，该信息将在 ClientCallback 函数中处理。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheet | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) | GridWorksheet |
| 行 | int | 单元格的行索引 |
| 列 | int | 单元格的列索引 |
| 值 | java.lang.String | 用于验证的值 |

**Returns:**
java.lang.String - 基于字符串的结果值
