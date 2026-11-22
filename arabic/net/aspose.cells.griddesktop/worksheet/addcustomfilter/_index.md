---
title: "Worksheet.AddCustomFilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. أضف مرشحًا مخصصًا لنطاق الصفوف المحدد من صف البداية إلى صف النهاية"
type: docs
url: /ar/net/aspose.cells.griddesktop/worksheet/addcustomfilter/
---
## AddCustomFilter(int, int, object[], GridFilterOperatorType[]) {#addcustomfilter}

أضف مرشحًا مخصصًا لنطاق الصفوف المحدد من الصف الأول إلى الصف الأخير.

```csharp
public void AddCustomFilter(int startrow, int startcolumn, object[] critiras, 
    GridFilterOperatorType[] filterOperatorTypes)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startrow | Int32 | صف البداية لنطاق الفلتر |
| startcolumn | Int32 | عمود البداية لنطاق الفلتر |
| critiras | Object[] | مصفوفة المعايير للأعمدة، كل واحدة تُطبق على كل عمود |
| filterOperatorTypes | GridFilterOperatorType[] | مصفوفة نوع عملية الفلتر للأعمدة، كل واحدة تُطبق على كل عمود |

### انظر أيضًا

* enum [GridFilterOperatorType](../../../aspose.cells.griddesktop.data/gridfilteroperatortype/)
* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## AddCustomFilter(int, string) {#addcustomfilter_1}

أضف مرشحًا مخصصًا للصف المحدد.

```csharp
public void AddCustomFilter(int row, string critira)
```

### ملاحظات

سلسلة معايير الفلتر. لاحظ أننا نستخدم الفاصلة (,) والفاصلة المنقوطة (;) كحرف تقسيم، لذا يجب ألا تحتوي قيمة الخلية على هذه الأحرف. أدناه أمثلة لسلسلة المعايير: //column 0 with value 12.3 CELL0 = 12.3 //column 1 with value ABC CELL1 = ABC //column 0 with value 123 or 456 or ABC and column 1 with value ABC CELL0 = 123,456,ABC; CELL1 = ABC

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


