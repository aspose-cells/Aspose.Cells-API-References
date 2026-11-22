---
title: "Style.IsFormulaHidden"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Style. تمثل ما إذا كانت الصيغة ستُخفى عندما يتم حماية ورقة العمل"
type: docs
url: /ar/net/aspose.cells/style/isformulahidden/
---
## Style.IsFormulaHidden property

يمثل ما إذا كانت الصيغة ستُخفى عندما يتم حماية ورقة العمل.

```csharp
public bool IsFormulaHidden { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsFormulaHiddenDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // إنشاء نمط مع تعيين IsFormulaHidden إلى true
            Style style = workbook.CreateStyle();
            style.IsFormulaHidden = true;
            
            // تطبيق النمط على خلية
            cells["A1"].SetStyle(style);
            cells["A1"].Formula = "=1+1";

            // إنشاء نمط آخر مع تعيين IsFormulaHidden إلى false
            Style style2 = workbook.CreateStyle();
            style2.IsFormulaHidden = false;
            
            // تطبيق النمط الثاني على خلية أخرى
            cells["B1"].SetStyle(style2);
            cells["B1"].Formula = "=2+2";

            // احمِ ورقة العمل لرؤية التأثير
            worksheet.Protect(ProtectionType.All, "password", null);

            // احفظ المصنف
            workbook.Save("IsFormulaHiddenDemo.xlsx");

            Console.WriteLine("Workbook saved with IsFormulaHidden examples.");
        }
    }
}
```

### انظر أيضًا

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


