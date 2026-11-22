---
title: "Workbook.Combine"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تجمع كائن Workbook آخر"
type: docs
url: /ar/net/aspose.cells/workbook/combine/
---
## Workbook.Combine method

يجمع كائن مصنف آخر.

```csharp
public void Combine(Workbook secondWorkbook)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| secondWorkbook | المصنف | كائن Workbook آخر. |

### ملاحظات

دمج Excel و ODS و CSV وغيرها من الملفات في ملف واحد.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCombineWithWorkbookDemo
    {
        public static void Run()
        {
            // إنشاء مصنف المصدر
            Workbook sourceWorkbook = new Workbook();
            sourceWorkbook.Worksheets[0].Cells["A1"].PutValue("Source Data");

            // إنشاء دفتر عمل هدف
            Workbook destWorkbook = new Workbook(FileFormatType.Xlsx);
            destWorkbook.Worksheets[0].Cells["B2"].PutValue("Destination Data");

            // دمج المصنفات
            destWorkbook.Combine(sourceWorkbook);

            // حفظ المصنف المدمج
            destWorkbook.Save("CombinedWorkbook.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


