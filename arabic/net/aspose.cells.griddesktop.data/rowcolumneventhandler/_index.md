---
title: RowColumnEventHandler
second_title: Aspose.Cells لمرجع .NET API
description: يمثل الواجهة التي تنوي معالجة أحداث الصف / العمود.
type: docs
weight: 780
url: /ar/net/aspose.cells.griddesktop.data/rowcolumneventhandler/
---
## RowColumnEventHandler delegate

يمثل الواجهة التي تنوي معالجة أحداث الصف / العمود.

فارغ **التعامل مع الخلية**(مرسل الكائن ، RowColumnEventArgs e) ؛

```csharp
public delegate void RowColumnEventHandler(object sender, RowColumnEventArgs e);
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| sender | Object | مصدر الحدث. |
| e | RowColumnEventArgs | حجة الحدث. قم باستدعاء e.RejectOperation () إذا كنت تريد إلغاء عملية الحذف في RowDeleting أو ColumnDeleting مع معالجات الأحداث. |

### أنظر أيضا

* class [RowColumnEventArgs](../../aspose.cells.griddesktop/rowcolumneventargs)
* مساحة الاسم [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data)
* المجسم [Aspose.Cells.GridDesktop](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
