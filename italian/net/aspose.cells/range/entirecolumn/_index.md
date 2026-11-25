---
title: "Range.EntireColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Range. Restituisce un oggetto Range che rappresenta l'intera colonna o le colonne che contengono l'intervallo specificato"
type: docs
url: /it/net/aspose.cells/range/entirecolumn/
---
## Range.EntireColumn property

Ottiene un oggetto Range che rappresenta l'intera colonna (o le colonne) che contiene l'intervallo specificato.

```csharp
public Range EntireColumn { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyEntireColumnDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un intervallo che inizia dalla cella C1 (riga 0, colonna 2)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 2, 1, 1);
            
            // Ottieni l'intera colonna che contiene l'intervallo (colonna C)
            Aspose.Cells.Range entireColumn = range.EntireColumn;
            
            // Applica la formattazione all'intera colonna
            Style style = entireColumn[0, 0].GetStyle();
            style.Custom = "##0%";
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.NumberFormat = true;
            entireColumn.ApplyStyle(style, styleFlag);
            
            // Salva la cartella di lavoro
            workbook.Save("EntireColumnDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


