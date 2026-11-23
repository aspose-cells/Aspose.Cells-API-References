---
title: "UnionRange.SetOutlineBorders"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode UnionRange. Définit des bordures de contour autour d'une plage de cellules"
type: docs
url: /fr/net/aspose.cells/unionrange/setoutlineborders/
---
## SetOutlineBorders(CellBorderType[], Color[]) {#setoutlineborders_1}

Définit les bordures extérieures autour d'une plage de cellules.

```csharp
public void SetOutlineBorders(CellBorderType[] borderStyles, Color[] borderColors)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| borderStyles | CellBorderType[] | Styles de bordure. |
| borderColors | Color[] | Couleurs de bordure. |

### Remarques

La longueur de borderStyles et de borderStyles doit être de 4. L'ordre de borderStyles et de borderStyles doit être haut,bas,gauche,droite.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class UnionRangeMethodSetOutlineBordersWithCellBorderTypeAColorArrayDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("Test Data");
            worksheet.Cells["A2"].PutValue("More Data");
            worksheet.Cells["B2"].PutValue("Additional Data");

            // Créer une plage et la convertir en UnionRange
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");
            UnionRange unionRange = worksheet.Cells.CreateRange(range.RefersTo).UnionRanges(new Aspose.Cells.Range[] { range });

            try
            {
                // Définir les styles et les couleurs des bordures pour les quatre côtés
                CellBorderType[] borderStyles = new CellBorderType[]
                {
                    CellBorderType.Thin,    // Top border
                    CellBorderType.Medium,  // Right border
                    CellBorderType.Thick,   // Bottom border
                    CellBorderType.Double   // Left border
                };

                Color[] borderColors = new Color[]
                {
                    Color.Red,     // Top border color
                    Color.Blue,    // Right border color
                    Color.Green,   // Bottom border color
                    Color.Orange   // Left border color
                };

                // Appeler SetOutlineBorders avec les tableaux
                unionRange.SetOutlineBorders(borderStyles, borderColors);

                Console.WriteLine("SetOutlineBorders method called successfully with CellBorderType[] and Color[] parameters");
                Console.WriteLine($"Applied borders to range: {unionRange.RefersTo}");

                // Enregistrez le classeur
                workbook.Save("SetOutlineBordersDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOutlineBorders: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [CellBorderType](../../cellbordertype/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorders(CellBorderType, Color) {#setoutlineborders}

Définit les bordures extérieures autour d'une plage de cellules avec le même style et la même couleur de bordure.

```csharp
public void SetOutlineBorders(CellBorderType borderStyle, Color borderColor)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| borderStyle | CellBorderType | Style de bordure. |
| borderColor | Color | Couleur de bordure. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class UnionRangeMethodSetOutlineBordersWithCellBorderTypeColorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Test";
            worksheet.Cells["A2"].Value = "More Data";
            worksheet.Cells["B2"].Value = "Example";

            try
            {
                // Créez un UnionRange couvrant A1:B2
                UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2")
                    .UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

                // Définir les bordures de contour avec un type de bordure et une couleur spécifiques
                unionRange.SetOutlineBorders(CellBorderType.Medium, Color.Blue);

                Console.WriteLine("SetOutlineBorders method called successfully");
                Console.WriteLine($"Border applied to range: {unionRange.RefersTo}");

                // Enregistrez le classeur
                workbook.Save("SetOutlineBordersDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOutlineBorders: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [CellBorderType](../../cellbordertype/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


