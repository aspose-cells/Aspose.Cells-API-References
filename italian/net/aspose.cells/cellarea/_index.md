---
title: "Struttura CellArea"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.CellArea struct. Rappresenta un'area di celle"
type: docs
url: /it/net/aspose.cells/cellarea/
---
## CellArea structure

Rappresenta un'area di celle.

```csharp
public struct CellArea : IComparable
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [CreateCellArea](../../aspose.cells/cellarea/createcellarea/#createcellarea_1)(string, string) | Crea un'area di celle. |
| static [CreateCellArea](../../aspose.cells/cellarea/createcellarea/#createcellarea)(int, int, int, int) | Crea un'area di celle. |
| [CompareTo](../../aspose.cells/cellarea/compareto/)(object) | Confronta due oggetti CellArea in base al loro angolo in alto a sinistra. |
| override [ToString](../../aspose.cells/cellarea/tostring/)() | Restituisce una stringa che rappresenta l'oggetto CellArea corrente. |

## Campi

| Nome | Descrizione |
| --- | --- |
| [EndColumn](../../aspose.cells/cellarea/endcolumn/) | Ottiene o imposta la colonna finale di quest'area. |
| [EndRow](../../aspose.cells/cellarea/endrow/) | Ottiene o imposta la riga finale di quest'area. |
| [StartColumn](../../aspose.cells/cellarea/startcolumn/) | Ottiene o imposta la colonna iniziale di quest'area. |
| [StartRow](../../aspose.cells/cellarea/startrow/) | Ottiene o imposta la riga iniziale di quest'area. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellAreaDemo
    {
        public static void CellAreaExample()
        {
            // Crea una nuova Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B5"].PutValue(20);
            worksheet.Cells["B8"].PutValue(50);
            worksheet.Cells["C2"].PutValue(8);
            worksheet.Cells["C7"].PutValue(15);
            worksheet.Cells["C9"].PutValue(30);

            // Crea area di celle
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 10;
            ca.StartColumn = 0;
            ca.EndColumn = 10;

            // Aggiungi una regola di formattazione condizionale al foglio di lavoro
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "30");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Yellow;

            // Salva la cartella di lavoro
            workbook.Save("CellAreaExample.xlsx");
            workbook.Save("CellAreaExample.pdf");

            // Dimostra il metodo ToString
            Console.WriteLine(ca.ToString());

            // Dimostra il metodo CompareTo
            CellArea ca2 = new CellArea { StartRow = 0, EndRow = 5, StartColumn = 0, EndColumn = 5 };
            int comparisonResult = ca.CompareTo(ca2);
            Console.WriteLine($"Comparison result: {comparisonResult}");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


