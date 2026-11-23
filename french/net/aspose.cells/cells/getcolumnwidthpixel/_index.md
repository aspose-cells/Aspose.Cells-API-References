---
title: "Cells.GetColumnWidthPixel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Obtient la largeur de la colonne spécifiée en vue normale, en unités de pixel"
type: docs
url: /fr/net/aspose.cells/cells/getcolumnwidthpixel/
---
## GetColumnWidthPixel(int) {#getcolumnwidthpixel}

Obtient la largeur de la colonne spécifiée en vue normale, en unités de pixels.

```csharp
public int GetColumnWidthPixel(int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| column | Int32 | Indice de colonne |

### Valeur de retour

Largeur de la colonne en vue normale.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetColumnWidthPixelWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir la largeur de la colonne en caractères (sera convertie en pixels)
            worksheet.Cells.SetColumnWidth(1, 25);
            
            // Obtenir la largeur de la colonne en pixels
            int widthInPixels = worksheet.Cells.GetColumnWidthPixel(1);
            
            // Afficher le résultat
            Console.WriteLine("Column width in pixels: " + widthInPixels);
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetColumnWidthPixel(int, bool) {#getcolumnwidthpixel_1}

Obtient la largeur de la colonne spécifiée en vue normale, en unités de pixels.

```csharp
[Obsolete("Use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int GetColumnWidthPixel(int column, bool original)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| column | Int32 | Indice de colonne |
| original | Boolean | Indique s'il faut renvoyer la largeur originale même lorsque la colonne est masquée |

### Valeur de retour

Largeur de la colonne en vue normale.

### Remarques

REMARQUE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode Cells.GetColumnWidth(int ,bool , CellsUnitType ). Cette méthode sera supprimée 12 mois après avril 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetColumnWidthPixelWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir la largeur de colonne standard à 80 pixels
            worksheet.Cells.StandardWidthPixels = 80;

            // Définir la largeur de colonne spécifique pour la colonne 2 (troisième colonne) à 120 pixels
            worksheet.Cells.SetColumnWidthPixel(2, 120);

            try
            {
                // Obtenir la largeur actuelle avec les modifications de l'utilisateur (original : false)
                int currentWidth = worksheet.Cells.GetColumnWidthPixel(2, false);
                Console.WriteLine($"Column 2 current width: {currentWidth} pixels");

                // Obtenir la largeur originale sans modifications (original : true)
                int originalWidth = worksheet.Cells.GetColumnWidthPixel(2, true);
                Console.WriteLine($"Column 2 original width: {originalWidth} pixels");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetColumnWidthPixel: {ex.Message}");
            }

            // Enregistrer le classeur pour démontrer la persistance de la largeur de colonne
            workbook.Save("ColumnWidthDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


