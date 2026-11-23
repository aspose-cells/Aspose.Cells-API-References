---
title: "Row.SetStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Row. Définit le style de cette ligne"
type: docs
url: /fr/net/aspose.cells/row/setstyle/
---
## Row.SetStyle method

Définit le style de cette ligne.

```csharp
public void SetStyle(Style style)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| style | Style | le style à utiliser comme style par défaut pour les cellules de cette ligne. |

### Remarques

Cette méthode ne fait que définir le style donné comme style par défaut pour cette ligne, sans modifier les paramètres de style des cellules existantes dans cette ligne. Pour mettre à jour les paramètres de style des cellules existantes avec le style spécifié en même temps, veuillez utiliser [`ApplyStyle`](../applystyle/)

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RowMethodSetStyleWithStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer et configurer un style
            Style style = workbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.Blue;
            style.ForegroundColor = System.Drawing.Color.Red;
            style.Pattern = BackgroundType.DiagonalStripe;

            // Obtenir la première ligne et appliquer le style
            Row row = worksheet.Cells.Rows[0];
            row.SetStyle(style);

            // Enregistrez le classeur
            workbook.Save("RowStyleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../../style/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


