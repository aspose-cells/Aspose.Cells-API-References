---
title: "UnionRange.FirstColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà UnionRange. Restituisce l'indice della prima colonna dell'intervallo"
type: docs
url: /it/net/aspose.cells/unionrange/firstcolumn/
---
## UnionRange.FirstColumn property

Ottiene l'indice della prima colonna dell'intervallo.

```csharp
public int FirstColumn { get; }
```

### Osservazioni

Ha effetto solo quando contiene un solo intervallo.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyFirstColumnDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola alcuni dati
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["C1"].PutValue("Header3");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["C2"].PutValue("Data3");

            // Crea un intervallo di unione
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:C1");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A2:C2");
            UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

            // Visualizza la proprietà FirstColumn
            Console.WriteLine("First column index of the union range: " + unionRange.FirstColumn);

            // Dimostra l'uso di FirstColumn nelle operazioni
            Console.WriteLine("First column name: " + CellsHelper.ColumnIndexToName(unionRange.FirstColumn));

            // Applica la formattazione alla prima colonna dell'intervallo di unione
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightGray;
            style.Pattern = BackgroundType.Solid;

            Aspose.Cells.Range firstColumnRange = worksheet.Cells.CreateRange(
                unionRange.FirstRow, unionRange.FirstColumn,
                unionRange.RowCount, 1);
            firstColumnRange.ApplyStyle(style, new StyleFlag { FontBold = true, CellShading = true });

            // Salva il risultato
            workbook.Save("UnionRangePropertyFirstColumnDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


