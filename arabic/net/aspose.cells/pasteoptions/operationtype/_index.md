---
title: "PasteOptions.OperationType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PasteOptions. يحصل على ويضبط نوع العملية عند لصق النطاق"
type: docs
url: /ar/net/aspose.cells/pasteoptions/operationtype/
---
## PasteOptions.OperationType property

يحصل على ويضبط نوع العملية عند لصق النطاق.

```csharp
public PasteOperationType OperationType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyOperationTypeDemo
    {
        public static void Run()
        {
            // إنشاء مصنف المصدر مع بيانات عينة
            Workbook wbOrigin = new Workbook();
            Worksheet sourceSheet = wbOrigin.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Data");
            sourceSheet.Cells["B2"].PutValue(100);
            
            // إنشاء دفتر عمل هدف
            Workbook wbDestination = new Workbook();
            Worksheet destSheet = wbDestination.Worksheets[0];
            destSheet.Cells["A1"].PutValue("Destination Data");
            destSheet.Cells["B2"].PutValue(200); // Will be modified by paste operation
            
            // إنشاء نطاقات للنسخ/اللصق
            var rangeOrigin = sourceSheet.Cells.CreateRange("A1:B3");
            var rangeDestination = destSheet.Cells.CreateRange("A1:B3");
            
            // إنشاء خيارات اللصق مع توضيح OperationType
            var options = new PasteOptions
            {
                PasteType = PasteType.All,
                OperationType = PasteOperationType.Add // Values will be added (100 + 200 = 300)
            };
            
            // تنفيذ عملية النسخ/اللصق
            rangeDestination.Copy(rangeOrigin, options);
            
            // تحقق من النتيجة
            Console.WriteLine("B2 value after paste with Add operation: " + destSheet.Cells["B2"].IntValue);
            
            // حفظ النتيجة
            wbDestination.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* enum [PasteOperationType](../../pasteoperationtype/)
* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


