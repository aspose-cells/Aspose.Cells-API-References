---
title: "Style.Style"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur Style. Initialise une nouvelle instance de la classe Style"
type: docs
url: /fr/net/aspose.cells/style/style/
---
## Style constructor

Initialise une nouvelle instance de la classe [`Style`](../).

```csharp
[Obsolete("Use CellsFactory.CreateStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Style()
```

### Remarques

NOTE : Ce constructeur est maintenant obsolète. À la place, veuillez utiliser la méthode CellsFactory.CreateStyle() method. Cette propriété sera supprimée 6 mois plus tard depuis octobre 2016. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodCtorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez un style en utilisant le constructeur
            Style style = new Style();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Red;
            style.Pattern = BackgroundType.Solid;

            // Appliquer le style à une cellule
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Styled Text");
            cell.SetStyle(style);

            // Enregistrez le classeur
            workbook.Save("StyleConstructorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


