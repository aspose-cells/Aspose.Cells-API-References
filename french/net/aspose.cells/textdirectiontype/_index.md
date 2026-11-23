---
title: "Énumération TextDirectionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.TextDirectionType. Représente la direction du flux de texte pour ce paragraphe"
type: docs
url: /fr/net/aspose.cells/textdirectiontype/
---
## TextDirectionType enumeration

Représente la direction du flux de texte pour ce paragraphe.

```csharp
public enum TextDirectionType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Context | `0` |  |
| LeftToRight | `1` |  |
| RightToLeft | `2` |  |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassTextDirectionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir la direction du texte de droite à gauche
            Style style = cells["A1"].GetStyle();
            style.TextDirection = TextDirectionType.RightToLeft;
            cells["A1"].SetStyle(style);
            cells["A1"].PutValue("Right to Left Text");

            // Définir la direction du texte de gauche à droite
            style = cells["A2"].GetStyle();
            style.TextDirection = TextDirectionType.LeftToRight;
            cells["A2"].SetStyle(style);
            cells["A2"].PutValue("Left to Right Text");

            // Définir la direction du texte du contexte
            style = cells["A3"].GetStyle();
            style.TextDirection = TextDirectionType.Context;
            cells["A3"].SetStyle(style);
            cells["A3"].PutValue("Context Text Direction");

            workbook.Save("TextDirectionTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


