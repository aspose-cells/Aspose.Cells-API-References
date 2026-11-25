---
title: "Classe PivotTableFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Pivot.PivotTableFormat. Rappresenta il formato definito nella PivotTable"
type: docs
url: /it/net/aspose.cells.pivot/pivottableformat/
---
## PivotTableFormat class

Rappresenta il formato definito nella PivotTable.

```csharp
public class PivotTableFormat
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [PivotArea](../../aspose.cells.pivot/pivottableformat/pivotarea/) { get; } | Ottiene l'area pivot. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetStyle](../../aspose.cells.pivot/pivottableformat/getstyle/)() | Ottiene lo stile formattato. |
| [SetStyle](../../aspose.cells.pivot/pivottableformat/setstyle/)(Style) | Imposta lo stile dell'area pivot. |

### Esempi

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotTableFormatDemo
    {
        public static void RunDemo()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["B3"].PutValue(30);

            // Aggiungi una tabella pivot
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount

            // Accedi a PivotTableFormatCollection
            PivotTableFormatCollection pivotFormats = pivotTable.PivotFormats;

            // Aggiungi un nuovo formato alla collezione
            int formatIndex = pivotFormats.Add();
            PivotTableFormat pivotFormat = pivotFormats[formatIndex];

            // Accedi all'area PivotArea del formato
            PivotArea pivotArea = pivotFormat.PivotArea;
            pivotArea.AxisType = PivotFieldType.Data;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;

            // Crea un nuovo stile
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            // Applica lo stile al PivotTableFormat
            pivotFormat.SetStyle(style);

            // Salva la cartella di lavoro
            workbook.Save("PivotTableFormatDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


