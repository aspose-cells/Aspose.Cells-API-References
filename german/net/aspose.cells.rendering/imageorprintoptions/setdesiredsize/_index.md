---
title: "ImageOrPrintOptions.SetDesiredSize"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions-Methode. Legt die gewünschte Breite und Höhe des Bildes fest"
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/setdesiredsize/
---
## SetDesiredSize(int, int) {#setdesiredsize}

Legt die gewünschte Breite und Höhe des Bildes fest.

```csharp
[Obsolete("Use SetDesiredSize(int, int, bool) by setting param keepAspectRatio to false instead.")]
public void SetDesiredSize(int desiredWidth, int desiredHeight)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| desiredWidth | Int32 | gewünschte Breite in Pixeln |
| desiredHeight | Int32 | gewünschte Höhe in Pixeln |

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen `SetDesiredSize`, indem Sie den Parameter keepAspectRatio auf false setzen. Diese Eigenschaft wird 12 Monate später, seit Mai 2023, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsMethodSetDesiredSizeWithInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Sample Data");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue(i);
            }

            // Druckbereich festlegen
            worksheet.PageSetup.PrintArea = "A1:A11";

            // Bildoptionen erstellen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;
            options.SetDesiredSize(800, 600); // Using SetDesiredSize with Int32 parameters
            options.ImageType = Aspose.Cells.Drawing.ImageType.Jpeg;

            // Render das Arbeitsblatt zu einem Bild
            SheetRender render = new SheetRender(worksheet, options);
            render.ToImage(0, "output.jpg");

            Console.WriteLine("Image generated with desired size 800x600");
        }
    }
}
```

### Siehe auch

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## SetDesiredSize(int, int, bool) {#setdesiredsize_1}

Legt die gewünschte Breite und Höhe des Bildes fest.

```csharp
public void SetDesiredSize(int desiredWidth, int desiredHeight, bool keepAspectRatio)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| desiredWidth | Int32 | gewünschte Breite in Pixeln |
| desiredHeight | Int32 | gewünschte Höhe in Pixeln |
| keepAspectRatio | Boolean | ob das Seitenverhältnis des Originalbildes beibehalten werden soll |

### Hinweise

Die Breite und Höhe des Ausgabebildes in Pixeln basieren ausschließlich auf der festgelegten gewünschten Breite und Höhe.

Die [`HorizontalResolution`](../horizontalresolution/) und [`VerticalResolution`](../verticalresolution/) wirken sich in diesem Fall nicht auf die Breite und Höhe des Ausgabebildes aus.

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsMethodSetDesiredSizeWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten hinzufügen und ein Diagramm erstellen
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries.CategoryData = "B1:B3";

            // Rufen Sie die Diagrammform ab
            Shape chartShape = worksheet.Shapes[0];

            // Lege Bildoptionen fest
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png;
            options.SetDesiredSize(800, 600, false); // Using SetDesiredSize with width, height, and keepAspectRatio

            // Speichern Sie das Diagramm als Bild
            MemoryStream stream = new MemoryStream();
            chartShape.ToImage(stream, options);

            // Speichere das Bild in einer Datei
            File.WriteAllBytes("output_chart.png", stream.ToArray());
        }
    }
}
```

### Siehe auch

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


