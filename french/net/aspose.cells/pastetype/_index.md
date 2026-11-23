---
title: "Enum PasteType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.PasteType enum. Représente le type de collage spécial"
type: docs
url: /fr/net/aspose.cells/pastetype/
---
## PasteType enumeration

Représente le type de collage spécial.

```csharp
public enum PasteType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| All | `0` | Copie toutes les données de la plage. |
| Default | `1` | Il fonctionne comme le comportement "All" de MS Excel. |
| AllExceptBorders | `2` | Copie toutes les données de la plage sans la plage. |
| DefaultExceptBorders | `3` | Il fonctionne comme le comportement "All except borders" de MS Excel. |
| ColumnWidths | `4` | Copie uniquement les largeurs de la plage. |
| RowHeights | `5` | Copie uniquement les hauteurs de la plage. |
| Comments | `6` | Copie uniquement les commentaires dans la plage. |
| Formats | `7` | Copie uniquement les formats dans la plage. |
| Formulas | `8` | Copie uniquement les formules dans la plage. |
| FormulasAndNumberFormats | `9` | Copie uniquement les formules et les formats numériques dans la plage. |
| Validation | `10` | Copie uniquement les validations dans la plage. |
| Values | `11` | Copie uniquement les valeurs dans la plage. |
| ValuesAndFormats | `12` | Copie uniquement les valeurs et les formats dans la plage. |
| ValuesAndNumberFormats | `13` | Copie uniquement les valeurs et les formats numériques dans la plage. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PasteTypeDemo
    {
        public static void PasteTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Définir la plage source
            Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:B4");

            // Définir la plage de destination
            Aspose.Cells.Range destinationRange = worksheet.Cells.CreateRange("D1:E4");

            // Créer PasteOptions et définir le PasteType
            PasteOptions pasteOptions = new PasteOptions
            {
                PasteType = PasteType.Values,
                SkipBlanks = true,
                OnlyVisibleCells = false,
                Transpose = false,
                IgnoreLinksToOriginalFile = true
            };

            // Copier la plage source vers la plage de destination avec les options de collage spécifiées
            destinationRange.Copy(sourceRange, pasteOptions);

            // Enregistrez le classeur
            workbook.Save("PasteTypeExample.xlsx");

            // Afficher les résultats
            Console.WriteLine("Data copied with PasteType.Values and saved to PasteTypeExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


