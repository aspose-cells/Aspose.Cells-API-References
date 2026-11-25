---
title: "WorkbookSettings.RepairLoad"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Indica se l'applicazione ha aperto l'ultima volta la cartella di lavoro in modalità sicura o di riparazione"
type: docs
url: /it/net/aspose.cells/workbooksettings/repairload/
---
## WorkbookSettings.RepairLoad property

Indica se l'applicazione ha aperto l'ultimo workbook in modalità sicura o di riparazione.

```csharp
public bool RepairLoad { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyRepairLoadDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Configura le impostazioni della cartella di lavoro
            workbook.Settings.AutoRecover = false;
            workbook.Settings.DataExtractLoad = true;
            workbook.Settings.CrashSave = true;
            workbook.Settings.RepairLoad = true;

            // Salva la cartella di lavoro
            string outputPath = "WorkbookSettings_RepairLoad_Example.xlsx";
            workbook.Save(outputPath);

            // Carica la cartella di lavoro salvata per verificare le impostazioni
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // Stampa le impostazioni sulla console
            Console.WriteLine("AutoRecover: " + loadedWorkbook.Settings.AutoRecover);
            Console.WriteLine("DataExtractLoad: " + loadedWorkbook.Settings.DataExtractLoad);
            Console.WriteLine("CrashSave: " + loadedWorkbook.Settings.CrashSave);
            Console.WriteLine("RepairLoad: " + loadedWorkbook.Settings.RepairLoad);
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


