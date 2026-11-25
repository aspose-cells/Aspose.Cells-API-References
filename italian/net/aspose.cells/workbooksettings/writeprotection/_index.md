---
title: "WorkbookSettings.WriteProtection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Fornisce l'accesso alle opzioni di protezione della scrittura della cartella di lavoro"
type: docs
url: /it/net/aspose.cells/workbooksettings/writeprotection/
---
## WorkbookSettings.WriteProtection property

Fornisce l'accesso alle opzioni di protezione in scrittura della cartella di lavoro.

```csharp
public WriteProtection WriteProtection { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWriteProtectionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Imposta le proprietà di protezione della scrittura
            workbook.Settings.WriteProtection.Password = "test123";
            workbook.Settings.WriteProtection.Author = "John Doe";
            workbook.Settings.WriteProtection.RecommendReadOnly = true;

            // Salva la cartella di lavoro
            string outputPath = "WriteProtectionDemo.xlsx";
            workbook.Save(outputPath);

            // Carica la cartella di lavoro salvata per verificare le proprietà
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // Restituisci le proprietà di protezione della scrittura
            Console.WriteLine("Author: " + loadedWorkbook.Settings.WriteProtection.Author);
            Console.WriteLine("ReadOnly Recommended: " + loadedWorkbook.Settings.WriteProtection.RecommendReadOnly);
        }
    }
}
```

### Vedi anche

* class [WriteProtection](../../writeprotection/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


