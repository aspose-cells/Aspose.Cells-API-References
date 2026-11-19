---
title: "CellEventStringHandler"
second_title: "Aspose.Cells for Java API 参考"
description: "表示用于处理单元格事件的接口。"
type: docs
url: /zh/java/com.aspose.gridweb/celleventstringhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CellEventStringHandler extends Serializable
```

表示用于处理单元格事件的接口。
## 方法

| 方法 | 描述 |
| --- | --- |
| [handleCellEvent(Object sender, CellEventArgs e)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-) | 处理相关的单元格事件。 |
### handleCellEvent(Object sender, CellEventArgs e) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-}
```
public abstract String handleCellEvent(Object sender, CellEventArgs e)
```


处理相关的单元格事件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 发送者 | java.lang.Object | 事件的源网格。 |
| e | [CellEventArgs](../../com.aspose.gridweb/celleventargs) | 事件参数。e.Cell 是触发事件的单元格。e.Argument 包含事件的参数。 |

**Returns:**
java.lang.String - 字符串值
