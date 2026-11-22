---
title: "ExportTableOptions.CheckMixedValueType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExportTableOptions. False سيقوم Aspose.Cells بتعيين نوع DataColumns بناءً على نوع القيمة في الصف الأول لأداء أفضل. True سيقوم Aspose.Cells بالتحقق مما إذا كان نوع القيمة في العمود مختلطًا قبل تعيين نوع DataColumns، وإذا كان النوع مختلطًا فإن نوع DataColumns سيكون string"
type: docs
url: /ar/net/aspose.cells/exporttableoptions/checkmixedvaluetype/
---
## ExportTableOptions.CheckMixedValueType property

False، سيقوم Aspose.Cells بتعيين نوع DataColumn بناءً على نوع القيمة في الصف الأول للأداء. True، سيتحقق Aspose.Cells مما إذا كان نوع القيمة في العمود مختلطًا قبل تعيين نوع DataColumn، وإذا كان نوع القيمة مختلطًا، سيكون نوع DataColumn هو string.

```csharp
public bool CheckMixedValueType { get; set; }
```

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyCheckMixedValueTypeDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف رؤوس
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Value Date");

            // أضف بيانات عينة بأنواع مختلطة
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(DateTime.Now);
            worksheet.Cells["A3"].PutValue(2.5);
            worksheet.Cells["B3"].PutValue("2023-01-15");
            worksheet.Cells["A4"].PutValue("3");
            worksheet.Cells["B4"].PutValue(DateTime.Now.AddDays(1));

            // إنشاء خيارات التصدير مع تمكين CheckMixedValueType
            ExportTableOptions options = new ExportTableOptions
            {
                CheckMixedValueType = true,
                ExportColumnName = true
            };

            // تصدير البيانات إلى DataTable
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 4, 2, options);

            // عرض النتائج
            Console.WriteLine("Columns: " + dataTable.Columns.Count);
            Console.WriteLine("Rows: " + dataTable.Rows.Count);
            Console.WriteLine("ID column type: " + dataTable.Columns["ID"].DataType);
            Console.WriteLine("Value Date column type: " + dataTable.Columns["Value Date"].DataType);
        }
    }
}
```

### انظر أيضًا

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


