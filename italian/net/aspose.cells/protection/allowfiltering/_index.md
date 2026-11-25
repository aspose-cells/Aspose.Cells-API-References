---
title: "Protection.AllowFiltering"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Protection. Rappresenta se all'utente è consentito utilizzare un AutoFilter creato prima che il foglio fosse protetto"
type: docs
url: /it/net/aspose.cells/protection/allowfiltering/
---
## Protection.AllowFiltering property

Rappresenta se all'utente è consentito utilizzare un AutoFiltro creato prima che il foglio fosse protetto.

```csharp
public bool AllowFiltering { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowFilteringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Abilita la protezione del foglio di lavoro
            worksheet.Protect(ProtectionType.All);
            
            // Imposta la proprietà AllowFiltering su true
            worksheet.Protection.AllowFiltering = true;
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
            
            // Verifica che la proprietà sia stata salvata correttamente
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("AllowFiltering: " + 
                loadedWorkbook.Worksheets[0].Protection.AllowFiltering);
        }
    }
}
```

### Vedi anche

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


