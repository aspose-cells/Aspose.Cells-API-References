---
title: "WriteProtection.IsWriteProtected"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WriteProtection. Indica se questa cartella di lavoro è protetta dalla scrittura"
type: docs
url: /it/net/aspose.cells/writeprotection/iswriteprotected/
---
## WriteProtection.IsWriteProtected property

Indica se questa cartella di lavoro è protetta in scrittura.

```csharp
public bool IsWriteProtected { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionPropertyIsWriteProtectedDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Abilita la protezione dalla scrittura con password
            workbook.Settings.WriteProtection.Password = "1234";
            
            // Verifica se la cartella di lavoro è protetta dalla scrittura
            Console.WriteLine("Is workbook write protected? " + 
                workbook.Settings.WriteProtection.IsWriteProtected);
            
            // Convalida la password
            Console.WriteLine("Is password valid? " + 
                workbook.Settings.WriteProtection.ValidatePassword("1234"));
            
            // Salva la cartella di lavoro
            workbook.Save("WriteProtectedWorkbook.xlsx");
            
            // Carica la cartella di lavoro salvata per verificare la protezione
            Workbook loadedWorkbook = new Workbook("WriteProtectedWorkbook.xlsx");
            
            // Verifica nuovamente lo stato della protezione
            Console.WriteLine("Is loaded workbook write protected? " + 
                loadedWorkbook.Settings.WriteProtection.IsWriteProtected);
        }
    }
}
```

### Vedi anche

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


