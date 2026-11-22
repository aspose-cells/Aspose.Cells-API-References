---
title: "VbaModule.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية VbaModule. يحصل على ويضبط اسم الوحدة"
type: docs
url: /ar/net/aspose.cells.vba/vbamodule/name/
---
## VbaModule.Name property

يسترجع ويضبط اسم الوحدة.

```csharp
public string Name { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModulePropertyNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();

            // أضف ورقة عمل واحصل على وحدة VBA الخاصة بها
            Worksheet sheet = wb.Worksheets[0];
            int moduleIndex = wb.VbaProject.Modules.Add(sheet);
            VbaModule module = wb.VbaProject.Modules[moduleIndex];

            // حدد اسم الوحدة
            module.Name = "Sheet1";

            // أضف كود VBA بسيط إلى الوحدة
            string vbaCode = "Private Sub Worksheet_SelectionChange(ByVal Target As Range)\r\n" +
                             "    MsgBox \"Sheet name: \" & Me.Name\r\n" +
                             "End Sub\r\n";
            module.Codes = vbaCode;

            // احفظ إلى تدفق الذاكرة (للتوضيح)
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsm);
            }
        }
    }
}
```

### انظر أيضًا

* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


