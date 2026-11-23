---
title: "WriteProtection.Author"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WriteProtection. Obtient et définit l'auteur"
type: docs
url: /fr/net/aspose.cells/writeprotection/author/
---
## WriteProtection.Author property

Obtient et définit l’auteur.

```csharp
public string Author { get; set; }
```

### Exemples

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

            // Démontrer l'utilisation de la propriété Author
            writeProtection.Author = "John Doe";
            writeProtection.Password = "password123";
            
            Console.WriteLine("Write protection author: " + writeProtection.Author);
            Console.WriteLine("Is write protected: " + writeProtection.IsWriteProtected);

            workbook.Save("WriteProtectionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


