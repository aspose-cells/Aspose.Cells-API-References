---
title: "WriteProtection.Author"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WriteProtection. Ottiene e imposta l'autore"
type: docs
url: /it/net/aspose.cells/writeprotection/author/
---
## WriteProtection.Author property

Ottiene e imposta l'autore.

```csharp
public string Author { get; set; }
```

### Esempi

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

            // Dimostra l'uso della proprietà Author
            writeProtection.Author = "John Doe";
            writeProtection.Password = "password123";
            
            Console.WriteLine("Write protection author: " + writeProtection.Author);
            Console.WriteLine("Is write protected: " + writeProtection.IsWriteProtected);

            workbook.Save("WriteProtectionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


