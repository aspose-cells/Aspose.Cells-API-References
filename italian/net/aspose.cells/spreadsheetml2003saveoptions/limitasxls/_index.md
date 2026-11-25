---
title: "SpreadsheetML2003SaveOptions.LimitAsXls"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SpreadsheetML2003SaveOptions. Limit as xls: l'indice massimo di riga è 65535 e l'indice massimo di colonna è 255"
type: docs
url: /it/net/aspose.cells/spreadsheetml2003saveoptions/limitasxls/
---
## SpreadsheetML2003SaveOptions.LimitAsXls property

Limite per xls, l'indice massimo di riga è 65535 e l'indice massimo di colonna è 255.

```csharp
public bool LimitAsXls { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetML2003SaveOptionsPropertyLimitAsXlsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            
            // Accedi alle celle e crea un intervallo
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange("A1", "C5");
            range.Name = "TestRange";
            
            // Salva con LimitAsXls = true
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions()
            {
                LimitAsXls = true
            };
            
            // Salva come SpreadsheetML con limiti XLS
            workbook.Save("output.xml", saveOptions);
            
            Console.WriteLine("File saved with LimitAsXls=true");
        }
    }
}
```

### Vedi anche

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


