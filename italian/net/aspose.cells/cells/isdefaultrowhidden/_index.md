---
title: "Cells.IsDefaultRowHidden"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cells. Indica se la riga è nascosta di default"
type: docs
url: /it/net/aspose.cells/cells/isdefaultrowhidden/
---
## Cells.IsDefaultRowHidden property

Indica se la riga è nascosta per impostazione predefinita.

```csharp
public bool IsDefaultRowHidden { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyIsDefaultRowHiddenDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta la proprietà di riga nascosta predefinita
            worksheet.Cells.IsDefaultRowHidden = true;
            
            // Visualizza il valore corrente di IsDefaultRowHidden
            Console.WriteLine("IsDefaultRowHidden: " + worksheet.Cells.IsDefaultRowHidden);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


