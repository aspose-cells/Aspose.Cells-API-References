---
title: "WorkbookSettings.ProtectionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "WorkbookSettings property. Ottiene il tipo di protezione della cartella di lavoro"
type: docs
url: /it/net/aspose.cells/workbooksettings/protectiontype/
---
## WorkbookSettings.ProtectionType property

Ottiene il tipo di protezione del workbook.

```csharp
public ProtectionType ProtectionType { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyProtectionTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Proteggi la cartella di lavoro con il tipo di protezione Windows
            workbook.Protect(ProtectionType.Windows, "password123");
            
            // Dimostra la proprietà ProtectionType
            Console.WriteLine("Workbook protection type: " + workbook.Settings.ProtectionType);
            
            // Salva la cartella di lavoro
            workbook.Save("ProtectedWorkbook.xlsx");
            
            // Carica la cartella di lavoro salvata per verificare che il tipo di protezione persista
            Workbook loadedWorkbook = new Workbook("ProtectedWorkbook.xlsx");
            Console.WriteLine("Loaded workbook protection type: " + loadedWorkbook.Settings.ProtectionType);
        }
    }
}
```

### Vedi anche

* enum [ProtectionType](../../protectiontype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


