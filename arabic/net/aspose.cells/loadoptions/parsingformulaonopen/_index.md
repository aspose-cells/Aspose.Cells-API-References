---
title: "LoadOptions.ParsingFormulaOnOpen"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LoadOptions. تشير إلى ما إذا كان يتم تحليل الصيغة عند قراءة الملف"
type: docs
url: /ar/net/aspose.cells/loadoptions/parsingformulaonopen/
---
## LoadOptions.ParsingFormulaOnOpen property

يشير إلى ما إذا كان سيتم تحليل الصيغة عند قراءة الملف.

```csharp
public bool ParsingFormulaOnOpen { get; set; }
```

### ملاحظات

ينطبق فقط على ملفات Excel Xlsx و Xltx و Xltm و Xlsm لأن الصيغ في الملفات تُخزن كصيغة نصية.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyParsingFormulaOnOpenDemo
    {
        public static void Run()
        {
            // إنشاء خيارات التحميل
            LoadOptions loadOptions = new LoadOptions();
            
            // عيّن ParsingFormulaOnOpen إلى false لتخطي تحليل الصيغ أثناء التحميل
            loadOptions.ParsingFormulaOnOpen = false;
            
            // تحميل المصنف باستخدام الخيارات المحددة
            Workbook workbook = new Workbook("example.xlsm", loadOptions);
            
            // الوصول إلى ورقة العمل وإظهار أن تحليل الصيغ تم تخطيه
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Console.WriteLine("Cell A1 formula: " + cell.Formula);
            Console.WriteLine("Cell A1 value: " + cell.Value);
        }
    }
}
```

### انظر أيضًا

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


