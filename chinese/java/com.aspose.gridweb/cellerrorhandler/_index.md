---
title: "CellErrorHandler"
second_title: "Aspose.Cells for Java API 参考"
description: "表示用于处理单元格错误事件的接口。"
type: docs
url: /zh/java/com.aspose.gridweb/cellerrorhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CellErrorHandler extends Serializable
```

表示用于处理单元格错误事件的接口。
## 方法

| 方法 | 描述 |
| --- | --- |
| [handleCellEvent(Object sender, GridCellException ex, OnErrorActionQuery query)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.GridCellException-com.aspose.gridweb.OnErrorActionQuery-) | 处理相关的单元格事件。 |
### handleCellEvent(Object sender, GridCellException ex, OnErrorActionQuery query) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.GridCellException-com.aspose.gridweb.OnErrorActionQuery-}
```
public abstract void handleCellEvent(Object sender, GridCellException ex, OnErrorActionQuery query)
```


处理相关的单元格事件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 发送者 | java.lang.Object | 事件的来源。 |
| ex | [GridCellException](../../com.aspose.gridweb/gridcellexception) | 单元格操作错误。 |
| query | [OnErrorActionQuery](../../com.aspose.gridweb/onerroractionquery) | 可以获取 onerror 操作类型信息。 |

