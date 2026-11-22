---
title: "ExportTableOptions.PreprocessExportedValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ExportTableOptions. معالجة مسبقة لقيمة الخلية الحالية قبل تصديرها"
type: docs
url: /ar/net/aspose.cells/exporttableoptions/preprocessexportedvalue/
---
## ExportTableOptions.PreprocessExportedValue method

معالجة مسبقة لقيمة الخلية الحالية لتصديرها.

```csharp
public virtual bool PreprocessExportedValue(int cellRow, int cellColumn, CellValue value)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| cellRow | Int32 | فهرس الصف للخلية الحالية |
| cellColumn | Int32 | فهرس العمود للخلية |
| القيمة | CellValue | القيمة والنوع للخلية الحالية |

### قيمة الإرجاع

ما إذا تم استبدال الخلية الحالية بنوع مختلف و/أو قيمة.

### ملاحظات

مؤشر الصف والعمود هو الفهرس المطلق للخلية في ورقة العمل، وليس الفهرس في الجدول المُصدَّر. قد يتحقق المستخدم من قيمة الخلية الحالية في تنفيذ التجاوز لهذه الطريقة، إذا كان يجب استبدال الخلية الحالية بنوع وقيمة أخرى، يجب على التنفيذ هنا تعيين النوع والقيمة المتوقعة إلى كائن CellValue وإرجاع true. بشكل افتراضي لا تفعل هذه الطريقة شيئًا وتُعيد false.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExportTableOptionsMethodPreprocessExportedValueWithInt32Int32CellValueDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء بيانات عينة في ورقة العمل
            worksheet.Cells["A1"].PutValue("Test Value");
            worksheet.Cells["A2"].PutValue(123.45);
            worksheet.Cells["A3"].PutValue(DateTime.Now);

            // إنشاء مثال من ExportTableOptions
            ExportTableOptions exportOptions = new ExportTableOptions();

            // إنشاء كائن CellValue للتوضيح
            CellValue cellValue = new CellValue();
            cellValue.Type = CellValueType.IsString;
            cellValue.Value = "Processed Value";

            try
            {
                // استدعِ PreprocessExportedValue بالمعلمات المحددة (الصف 0، العمود 0، CellValue)
                bool result = exportOptions.PreprocessExportedValue(0, 0, cellValue);

                // اعرض نتيجة استدعاء الطريقة
                Console.WriteLine($"PreprocessExportedValue returned: {result}");

                // عدّل الخلية بالقيمة المعالجة إذا لزم الأمر
                if (result)
                {
                    worksheet.Cells[0, 0].PutValue(cellValue.Value);
                }

                // احفظ المصنف
                workbook.Save("PreprocessExportedValueDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing PreprocessExportedValue method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [CellValue](../../cellvalue/)
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


