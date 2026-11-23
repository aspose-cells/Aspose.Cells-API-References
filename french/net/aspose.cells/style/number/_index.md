---
title: "Style.Number"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Obtient ou définit le format d'affichage des nombres et des dates. Les modèles de formatage diffèrent selon les régions"
type: docs
url: /fr/net/aspose.cells/style/number/
---
## Style.Number property

Obtient ou définit le format d'affichage des nombres et des dates. Les modèles de formatage diffèrent selon les régions.

```csharp
public int Number { get; set; }
```

### Remarques

Par exemple, les modèles de formatage représentés par des nombres pour la région en_US :

| **Value** | **Type** | **Format String** |
| --- | --- | --- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Red]($#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Red]($#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `m/d/yyyy` |
| 15 | Date | `d-mmm-yy` |
| 16 | Date | `d-mmm` |
| 17 | Date | `mmm-yy` |
| 18 | Time | `h:mm AM/PM` |
| 19 | Time | `h:mm:ss AM/PM` |
| 20 | Time | `h:mm` |
| 21 | Time | `h:mm:ss` |
| 22 | Time | `m/d/yyyy h:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[Red](#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Red](#,##0.00)` |
| 41 | Accounting | `_(* #,##0_);_(* (#,##0);_(* "-"_);_(@_)` |
| 42 | Currency | `_($* #,##0_);_($* (#,##0);_($* "-"_);_(@_)` |
| 43 | Accounting | `_(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_)` |
| 44 | Currency | `_($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_)` |
| 45 | Time | `mm:ss` |
| 46 | Time | `[h]:mm:ss` |
| 47 | Time | `mm:ss.0` |
| 48 | Scientific | `##0.0E+0` |
| 49 | Text | `@` |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyNumberDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accéder à une cellule et obtenir son style
            Cell cell = worksheet.Cells["A1"];
            Style style = cell.GetStyle();
            
            // Définir le format numérique
            style.Number = 5; // 5 represents the "0.00" number format
            cell.SetStyle(style);
            
            // Définir une valeur numérique pour démontrer le formatage
            cell.PutValue(123.456);
            
            // Enregistrez le classeur
            workbook.Save("NumberFormatDemo.xlsx");
            
            Console.WriteLine("Number format demonstration completed.");
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


