---
title: "LoadOptions.ParsingPivotCachedRecords"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LoadOptions. تشير إلى ما إذا كان يتم تحليل سجلات Pivot المخزنة مؤقتًا عند تحميل الملف. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/loadoptions/parsingpivotcachedrecords/
---
## LoadOptions.ParsingPivotCachedRecords property

يشير إلى ما إذا كان سيتم تحليل سجلات Pivot المخزنة مؤقتًا عند تحميل الملف. القيمة الافتراضية هي false.

```csharp
public bool ParsingPivotCachedRecords { get; set; }
```

### ملاحظات

ينطبق فقط على ملفات Excel Xlsx، Xltx، Xltm، Xlsm و xlsb

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyParsingPivotCachedRecordsDemo
    {
        public static void Run()
        {
            // إنشاء خيارات تحميل CSV
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv);
            
            // تمكين تحليل سجلات Pivot المخزنة مؤقتًا
            loadOptions.ParsingPivotCachedRecords = true;
            
            // حمّل دفتر العمل باستخدام الخيارات
            Workbook workbook = new Workbook("example.csv", loadOptions);
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "PivotData";
            
            // إنشاء جدول محوري (إظهار أن الخاصية تم تعيينها)
            int pivotIndex = worksheet.PivotTables.Add("A1:C10", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // احفظ المصنف
            workbook.Save("PivotTableOutput.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


