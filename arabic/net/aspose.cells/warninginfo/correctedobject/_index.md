---
title: "WarningInfo.CorrectedObject"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WarningInfo. يحصل ويضبط الكائن المصحح"
type: docs
url: /ar/net/aspose.cells/warninginfo/correctedobject/
---
## WarningInfo.CorrectedObject property

يحصل على ويضبط الكائن المصحح.

```csharp
public object CorrectedObject { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WarningInfoPropertyCorrectedObjectDemo
    {
        public static void Run()
        {
            // إنشاء مصنف وتفعيل التحذير
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // قم بتعيين اسم قد يثير تحذيرًا عادةً
            string originalName = "MyRange";
            worksheet.Cells.CreateRange(originalName);
            
            // معالجة رد النداء للتحذير
            workbook.Settings.WarningCallback = new WarningHandler();
            
            // هذه العملية ستؤدي إلى تشغيل رد النداء للتحذير
            worksheet.Cells.CreateRange(originalName); // Duplicate range name
        }
    }

    public class WarningHandler : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            if (warningInfo.WarningType == WarningType.DuplicateDefinedName)
            {
                // توضيح استخدام CorrectedObject
                warningInfo.CorrectedObject = "_" + warningInfo.ErrorObject;
                Console.WriteLine($"Warning handled. Original: {warningInfo.ErrorObject}, Corrected: {warningInfo.CorrectedObject}");
            }
        }
    }
}
```

### انظر أيضًا

* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


