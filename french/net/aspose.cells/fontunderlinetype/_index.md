---
title: "Enum FontUnderlineType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.FontUnderlineType enum. Énumère les types de soulignement de police"
type: docs
url: /fr/net/aspose.cells/fontunderlinetype/
---
## FontUnderlineType enumeration

Énumère les types de soulignement de police.

```csharp
public enum FontUnderlineType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Représente aucun soulignement. |
| Single | `1` | Représente un soulignement simple. |
| Double | `2` | Représente un double soulignement. |
| Accounting | `3` | Représente un soulignement comptable simple. |
| DoubleAccounting | `4` | Représente un double soulignement comptable. |
| Dash | `5` | Représente le soulignement pointillé |
| DashDotDotHeavy | `6` | Représente le soulignement épais tiret-point-point |
| DashDotHeavy | `7` | Représente le soulignement épais tiret-point |
| DashedHeavy | `8` | Représente le soulignement épais en tirets |
| DashLong | `9` | Représente le soulignement long en tirets |
| DashLongHeavy | `10` | Représente le soulignement épais long en tirets |
| DotDash | `11` | Représente le soulignement tiret-point |
| DotDotDash | `12` | Représente le soulignement tiret-point-point |
| Dotted | `13` | Représente le soulignement pointillé |
| DottedHeavy | `14` | Représente le soulignement épais pointillé |
| Heavy | `15` | Représente le soulignement épais |
| Wave | `16` | Représente le soulignement en vague |
| WavyDouble | `17` | Représente le double soulignement en vague |
| WavyHeavy | `18` | Représente le soulignement ondulé épais |
| Words | `19` | Représente le soulignement des caractères non espaces. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontUnderlineTypeDemo
    {
        public static void FontUnderlineTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Obtenez la référence de la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accès à la cellule "A1" de la feuille de calcul
            Cell cell = worksheet.Cells["A1"];
            
            // Ajout d'une valeur à la cellule "A1"
            cell.PutValue("Hello Aspose!");

            // Obtenir le style de la cellule
            Style style = cell.GetStyle();
            
            // Définir le type de soulignement de la police sur un soulignement simple
            style.Font.Underline = FontUnderlineType.Single;
            
            // Appliquez le style à la cellule
            cell.SetStyle(style);

            // Enregistrez le classeur
            workbook.Save("FontUnderlineTypeExample.xlsx");
            workbook.Save("FontUnderlineTypeExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


