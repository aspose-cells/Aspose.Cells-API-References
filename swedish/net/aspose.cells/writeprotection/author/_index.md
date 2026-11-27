---
title: "WriteProtection.Author"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WriteProtection-egenskapen. Hämtar och anger författaren"
type: docs
url: /sv/net/aspose.cells/writeprotection/author/
---
## WriteProtection.Author property

Hämtar och anger författaren.

```csharp
public string Author { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionPropertyAuthorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WorkbookSettings settings = workbook.Settings;
            WriteProtection writeProtection = settings.WriteProtection;

            // Demonstrera användning av Author-egenskapen
            writeProtection.Author = "John Doe";
            writeProtection.Password = "password123";
            
            Console.WriteLine("Write protection author: " + writeProtection.Author);
            Console.WriteLine("Is write protected: " + writeProtection.IsWriteProtected);

            workbook.Save("WriteProtectionDemo.xlsx");
        }
    }
}
```

### Se även

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


