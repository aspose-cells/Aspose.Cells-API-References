---
title: "HtmlLoadOptions.DeleteRedundantSpaces"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlLoadOptions. Indica si se eliminan los espacios redundantes cuando el texto envuelve líneas usando la etiqueta br. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/htmlloadoptions/deleteredundantspaces/
---
## HtmlLoadOptions.DeleteRedundantSpaces property

Indica si se eliminan los espacios redundantes cuando el texto envuelve líneas usando la etiqueta `<br>`. El valor predeterminado es false.

```csharp
public bool DeleteRedundantSpaces { get; set; }
```

### Ejemplos

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

### Ver también

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


