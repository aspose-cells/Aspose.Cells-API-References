---
title: "HtmlLoadOptions.DeleteRedundantSpaces"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlLoadOptions‑egenskapen. Anger om överflödiga mellanslag ska tas bort när texten radbryts med br‑taggen. Standardvärdet är false"
type: docs
url: /sv/net/aspose.cells/htmlloadoptions/deleteredundantspaces/
---
## HtmlLoadOptions.DeleteRedundantSpaces property

Anger om överflödiga mellanslag ska tas bort när texten radbryts med `<br>`-taggen. Standardvärdet är false.

```csharp
public bool DeleteRedundantSpaces { get; set; }
```

### Exempel

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

### Se även

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


