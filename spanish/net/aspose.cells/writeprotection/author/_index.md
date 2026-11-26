---
title: "WriteProtection.Author"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WriteProtection. Obtiene y establece el autor"
type: docs
url: /es/net/aspose.cells/writeprotection/author/
---
## WriteProtection.Author property

Obtiene y establece el autor.

```csharp
public string Author { get; set; }
```

### Ejemplos

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

            // Demostrar el uso de la propiedad Author
            writeProtection.Author = "John Doe";
            writeProtection.Password = "password123";
            
            Console.WriteLine("Write protection author: " + writeProtection.Author);
            Console.WriteLine("Is write protected: " + writeProtection.IsWriteProtected);

            workbook.Save("WriteProtectionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


