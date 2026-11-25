---
title: "WorkbookSettings.CheckCustomNumberFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Indica se verificare il formato numerico personalizzato quando si imposta Style.Custom"
type: docs
url: /it/net/aspose.cells/workbooksettings/checkcustomnumberformat/
---
## WorkbookSettings.CheckCustomNumberFormat property

Indica se controllare il formato numerico personalizzato quando si imposta Style.Custom.

```csharp
public bool CheckCustomNumberFormat { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyCheckCustomNumberFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Style style = workbook.CreateStyle();
            
            // Prima impostare un formato numerico personalizzato valido
            style.Custom = "#,##0.00";
            
            // Abilitare la verifica rigorosa
            workbook.Settings.CheckCustomNumberFormat = true;
            
            try
            {
                // Tentare di impostare un formato numerico personalizzato non valido
                style.Custom = "fff @ ggg";
            }
            catch (CellsException ex)
            {
                Console.WriteLine("Error setting custom format: " + ex.Message);
            }
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


