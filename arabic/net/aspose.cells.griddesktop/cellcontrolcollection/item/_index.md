---
title: "CellControlCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CellControlCollection. تحصل على التحكم في الخلية عند فهرس الصف والعمود المحدد"
type: docs
url: /ar/net/aspose.cells.griddesktop/cellcontrolcollection/item/
---
## CellControlCollection indexer (1 of 2)

يحصل على التحكم في الخلية عند فهرس الصف والعمود المحدد.

```csharp
public CellControl this[int row, int col] { get; }
```

| معامل | الوصف |
| --- | --- |
| صف | فهرس الصف. |
| عمود | فهرس العمود. |

### ملاحظات

إذا لم يكن هناك كائن CellControl عند فهرس الصف والعمود المحدد، سيتحقق هذا من كائن CellControl للعمود.

### انظر أيضًا

* class [CellControl](../../cellcontrol/)
* class [CellControlCollection](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## CellControlCollection indexer (2 of 2)

يحصل على التحكم في الخلية بالاسم المحدد للخلية.

```csharp
public CellControl this[string cellName] { get; }
```

| معامل | الوصف |
| --- | --- |
| cellName | اسم الخلية (بتنسيق اسم إكسل، مثل 'A1'، 'F22') |

### ملاحظات

إذا لم يكن هناك كائن CellControl عند فهرس الصف والعمود المحدد، سيتحقق هذا من كائن CellControl للعمود.

### انظر أيضًا

* class [CellControl](../../cellcontrol/)
* class [CellControlCollection](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


