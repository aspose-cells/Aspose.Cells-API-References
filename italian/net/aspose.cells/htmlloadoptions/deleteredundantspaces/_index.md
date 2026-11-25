---
title: "HtmlLoadOptions.DeleteRedundantSpaces"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlLoadOptions. Indica se eliminare spazi ridondanti quando il testo avvolge le righe usando il tag br. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/htmlloadoptions/deleteredundantspaces/
---
## HtmlLoadOptions.DeleteRedundantSpaces property

Indica se eliminare gli spazi ridondanti quando il testo avvolge le righe usando il tag `<br>`. Il valore predefinito è false.

```csharp
public bool DeleteRedundantSpaces { get; set; }
```

### Esempi

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

### Vedi anche

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


