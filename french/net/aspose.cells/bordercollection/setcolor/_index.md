---
title: "BorderCollection.SetColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode BorderCollection. Définit la Color de toutes les bordures de la collection"
type: docs
url: /fr/net/aspose.cells/bordercollection/setcolor/
---
## BorderCollection.SetColor method

Définit la Couleur de toutes les bordures de la collection.

```csharp
public void SetColor(Color color)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| color | Color | Color des bordures. |

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderCollectionMethodSetColorWithColorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un style avec des bordures colorées
            Style style = workbook.CreateStyle();
            
            // Définir les styles de lignes de bordure
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

            // Définir la couleur de la bordure en rouge en utilisant la méthode SetColor
            style.Borders.SetColor(Color.Red);

            // Appliquer le style à une cellule
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Cell with colored borders");
            cell.SetStyle(style);

            // Ajuster automatiquement la colonne pour une meilleure visibilité
            worksheet.AutoFitColumn(0);

            // Enregistrez le classeur
            workbook.Save("BorderColorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


