---
title: "Classe CellValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.CellValue. Représente la valeur de la cellule et le type correspondant"
type: docs
url: /fr/net/aspose.cells/cellvalue/
---
## CellValue class

Représente la valeur de la cellule et le type correspondant.

```csharp
public class CellValue
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [CellValue](cellvalue/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Type](../../aspose.cells/cellvalue/type/) { get; set; } | Obtient ou définit le type de la valeur de la cellule. |
| [Value](../../aspose.cells/cellvalue/value/) { get; set; } | Obtient ou définit la valeur de la cellule. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellValueDemo
    {
        public static void CellValueExample()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez une instance de CellValue
            CellValue cellValue = new CellValue();

            // Définissez le type et la valeur de la cellule
            cellValue.Type = CellValueType.IsNumeric;
            cellValue.Value = 123.45;

            // Attribuer le CellValue à une cellule de la feuille de calcul
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue(cellValue.Value);

            // Enregistrez le classeur
            workbook.Save("CellValueExample.xlsx");
            workbook.Save("CellValueExample.pdf");
            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


