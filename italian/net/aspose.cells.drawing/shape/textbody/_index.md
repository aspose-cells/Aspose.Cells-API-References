---
title: "Shape.TextBody"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene e imposta la configurazione del testo della forma"
type: docs
url: /it/net/aspose.cells.drawing/shape/textbody/
---
## Shape.TextBody property

Ottiene e imposta l'impostazione del testo della forma.

```csharp
public FontSettingCollection TextBody { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextBodyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 200);
            FontSettingCollection fontSettingCollection = shape.TextBody;
            fontSettingCollection.Text = "This is a test.";

            workbook.Save("ShapeTextBodyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FontSettingCollection](../../../aspose.cells.drawing.texts/fontsettingcollection/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


