---
title: "HtmlLoadOptions.DeleteRedundantSpaces"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlLoadOptions özelliği. Metin br etiketi kullanarak satırları kaydırdığında gereksiz boşlukların silinip silinmeyeceğini gösterir. Varsayılan değer false'tur"
type: docs
url: /tr/net/aspose.cells/htmlloadoptions/deleteredundantspaces/
---
## HtmlLoadOptions.DeleteRedundantSpaces property

Metin satırları `<br>` etiketiyle sarıldığında gereksiz boşlukların silinip silinmeyeceğini gösterir. Varsayılan değer false'dur.

```csharp
public bool DeleteRedundantSpaces { get; set; }
```

### Örnekler

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

### Ayrıca Bakınız

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


