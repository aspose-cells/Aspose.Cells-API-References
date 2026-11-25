---
title: "WorkbookSettings.DataExtractLoad"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. indica se l'applicazione ha aperto per ultimo la cartella di lavoro per il recupero dati"
type: docs
url: /it/net/aspose.cells/workbooksettings/dataextractload/
---
## WorkbookSettings.DataExtractLoad property

Indica se l'applicazione ha aperto per l'ultima volta la workbook per il recupero dati.

```csharp
public bool DataExtractLoad { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDataExtractLoadDemo
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
            string destPath = "output.xlsx";
            workbook.Save(destPath);
            
            // Ricarica la cartella di lavoro per verificare le impostazioni
            Workbook loadedWorkbook = new Workbook(destPath);
            
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


