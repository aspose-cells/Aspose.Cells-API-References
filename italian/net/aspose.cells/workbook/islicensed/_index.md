---
title: "Workbook.IsLicensed"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Workbook. Indica se la licenza è impostata"
type: docs
url: /it/net/aspose.cells/workbook/islicensed/
---
## Workbook.IsLicensed property

Indica se la licenza è impostata.

```csharp
public bool IsLicensed { get; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyIsLicensedDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            
            // Imposta alcune proprietà di base per dimostrare che il workbook è in uso
            wb.Worksheets[0].Name = "Sheet1";
            wb.Worksheets[0].Cells[0, 0].PutValue("Sample Data");
            
            // Verifica se la cartella di lavoro è licenziata
            Console.WriteLine($"IsLicensed: {wb.IsLicensed}");
            
            // Dimostra un comportamento diverso in base allo stato della licenza
            if (wb.IsLicensed)
            {
                Console.WriteLine("Running in licensed mode - full features available");
            }
            else
            {
                Console.WriteLine("Running in evaluation mode - watermarks will appear");
            }

            // Salva su stream di memoria per dimostrare la funzionalità
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsx);
                Console.WriteLine($"Workbook saved successfully (Size: {ms.Length} bytes)");
            }
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


