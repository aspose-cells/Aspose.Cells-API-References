---
title: "HtmlLoadOptions.DeleteRedundantSpaces"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlLoadOptions. Указывает, удалять ли избыточные пробелы, когда текст переносит строки с помощью тега br. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/htmlloadoptions/deleteredundantspaces/
---
## HtmlLoadOptions.DeleteRedundantSpaces property

Указывает, следует ли удалять лишние пробелы при переносе строк текста с использованием тега `<br>`. Значение по умолчанию — false.

```csharp
public bool DeleteRedundantSpaces { get; set; }
```

### Примеры

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

### См. также

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


