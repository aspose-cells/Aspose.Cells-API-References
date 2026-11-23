---
title: "Style.SetBorder"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Style. Définit les bordures du style"
type: docs
url: /fr/net/aspose.cells/style/setborder/
---
## SetBorder(BorderType, CellBorderType, Color) {#setborder_1}

Définit les bordures du style.

```csharp
public bool SetBorder(BorderType borderType, CellBorderType borderStyle, Color borderColor)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| borderType | BorderType | Les bordure(s) à définir peuvent être une combinaison de [`BorderType`](../../bordertype/). |
| borderStyle | CellBorderType | Le style de la bordure. |
| borderColor | Color | La couleur de la bordure. |

### Valeur de retour

Indique si les paramètres de bordure actuels ont été modifiés.

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleMethodSetBorderWithBorderTypeCellBorderTypeColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            var range = worksheet.Cells.CreateRange("A1:D4");

            Style style = workbook.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.DiagonalDown, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.DiagonalUp, CellBorderType.Thin, Color.Blue);

            StyleFlag flag = new StyleFlag { Borders = true };
            range.ApplyStyle(style, flag);

            workbook.Save("BorderExample.xlsx");
        }
    }
}
```

### Voir aussi

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetBorder(BorderType, CellBorderType, CellsColor) {#setborder}

Définit les bordures du style.

```csharp
public bool SetBorder(BorderType borderType, CellBorderType borderStyle, CellsColor borderColor)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| borderType | BorderType | Les bordure(s) à définir peuvent être une combinaison de [`BorderType`](../../bordertype/). |
| borderStyle | CellBorderType | Le style de la bordure. |
| borderColor | CellsColor | La couleur de la bordure. |

### Valeur de retour

Indique si les paramètres de bordure actuels ont été modifiés.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class StyleMethodSetBorderWithBorderTypeCellBorderTypeCellsCDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données pour le contexte
            worksheet.Cells["A1"].Value = "Border Demo";
            
            try
            {
                // Créer un style
                Style style = workbook.CreateStyle();
                
                // Créer un objet CellsColor en utilisant la méthode de fabrique appropriée
                CellsColor borderColor = workbook.CreateCellsColor();
                borderColor.Color = Color.Green;
                
                // Appeler SetBorder avec les paramètres BorderType, CellBorderType et CellsColor
                bool result = style.SetBorder(
                    BorderType.TopBorder, 
                    CellBorderType.Thick, 
                    borderColor);
                
                // Appliquer le style à une cellule
                worksheet.Cells["A1"].SetStyle(style);
                
                Console.WriteLine("SetBorder method called successfully. Result: " + result);
                
                // Enregistrez le classeur
                workbook.Save("SetBorderDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetBorder: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


