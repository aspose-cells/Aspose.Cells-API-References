---
title: "WorkbookSettings.CheckCompatibility"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Indica se verificare la compatibilità con versioni precedenti durante il salvataggio della cartella di lavoro"
type: docs
url: /it/net/aspose.cells/workbooksettings/checkcompatibility/
---
## WorkbookSettings.CheckCompatibility property

Indica se verificare la compatibilità con versioni precedenti durante il salvataggio della workbook.

```csharp
public bool CheckCompatibility { get; set; }
```

### Osservazioni

Il valore predefinito è true. Solo per file Excel97-2003 xls o xlt.

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyCheckCompatibilityDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Imposta CheckCompatibility su true e salva
            workbook.Settings.CheckCompatibility = true;
            workbook.Save("CheckCompatibilityDemo_true.xlsx");
            
            // Ricarica e verifica
            workbook = new Workbook("CheckCompatibilityDemo_true.xlsx");
            Console.WriteLine("CheckCompatibility (true): " + workbook.Settings.CheckCompatibility);
            
            // Imposta CheckCompatibility su false e salva
            workbook.Settings.CheckCompatibility = false;
            workbook.Save("CheckCompatibilityDemo_false.xlsx");
            
            // Ricarica e verifica
            workbook = new Workbook("CheckCompatibilityDemo_false.xlsx");
            Console.WriteLine("CheckCompatibility (false): " + workbook.Settings.CheckCompatibility);
            
            // Dimostra le operazioni sui colori
            Console.WriteLine("Is Red in palette: " + workbook.IsColorInPalette(Color.Red));
            Color customColor = workbook.GetMatchingColor(Color.FromArgb(255, 123, 123, 123));
            Console.WriteLine("Matching color R value: " + customColor.R);
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


