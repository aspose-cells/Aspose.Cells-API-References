---
title: "Worksheet.FilterString"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. تعيين الفلتر للعمود. ملاحظة: يجب استدعاء AddAutoFilter قبل استدعاء filterString سلسلة معايير الفلتر. ملاحظة: نستخدم الفاصلة كحرف تقسيم، لذا يجب ألا يحتوي قيمة الخلية التي تريد تصفيتها على فاصلة. filterString10123456 يعني أن العمود 10 يجب أن يحتوي على 123 أو 456 filterString10123 يعني أن العمود 10 يجب أن يحتوي على القيمة 123، مفصولة بفواصل، مثال: 123456789 أو abc"
type: docs
url: /ar/net/aspose.cells.griddesktop/worksheet/filterstring/
---
## Worksheet.FilterString method

يضبط الفلتر للعمود. لاحظ أننا سنستدعي AddAutoFilter قبل استدعاء filterString. سلسلة معايير الفلتر. لاحظ أننا نستخدم الفاصلة-&gt;"," كحرف تقسيم، لذا يجب ألا تحتوي قيمة الخلية التي تريد تصفيتها على الفاصلة. filterString(10,"123,456") يعني أن العمود 10 يجب أن يحتوي على 123 أو 456، filterString(10,"123") يعني أن العمود 10 يجب أن يحتوي على 123. القيم مفصولة بفاصلة، مثال: 123,456,789 أو abc

```csharp
public void FilterString(int column, string criteria)
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


