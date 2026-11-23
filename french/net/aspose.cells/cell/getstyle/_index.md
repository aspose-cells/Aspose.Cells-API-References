---
title: "Cell.GetStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Récupère le style de la cellule"
type: docs
url: /fr/net/aspose.cells/cell/getstyle/
---
## GetStyle() {#getstyle}

Obtient le style de la cellule.

```csharp
public Style GetStyle()
```

### Valeur de retour

Objet Style.

### Remarques

Pour modifier le style de la cellule, veuillez appeler la méthode Cell.SetStyle() après avoir modifié l'objet style retourné. Cette méthode est identique à `GetStyle` avec la valeur true pour le paramètre.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetStyleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir différents alignements verticaux pour les cellules
            cells["A1"].PutValue("Bottom Alignment");
            cells["A1"].GetStyle().VerticalAlignment = TextAlignmentType.Bottom;

            cells["A2"].PutValue("Center Alignment");
            cells["A2"].GetStyle().VerticalAlignment = TextAlignmentType.Center;

            cells["A3"].PutValue("Distributed Alignment");
            cells["A3"].GetStyle().VerticalAlignment = TextAlignmentType.Distributed;

            cells["A4"].PutValue("Justify Alignment");
            cells["A4"].GetStyle().VerticalAlignment = TextAlignmentType.Justify;

            cells["A5"].PutValue("Top Alignment");
            cells["A5"].GetStyle().VerticalAlignment = TextAlignmentType.Top;

            // Démontrer la méthode GetStyle()
            Console.WriteLine("A1 Vertical Alignment: " + cells["A1"].GetStyle().VerticalAlignment);
            Console.WriteLine("A2 Vertical Alignment: " + cells["A2"].GetStyle().VerticalAlignment);
            Console.WriteLine("A3 Vertical Alignment: " + cells["A3"].GetStyle().VerticalAlignment);
            Console.WriteLine("A4 Vertical Alignment: " + cells["A4"].GetStyle().VerticalAlignment);
            Console.WriteLine("A5 Vertical Alignment: " + cells["A5"].GetStyle().VerticalAlignment);
        }
    }
}
```

### Voir aussi

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetStyle(bool) {#getstyle_1}

Si checkBorders est vrai, vérifie si les bordures des autres cellules affecteront le style de cette cellule.

```csharp
public Style GetStyle(bool checkBorders)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| checkBorders | Boolean | Vérifier les bordures des autres cellules |

### Valeur de retour

Objet Style.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetStyleWithBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder à une cellule et définir des données d'exemple
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue(123.456);

            // Obtenir le style de la cellule sans hériter de la ligne/colonne (paramètre false)
            Style style = cell.GetStyle(false);
            
            // Modifier le style
            style.Custom = "0.000";
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.None;

            // Appliquer le style modifié à la cellule
            cell.SetStyle(style);

            // Vérifier les modifications du style
            Console.WriteLine("Number Format: " + cell.GetStyle(false).Custom);
            Console.WriteLine("Top Border Style: " + cell.GetStyle(false).Borders[BorderType.TopBorder].LineStyle);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


