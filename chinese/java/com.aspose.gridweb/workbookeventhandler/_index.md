---
title: "WorkbookEventHandler"
second_title: "Aspose.Cells for Java API 参考"
description: "表示用于处理工作簿事件的接口。"
type: docs
url: /zh/java/com.aspose.gridweb/workbookeventhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface WorkbookEventHandler extends Serializable
```

表示用于处理工作簿事件的接口。
## 方法

| 方法 | 描述 |
| --- | --- |
| [handleCellEvent(Object sender, CellEventArgs e)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-) | 处理相关的单元格事件。 |
### handleCellEvent(Object sender, CellEventArgs e) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-}
```
public abstract void handleCellEvent(Object sender, CellEventArgs e)
```


处理相关的单元格事件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 发送者 | java.lang.Object | 事件的来源。 |
| e | [CellEventArgs](../../com.aspose.gridweb/celleventargs) | 事件参数。 |

