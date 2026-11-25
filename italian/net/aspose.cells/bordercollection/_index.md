---
title: "Classe BorderCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.BorderCollection. Incapsula una raccolta di oggetti Border"
type: docs
url: /it/net/aspose.cells/bordercollection/
---
## BorderCollection class

Incapsula una raccolta di oggetti [`Border`](../border/).

```csharp
public class BorderCollection
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DiagonalColor](../../aspose.cells/bordercollection/diagonalcolor/) { get; set; } | Ottiene o imposta il Color delle linee diagonali. |
| [DiagonalStyle](../../aspose.cells/bordercollection/diagonalstyle/) { get; set; } | Ottiene o imposta lo stile delle linee diagonali. |
| [IsOutline](../../aspose.cells/bordercollection/isoutline/) { get; set; } | Indica se i bordi sinistro, destro, superiore e inferiore devono essere applicati solo ai bordi esterni di un intervallo di celle. Il valore predefinito è true. |
| [Item](../../aspose.cells/bordercollection/item/) { get; } | Ottiene l'elemento [`Border`](../border/) all'indice specificato. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetColor](../../aspose.cells/bordercollection/setcolor/)(Color) | Imposta il Color di tutti i bordi nella raccolta. |
| [SetStyle](../../aspose.cells/bordercollection/setstyle/)(CellBorderType) | Imposta lo stile di tutti i bordi della raccolta. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BorderCollectionDemo
    {
        public static void BorderCollectionExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();

            // Aggiungere un nuovo foglio di lavoro all'oggetto Workbook
            workbook.Worksheets.Add();

            // Ottenere il riferimento del foglio di lavoro appena aggiunto passando il suo indice di foglio
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedere alla cella "A1" dal foglio di lavoro
            Cell cell = worksheet.Cells["A1"];

            // Aggiungere un valore alla cella "A1"
            cell.PutValue("Visit Aspose!");

            // Ottenere lo stile della cella
            Style style = cell.GetStyle();

            // Impostare lo stile della linea del bordo superiore
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;

            // Impostare il colore del bordo superiore
            style.Borders[BorderType.TopBorder].Color = Color.Red;

            // Impostare lo stile della linea del bordo inferiore
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thick;

            // Impostare il colore del bordo inferiore
            style.Borders[BorderType.BottomBorder].Color = Color.Green;

            // Impostare lo stile della linea del bordo sinistro
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dashed;

            // Impostare il colore del bordo sinistro
            style.Borders[BorderType.LeftBorder].Color = Color.Yellow;

            // Impostare lo stile della linea del bordo destro
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Dotted;

            // Impostare il colore del bordo destro
            style.Borders[BorderType.RightBorder].Color = Color.Blue;

            // Impostare le proprietà diagonali
            style.Borders.DiagonalColor = Color.Red;
            style.Borders.DiagonalStyle = CellBorderType.Dashed;

            // Applicare lo stile alla cella
            cell.SetStyle(style);

            // Salvataggio del file Excel
            workbook.Save("BorderCollectionExample.xlsx");
            workbook.Save("BorderCollectionExample.pdf");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


