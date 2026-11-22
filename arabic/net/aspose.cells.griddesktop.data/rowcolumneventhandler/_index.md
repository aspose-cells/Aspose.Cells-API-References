---
title: "مفوض RowColumnEventHandler"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "يمثل الواجهة التي تهدف إلى معالجة أحداث الصف/العمود"
type: docs
url: /ar/net/aspose.cells.griddesktop.data/rowcolumneventhandler/
---
## RowColumnEventHandler delegate

يمثل الواجهة التي تهدف إلى معالجة أحداث الصف/العمود.

void **handleCellEvent**(Object sender, RowColumnEventArgs e);

```csharp
public delegate void RowColumnEventHandler(object sender, RowColumnEventArgs e);
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sender | Object | مصدر الحدث. |
| e | RowColumnEventArgs | معامل الحدث. استدعِ e.RejectOperation() إذا كنت تريد إلغاء عملية الحذف في معالجات أحداث RowDeleting أو ColumnDeleting. |

### انظر أيضًا

* class [RowColumnEventArgs](../../aspose.cells.griddesktop/rowcolumneventargs/)
* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


