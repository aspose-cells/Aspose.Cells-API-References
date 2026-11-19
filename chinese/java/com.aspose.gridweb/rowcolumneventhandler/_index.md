---
title: "RowColumnEventHandler"
second_title: "Aspose.Cells for Java API 参考"
description: "表示用于处理行/列事件的接口。"
type: docs
url: /zh/java/com.aspose.gridweb/rowcolumneventhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface RowColumnEventHandler extends Serializable
```

表示用于处理行/列事件的接口。
## 方法

| 方法 | 描述 |
| --- | --- |
| [handleCellEvent(Object sender, RowColumnEventArgs e)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.RowColumnEventArgs-) | 处理相关的单元格事件。 |
### handleCellEvent(Object sender, RowColumnEventArgs e) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.RowColumnEventArgs-}
```
public abstract void handleCellEvent(Object sender, RowColumnEventArgs e)
```


处理相关的单元格事件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 发送者 | java.lang.Object | 事件的来源。 |
| e | [RowColumnEventArgs](../../com.aspose.gridweb/rowcolumneventargs) | 事件参数。如果想在 RowDeleting 或 ColumnDeleting 事件处理程序中取消删除操作，请调用 e.RejectOperation()。 |

