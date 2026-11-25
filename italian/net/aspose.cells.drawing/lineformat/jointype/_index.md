---
title: "LineFormat.JoinType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LineFormat. Specifica il tipo di giunzione della linea"
type: docs
url: /it/net/aspose.cells.drawing/lineformat/jointype/
---
## LineFormat.JoinType property

Specifica il tipo di unione della linea.

```csharp
public LineJoinType JoinType { get; set; }
```

### Esempi

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyJoinTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una forma linea
            LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Imposta il tipo di giunzione della linea su Arrotondato
            line.Line.JoinType = LineJoinType.Round;

            // Salva la cartella di lavoro
            workbook.Save("LineJoinTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [LineJoinType](../../linejointype/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


