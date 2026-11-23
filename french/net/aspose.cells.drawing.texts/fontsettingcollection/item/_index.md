---
title: "FontSettingCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FontSettingCollection. Obtient le FontSetting par l'index"
type: docs
url: /fr/net/aspose.cells.drawing.texts/fontsettingcollection/item/
---
## FontSettingCollection indexer

Obtient le [`FontSetting`](../../../aspose.cells/fontsetting/) par l'index.

```csharp
public FontSetting this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice. |

### Exemples

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

            // Définir les propriétés de police pour des caractères spécifiques
            Aspose.Cells.Font fo = tb.Characters(3, 5).Font;
            fo.IsSuperscript = true;
            fo.Color = Color.Red;

            // Accéder à la police via la propriété TextBody.Item
            Aspose.Cells.Font fo1 = tb.TextBody[3].Font;
            Console.WriteLine("IsSuperscript: " + fo1.IsSuperscript);
            Console.WriteLine("Color: " + fo1.Color);

            w.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


