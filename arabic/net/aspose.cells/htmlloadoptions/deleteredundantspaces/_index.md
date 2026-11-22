---
title: "HtmlLoadOptions.DeleteRedundantSpaces"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlLoadOptions. تشير إلى ما إذا كان سيتم حذف المسافات الزائدة عندما يلتف النص إلى أسطر باستخدام وسم br. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/htmlloadoptions/deleteredundantspaces/
---
## HtmlLoadOptions.DeleteRedundantSpaces property

يشير إلى ما إذا كان يتم حذف المسافات الزائدة عندما يلتف النص إلى أسطر باستخدام الوسم `<br>`. القيمة الافتراضية هي false.

```csharp
public bool DeleteRedundantSpaces { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyDeleteRedundantSpacesDemo
    {
        public static void Run()
        {
            string html = "<p>   This    text   has   redundant   spaces   </p>";
            
            HtmlLoadOptions opts = new HtmlLoadOptions();
            opts.DeleteRedundantSpaces = true;
            
            byte[] htmlBytes = Encoding.UTF8.GetBytes(html);
            using (MemoryStream stream = new MemoryStream(htmlBytes))
            {
                Workbook workbook = new Workbook(stream, opts);
                Worksheet worksheet = workbook.Worksheets[0];
                
                Console.WriteLine("Cell text after removing redundant spaces: " + 
                    worksheet.Cells["A1"].StringValue);
                
                workbook.Save("output.xlsx");
            }
        }
    }
}
```

### انظر أيضًا

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


