---
title: "FontSettingCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FontSettingCollection. Obtiene el FontSetting por el índice"
type: docs
url: /es/net/aspose.cells.drawing.texts/fontsettingcollection/item/
---
## FontSettingCollection indexer

Obtiene el [`FontSetting`](../../../aspose.cells/fontsetting/) por el índice.

```csharp
public FontSetting this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FontSettingCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook w = new Workbook();
            Worksheet s = w.Worksheets[0];

            Shape tb = s.Shapes.AddTextBox(3, 0, 7, 0, 70, 300);
            tb.Text = "Sample Text";

            // Establecer propiedades de fuente para caracteres específicos
            Aspose.Cells.Font fo = tb.Characters(3, 5).Font;
            fo.IsSuperscript = true;
            fo.Color = Color.Red;

            // Acceder a la fuente mediante la propiedad TextBody.Item
            Aspose.Cells.Font fo1 = tb.TextBody[3].Font;
            Console.WriteLine("IsSuperscript: " + fo1.IsSuperscript);
            Console.WriteLine("Color: " + fo1.Color);

            w.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


