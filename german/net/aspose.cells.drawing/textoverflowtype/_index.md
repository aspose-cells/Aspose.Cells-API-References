---
title: "Enum TextOverflowType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.TextOverflowType-Enum. Stellt die Art des vertikalen oder horizontalen Textüberlaufs dar"
type: docs
url: /de/net/aspose.cells.drawing/textoverflowtype/
---
## TextOverflowType enumeration

Stellt die Art des vertikalen oder horizontalen Textüberlaufs dar.

```csharp
public enum TextOverflowType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Clip | `0` | Achten Sie auf obere und untere Barrieren. Geben Sie keinen Hinweis darauf, dass unsichtbarer Text vorhanden ist. |
| Ellipsis | `1` | Achten Sie auf obere und untere Barrieren. Verwenden Sie ein Auslassungszeichen, um anzuzeigen, dass unsichtbarer Text vorhanden ist. Nur für vertikalen Überlauf. |
| Overflow | `2` | Lassen Sie den Text überlaufen und ignorieren Sie obere und untere Barrieren. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DrawingClassTextOverflowTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Fügen Sie dem Diagramm ein Textfeld hinzu
            TextBox textBox = chart.Shapes.AddTextBoxInChart(10, 10, 200, 50);

            // Legen Sie die Eigenschaften des Textfelds fest
            textBox.TextBody.TextAlignment.AutoSize = false;
            textBox.Text = "This is a long text that will demonstrate text overflow handling";
            
            // Legen Sie den Textüberlauftyp fest
            textBox.TextVerticalOverflow = TextOverflowType.Clip;

            // Speichere die Arbeitsmappe
            workbook.Save("TextOverflowTypeDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


