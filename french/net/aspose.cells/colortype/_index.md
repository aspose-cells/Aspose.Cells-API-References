---
title: "Enumération ColorType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enumération Aspose.Cells.ColorType. Représente tous les types de couleur"
type: docs
url: /fr/net/aspose.cells/colortype/
---
## ColorType enumeration

Représente tous les types de couleur

```csharp
public enum ColorType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Automatic | `0` | Couleur automatique. |
| AutomaticIndex | `1` | C'est une couleur automatique, mais la couleur affichée dépend du paramètre du système d'exploitation. |
| RGB | `2` | La couleur RVB. |
| IndexedColor | `3` | L'index de couleur dans la palette de couleurs. |
| Theme | `4` | La couleur du thème. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassColorTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Créez un nouveau classeur pour la démonstration
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Démontrer l'utilisation des valeurs d'énumération ColorType
                ColorType automatic = ColorType.Automatic;
                ColorType rgb = ColorType.RGB;
                ColorType theme = ColorType.Theme;

                // Afficher les valeurs d'énumération
                Console.WriteLine($"Automatic color type value: {(int)automatic}");
                Console.WriteLine($"RGB color type value: {(int)rgb}");
                Console.WriteLine($"Theme color type value: {(int)theme}");

                // Créer une cellule et définir sa valeur
                Cell cell = worksheet.Cells["A1"];
                cell.PutValue("ColorType Demo");

                // Créer un style et l'appliquer à la cellule
                Style style = workbook.CreateStyle();
                style.Font.Color = System.Drawing.Color.Black;
                cell.SetStyle(style);

                // Enregistrez le classeur
                workbook.Save("ColorTypeDemo.xlsx");

                Console.WriteLine("ColorType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in ColorType demonstration: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


