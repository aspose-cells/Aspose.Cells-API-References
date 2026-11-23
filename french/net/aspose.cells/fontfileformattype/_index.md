---
title: "Enum FontFileFormatType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.FontFileFormatType. Représente le type de format de police"
type: docs
url: /fr/net/aspose.cells/fontfileformattype/
---
## FontFileFormatType enumeration

Représente le type de format de police.

```csharp
public enum FontFileFormatType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Unknown | `0` | Type de format de police inconnu. |
| Ttf | `1` | Type de format de police TTF. |
| Otf | `2` | Type de format de police OTF. |
| Ttc | `3` | Type de format de police TTC. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassFontFileFormatTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder à une cellule et définir son style
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Font Format Type Demo");
            Style style = cell.GetStyle();

            // Démontrer l'utilisation de FontFileFormatType
            FontFileFormatType fontFormat = FontFileFormatType.Ttf;
            Console.WriteLine("Selected font format: " + fontFormat.ToString());

            // Appliquer les paramètres de police
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            cell.SetStyle(style);

            // Vérifier la compatibilité du format de police
            if (fontFormat == FontFileFormatType.Ttf)
            {
                Console.WriteLine("Using TrueType font format");
            }

            // Enregistrez le classeur
            workbook.Save("FontFileFormatTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


