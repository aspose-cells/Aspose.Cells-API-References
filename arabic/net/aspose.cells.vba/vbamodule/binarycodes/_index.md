---
title: "VbaModule.BinaryCodes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية VbaModule. يحصل على ويضبط الرموز الثنائية للوحدة"
type: docs
url: /ar/net/aspose.cells.vba/vbamodule/binarycodes/
---
## VbaModule.BinaryCodes property

يسترجع ويضبط الرموز الثنائية للوحدة.

```csharp
public byte[] BinaryCodes { get; }
```

### أمثلة

```csharp
using System;
using System.Text;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModulePropertyBinaryCodesDemo
    {
        public static void Run()
        {
            // حمّل دفتر العمل مع مشروع VBA
            Workbook workbook = new Workbook("example.xlsm");
            
            // الوصول إلى مشروع VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // احصل على الرموز الثنائية من الوحدة الأولى
            byte[] binaryCodes = vbaProject.Modules[0].BinaryCodes;
            
            // حوّل إلى سلسلة باستخدام ترميز صيني (936)
            string codeContent = Encoding.GetEncoding(936).GetString(binaryCodes);
            
            // أخرج المحتوى الذي يحتوي على أحرف صينية
            Console.WriteLine("VBA Module Content:");
            Console.WriteLine(codeContent);
        }
    }
}
```

### انظر أيضًا

* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


