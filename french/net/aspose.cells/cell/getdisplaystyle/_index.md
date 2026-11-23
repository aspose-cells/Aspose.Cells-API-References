---
title: "Cell.GetDisplayStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Obtient le style d'affichage de cette cellule"
type: docs
url: /fr/net/aspose.cells/cell/getdisplaystyle/
---
## GetDisplayStyle() {#getdisplaystyle}

Obtient le style d'affichage de cette cellule.

```csharp
public Style GetDisplayStyle()
```

### Valeur de retour

style d'affichage de cette cellule

### Remarques

Identique à l'utilisation de SideBorders pour `GetDisplayStyle`. Ainsi, cette méthode vérifiera et ajustera les bordures haut/bas/gauche/droite de cette cellule selon le style ([`GetStyle`](../getstyle/)) de ses cellules adjacentes, mais ne vérifiera pas les cellules fusionnées et ne vérifiera pas le style d'affichage des cellules adjacentes.

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellMethodGetDisplayStyleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir le style pour la cellule A1
            Style style1 = workbook.CreateStyle();
            style1.ForegroundColor = Color.FromArgb(157, 195, 230);
            worksheet.Cells["A1"].SetStyle(style1);
            
            // Définir le style pour la cellule A23
            Style style2 = workbook.CreateStyle();
            style2.ForegroundColor = Color.Red;
            worksheet.Cells["A23"].SetStyle(style2);
            
            // Obtenir et afficher les styles
            Style displayStyle1 = worksheet.Cells["A1"].GetDisplayStyle();
            Console.WriteLine("A1 Foreground Color: " + displayStyle1.ForegroundColor);
            
            Style displayStyle2 = worksheet.Cells["A23"].GetDisplayStyle();
            Console.WriteLine("A23 Foreground Color: " + displayStyle2.ForegroundColor);
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

## GetDisplayStyle(bool) {#getdisplaystyle_2}

Obtient le style d'affichage de cette cellule.

```csharp
public Style GetDisplayStyle(bool includeMergedBorders)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| includeMergedBorders | Boolean | Indique s'il faut vérifier les bordures des cellules fusionnées. |

### Valeur de retour

style d'affichage de cette cellule

### Remarques

Si le drapeau spécifié est false, alors c'est identique à `GetDisplayStyle`. Sinon, c'est identique à l'utilisation de SideBorders&#x7C;DynamicStyleBorders pour `GetDisplayStyle`.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDisplayStyleWithBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accéder à la cellule B2 et définir certaines propriétés de style
            Cell cell = worksheet.Cells["B2"];
            Style cellStyle = cell.GetStyle();
            cellStyle.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            cell.SetStyle(cellStyle);
            
            // Obtenir le style d'affichage avec formatage (paramètre true)
            Style displayStyle = cell.GetDisplayStyle(true);
            
            // Afficher le style de ligne de la bordure droite
            Console.WriteLine("Right Border Line Style: " + displayStyle.Borders[BorderType.RightBorder].LineStyle);
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

## GetDisplayStyle(BorderType) {#getdisplaystyle_1}

Obtient le style d'affichage de cette cellule.

```csharp
public Style GetDisplayStyle(BorderType adjacentBorders)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| adjacentBorders | BorderType | Indique quelles bordures doivent être vérifiées et ajustées selon les bordures des cellules adjacentes. |

### Valeur de retour

style d'affichage de cette cellule

### Remarques

Si cette cellule est également affectée par d'autres paramètres tels que le formatage conditionnel, les objets de liste, etc., le style d'affichage peut différer de [`GetStyle`](../getstyle/). Pour les indicateurs d'ajustement des bordures selon les cellules adjacentes, TopBorder/BottomBorder/LeftBorder/RightBorder indiquent s'il faut vérifier et combiner les bordures inférieure/superérieure/droite/gauche des cellules gauche/droite/haute/basse adjacentes à celle-ci. Pour des raisons de performance et de compatibilité, certaines énumérations sont utilisées pour désigner des opérations spéciales : Horizontal/Vertical indiquent s'il faut vérifier et combiner la bordure inférieure/droite des cellules fusionnées avec celle-ci. Diagonal (c’est‑à‑dire que DiagonalUpBorder et DiagonalDownBorder sont tous deux définis) indique la vérification et la combinaison des bordures provenant du style d'affichage des cellules adjacentes. Veuillez noter que la vérification des bordures/styles des cellules adjacentes, en particulier des styles d'affichage, est un processus gourmand en temps. S'il n'est pas nécessaire d'obtenir les bordures pour le style retourné, utiliser None pour désactiver le traitement des cellules adjacentes améliorera les performances. Lors de la récupération des bordures des cellules adjacentes à partir des styles définis uniquement sur ces cellules (sans définir Diagonal), les performances peuvent également être meilleures car la vérification du style d'affichage d'une cellule est également coûteuse.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDisplayStyleWithBorderTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Définir des données d'exemple
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue(i);
            }

            // Créer une mise en forme conditionnelle
            FormatConditionCollection fcs = sheet.ConditionalFormattings[sheet.ConditionalFormattings.Add()];
            fcs.AddArea(CellArea.CreateCellArea(0, 0, 9, 0));
            fcs.AddCondition(FormatConditionType.ColorScale);

            // Obtenir le style d'affichage avec différents types de bordure
            for (int i = 0; i < 10; i++)
            {
                Style styleWithBorder = cells[i, 0].GetDisplayStyle(BorderType.TopBorder);
                Style styleWithoutBorder = cells[i, 0].GetDisplayStyle(BorderType.None);

                Console.WriteLine($"Cell {i + 1}:");
                Console.WriteLine($"  Style with border - Foreground: {styleWithBorder.ForegroundArgbColor:X}");
                Console.WriteLine($"  Style without border - Foreground: {styleWithoutBorder.ForegroundArgbColor:X}");
            }
        }
    }
}
```

### Voir aussi

* class [Style](../../style/)
* enum [BorderType](../../bordertype/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


