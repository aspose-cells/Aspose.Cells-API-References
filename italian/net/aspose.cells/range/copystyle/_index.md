---
title: "Range.CopyStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Copia le impostazioni di stile da un intervallo di origine"
type: docs
url: /it/net/aspose.cells/range/copystyle/
---
## Range.CopyStyle method

Copia le impostazioni di stile da un intervallo di origine.

```csharp
public void CopyStyle(Range range)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| range | Range | Oggetto [`Range`](../) di origine. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodCopyStyleWithRangeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet sheetSrc = workbook.Worksheets[0];
            sheetSrc.Name = "Source";
            
            // Aggiungi qualche stile di esempio all'intervallo di origine
            Cells cellsSrc = sheetSrc.Cells;
            Aspose.Cells.Range rangeSrc = cellsSrc.CreateRange("A1:D5");
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            rangeSrc.SetStyle(style);
            
            // Crea foglio di lavoro di destinazione
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "Destination";
            
            // Crea intervallo di destinazione e copia lo stile
            Cells cellsDest = sheetDest.Cells;
            Aspose.Cells.Range rangeDest = cellsDest.CreateRange("A1:D5");
            rangeDest.CopyStyle(rangeSrc);
            
            // Salva la cartella di lavoro
            workbook.Save("RangeCopyStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


