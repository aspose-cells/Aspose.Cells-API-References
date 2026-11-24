---
title: "WriteProtection.Author"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WriteProtection-Eigenschaft. Gibt den Autor zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells/writeprotection/author/
---
## WriteProtection.Author property

Liest und setzt den Autor.

```csharp
public string Author { get; set; }
```

### Beispiele

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

            // Verwendung der Author-Eigenschaft demonstrieren
            writeProtection.Author = "John Doe";
            writeProtection.Password = "password123";
            
            Console.WriteLine("Write protection author: " + writeProtection.Author);
            Console.WriteLine("Is write protected: " + writeProtection.IsWriteProtected);

            workbook.Save("WriteProtectionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


