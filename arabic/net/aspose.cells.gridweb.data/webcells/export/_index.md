---
title: "WebCells.Export"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة WebCells. تصدر البيانات في مجموعة Cells من WebWorksheet إلى كائن DataTable جديد"
type: docs
url: /ar/net/aspose.cells.gridweb.data/webcells/export/
---
## WebCells.Export method

يصدّر البيانات في مجموعة Cells لعنصر WebWorksheet إلى كائن DataTable جديد

```csharp
public DataTable Export(int startRow, int startColumn, int rows, int columns, 
    bool exportColumnName, bool isVertical)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | Int32 | رقم الصف للخلية الأولى التي سيتم تصديرها. |
| startColumn | Int32 | رقم العمود للخلية الأولى التي سيتم تصديرها. |
| صفوف | Int32 | عدد الصفوف التي سيتم استيرادها. |
| أعمدة | Int32 | عدد الأعمدة التي سيتم استيرادها. |
| exportColumnName | منطقي | يشير إلى ما إذا كانت البيانات في الصف الأول تُصدر كاسم العمود في DataTable. |
| isVertical | منطقي | صحيح إذا كان الصف في ملف Excel يمثل صفًا في DataTable. خطأ إذا كان العمود في ملف Excel يمثل صفًا في DataTable. |

### قيمة الإرجاع

كائن DataTable المُصدّر.

### انظر أيضًا

* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


