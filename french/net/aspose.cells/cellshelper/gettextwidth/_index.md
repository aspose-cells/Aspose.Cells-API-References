---
title: "CellsHelper.GetTextWidth"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CellsHelper. Obtient la largeur du texte en points"
type: docs
url: /fr/net/aspose.cells/cellshelper/gettextwidth/
---
## CellsHelper.GetTextWidth method

Obtient la largeur du texte en points.

```csharp
public static double GetTextWidth(string text, Font font, double scaling)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| texte | String | Le texte. |
| police | Police | La police du texte. |
| mise à l'échelle | Double | La mise à l'échelle du texte. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodGetTextWidthWithStringFontDoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Font font = workbook.DefaultStyle.Font;
            double textWidth = CellsHelper.GetTextWidth("Sample Text", font, 1.0);
            Console.WriteLine("Text width: " + textWidth);
        }
    }
}
```

### Voir aussi

* class [Font](../../font/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


