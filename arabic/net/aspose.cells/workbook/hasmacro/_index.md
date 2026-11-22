---
title: "Workbook.HasMacro"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Workbook. تشير إلى ما إذا كانت هذه الورقة تحتوي على ماكرو/VBA"
type: docs
url: /ar/net/aspose.cells/workbook/hasmacro/
---
## Workbook.HasMacro property

يشير إلى ما إذا كان هذا الجدول يحتوي على ماكرو/VBA.

```csharp
public bool HasMacro { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyHasMacroDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل مع ماكرو بتحميل ملف قالب
            Workbook workbookWithMacro = new Workbook("sample_with_macro.xlsm");
            Console.WriteLine("Workbook with macro - HasMacro: " + workbookWithMacro.HasMacro);

            // إنشاء دفتر عمل بدون ماكرو
            Workbook workbookWithoutMacro = new Workbook();
            Console.WriteLine("Workbook without macro - HasMacro: " + workbookWithoutMacro.HasMacro);
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


