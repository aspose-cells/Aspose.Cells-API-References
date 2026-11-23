---
title: "Style.TextDirection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Représente l'ordre de lecture du texte"
type: docs
url: /fr/net/aspose.cells/style/textdirection/
---
## Style.TextDirection property

Représente l'ordre de lecture du texte.

```csharp
public TextDirectionType TextDirection { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyTextDirectionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir différentes directions de texte
            Style style1 = cells["A1"].GetStyle();
            style1.TextDirection = TextDirectionType.Context;
            cells["A1"].SetStyle(style1);
            cells["A1"].PutValue("Context Direction");

            Style style2 = cells["A2"].GetStyle();
            style2.TextDirection = TextDirectionType.LeftToRight;
            cells["A2"].SetStyle(style2);
            cells["A2"].PutValue("LeftToRight Direction");

            Style style3 = cells["A3"].GetStyle();
            style3.TextDirection = TextDirectionType.RightToLeft;
            cells["A3"].SetStyle(style3);
            cells["A3"].PutValue("RightToLeft Direction");

            // Enregistrez le classeur
            workbook.Save("TextDirectionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [TextDirectionType](../../textdirectiontype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


