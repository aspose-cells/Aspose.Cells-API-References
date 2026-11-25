---
title: "WorkbookSettings.AutoRecover"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Indica se il file è contrassegnato per il recupero automatico"
type: docs
url: /it/net/aspose.cells/workbooksettings/autorecover/
---
## WorkbookSettings.AutoRecover property

Indica se il file è contrassegnato per il recupero automatico.

```csharp
public bool AutoRecover { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyAutoRecoverDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Imposta AutoRecover e altre impostazioni
            workbook.Settings.AutoRecover = false;
            workbook.Settings.DataExtractLoad = true;
            workbook.Settings.CrashSave = true;
            workbook.Settings.RepairLoad = true;

            // Salva la cartella di lavoro
            string outputPath = "WorkbookSettings_AutoRecoverDemo.xlsx";
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


