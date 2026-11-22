---
title: "الفئة CellValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.CellValue. تمثّل قيمة الخلية والنوع المقابل لها"
type: docs
url: /ar/net/aspose.cells/cellvalue/
---
## CellValue class

يمثل قيمة الخلية والنوع المقابل.

```csharp
public class CellValue
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [CellValue](cellvalue/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Type](../../aspose.cells/cellvalue/type/) { get; set; } | يحصل أو يعيّن نوع قيمة الخلية. |
| [Value](../../aspose.cells/cellvalue/value/) { get; set; } | يحصل أو يعيّن قيمة الخلية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellValueDemo
    {
        public static void CellValueExample()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أنشئ مثيلاً من CellValue
            CellValue cellValue = new CellValue();

            // عيّن النوع والقيمة للخلية
            cellValue.Type = CellValueType.IsNumeric;
            cellValue.Value = 123.45;

            // قم بتعيين CellValue إلى خلية في ورقة العمل
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue(cellValue.Value);

            // احفظ المصنف
            workbook.Save("CellValueExample.xlsx");
            workbook.Save("CellValueExample.pdf");
            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


