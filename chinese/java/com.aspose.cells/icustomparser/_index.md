---
title: "ICustomParser"
second_title: "Aspose.Cells for Java API 参考"
description: "允许用户添加自定义值解析器，以将字符串值解析为其他适当的单元格值对象。"
type: docs
url: /zh/java/com.aspose.cells/icustomparser/
---
```
public interface ICustomParser
```

允许用户添加自定义值解析器，以将字符串值解析为其他适当的单元格值对象。
## 方法

| 方法 | 描述 |
| --- | --- |
| [getFormat()](#getFormat--) | 获取上一次调用 [parseObject(String)](../../com.aspose.cells/icustomparser\#parseObject-String-) 所得到的已解析值对应的格式模式。 |
| [parseObject(String value)](#parseObject-java.lang.String-) | 将给定的字符串解析为适当的值对象。 |
### getFormat() {#getFormat--}
```
public abstract String getFormat()
```


获取上一次调用 [parseObject(String)](../../com.aspose.cells/icustomparser\#parseObject-String-) 所得到的已解析值对应的格式模式。

**Remarks**

返回的格式模式可用于格式化相应的单元格（将单元格的 Style 设置为 Custom）。

**Returns:**
java.lang.String
### parseObject(String value) {#parseObject-java.lang.String-}
```
public abstract Object parseObject(String value)
```


将给定的字符串解析为适当的值对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 待解析的字符串值 |

**Returns:**
java.lang.Object - 从给定字符串解析得到的值对象。如果给定字符串无法解析为适当的值对象，则返回 null。
