---
title: "GridWorksheet.FilterString"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GridWorksheet. تعيين الفلتر للعمود. ملاحظة: يجب استدعاء AddAutoFilter قبل استدعاء filterString. سلسلة معايير الفلتر. ملاحظة: نستخدم الفاصلة كحرف تقسيم لذا يجب ألا تحتوي قيمة الخلية التي تريد تصفيتها على فاصلة. filterString10123456 يعني أن العمود 10 يجب أن يحتوي على 123 أو 456. filterString10123 يعني أن العمود 10 يجب أن يحتوي على 123. قيمة فهرس العمود مقسومة بفواصل مثال: 123456789 أو abc"
type: docs
url: /ar/net/aspose.cells.gridweb.data/gridworksheet/filterstring/
---
## GridWorksheet.FilterString method

يضبط الفلتر للعمود. لاحظ أننا سنستدعي AddAutoFilter قبل استدعاء filterString. سلسلة معايير الفلتر. لاحظ أننا نستخدم الفاصلة-&gt;"," كحرف تقسيم، لذا يجب ألا تحتوي قيمة الخلية التي تريد تصفيتها على الفاصلة. filterString(10,"123,456") يعني أن العمود 10 يجب أن يحتوي على 123 أو 456، filterString(10,"123") يعني أن العمود 10 يجب أن يحتوي على 123 قيمة فهرس العمود مقسمة بالفاصلة، مثال: 123,456,789 أو abc

```csharp
public void FilterString(int column, string criteria)
```

### انظر أيضًا

* class [GridWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


