---
title: "HtmlLoadOptions.DeleteRedundantSpaces"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlLoadOptions-Eigenschaft. Gibt an, ob überflüssige Leerzeichen gelöscht werden, wenn der Text Zeilenumbrüche mit dem br-Tag erzeugt. Der Standardwert ist false"
type: docs
url: /de/net/aspose.cells/htmlloadoptions/deleteredundantspaces/
---
## HtmlLoadOptions.DeleteRedundantSpaces property

Gibt an, ob überflüssige Leerzeichen gelöscht werden, wenn der Text Zeilenumbrüche mit dem `<br>`‑Tag erzeugt. Der Standardwert ist false.

```csharp
public bool DeleteRedundantSpaces { get; set; }
```

### Beispiele

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

### Siehe auch

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


