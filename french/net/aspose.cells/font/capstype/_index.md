---
title: "Font.CapsType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Font. Obtient et définit le type de majuscules du texte"
type: docs
url: /fr/net/aspose.cells/font/capstype/
---
## Font.CapsType property

Obtient et définit le type de majuscules du texte.

```csharp
[Obsolete("Use TextOptions.CapsType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public TextCapsType CapsType { get; set; }
```

### Remarques

Uniquement pour les polices des Formes ou des Graphiques. NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété [`CapsType`](../../../aspose.cells.drawing.texts/textoptions/capstype/). Cette propriété sera supprimée 12 mois plus tard, à partir de janvier 2026. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyCapsTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("sample text");

            Style style = cell.GetStyle();
            style.Font.CapsType = TextCapsType.All;
            cell.SetStyle(style);

            workbook.Save("FontCapsTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [TextCapsType](../../textcapstype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


