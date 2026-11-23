---
title: "Cells.GetCellDisplayStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Obtient le style d'affichage de la cellule donnée"
type: docs
url: /fr/net/aspose.cells/cells/getcelldisplaystyle/
---
## GetCellDisplayStyle(int, int) {#getcelldisplaystyle}

Obtient le style d'affichage de la cellule donnée.

```csharp
public Style GetCellDisplayStyle(int row, int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | indice de ligne de la cellule donnée |
| column | Int32 | colonne de la cellule donnée |

### Valeur de retour

le style d'affichage de la cellule donnée.

### Remarques

Identique avec [`GetDisplayStyle`](../../cell/getdisplaystyle/), et idem en utilisant SideBorders pour `GetCellDisplayStyle`.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetCellDisplayStyleWithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Préparez le style de cellule pour la démonstration
            Cell cell = cells[0, 0];
            cell.PutValue("Style Demo");
            
            // Créez un style personnalisé
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            
            // Appliquez le style à la cellule
            cell.SetStyle(style);

            try
            {
                // Appelez GetCellDisplayStyle avec la ligne 0 et la colonne 0
                Style displayStyle = cells.GetCellDisplayStyle(0, 0);

                // Propriétés du style d'affichage
                Console.WriteLine($"Bold: {displayStyle.Font.IsBold}");
                Console.WriteLine($"Background Color: {displayStyle.ForegroundColor}");

                // Appliquez le style d'affichage à une autre cellule pour une vérification visuelle
                cells[2, 2].SetStyle(displayStyle);
                cells[2, 2].PutValue("Style Copied");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellDisplayStyle method: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("CellsMethodGetCellDisplayStyleWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetCellDisplayStyle(int, int, BorderType) {#getcelldisplaystyle_1}

Obtient le style d'affichage de la cellule donnée.

```csharp
public Style GetCellDisplayStyle(int row, int column, BorderType adjacentBorders)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | indice de ligne de la cellule donnée |
| column | Int32 | colonne de la cellule donnée |
| adjacentBorders | BorderType | Indique quelles bordures doivent être vérifiées et ajustées en fonction des bordures des cellules adjacentes. Veuillez consulter la description du même paramètre de [`GetDisplayStyle`](../../cell/getdisplaystyle/). |

### Valeur de retour

le style d'affichage de la cellule donnée.

### Remarques

Si la cellule est également affectée par d’autres paramètres tels que le formatage conditionnel, les objets de liste, etc., alors le style d’affichage peut différer de [`GetCellStyle`](../getcellstyle/). Et comme ces paramètres peuvent également être appliqués aux cellules vides (inexistantes), l’utilisation de cette méthode peut éviter l’instanciation de ces cellules vides, de sorte que les performances seront meilleures que d’obtenir l’instance Cell depuis Cells puis d’appeler [`GetDisplayStyle`](../../cell/getdisplaystyle/).

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetCellDisplayStyleWithInt32Int32BorderTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accédez à la cellule A1 et définissez un style de bordure
            Cell cell = worksheet.Cells["A1"];
            Style style = cell.GetStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;
            cell.SetStyle(style);

            try
            {
                // Appelez GetCellDisplayStyle avec des paramètres spécifiques (0,0 pour A1, type TopBorder)
                Style displayStyle = worksheet.Cells.GetCellDisplayStyle(0, 0, BorderType.TopBorder);

                // Vérifiez si le style récupéré correspond à notre couleur de bordure
                if (displayStyle.Borders[BorderType.TopBorder].Color == System.Drawing.Color.Red)
                {
                    Console.WriteLine("Top border display style retrieved successfully - Color: Red");
                }

                // Démontrez l’application du style en modifiant une autre cellule
                Cell targetCell = worksheet.Cells["B1"];
                targetCell.SetStyle(displayStyle);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellDisplayStyle method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("GetCellDisplayStyleWithBorderTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../../style/)
* enum [BorderType](../../bordertype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


