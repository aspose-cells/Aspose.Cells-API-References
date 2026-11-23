---
title: "Énumération PasteOperationType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.PasteOperationType. Représente le type d'opération lors du collage d'une plage"
type: docs
url: /fr/net/aspose.cells/pasteoperationtype/
---
## PasteOperationType enumeration

Représente le type d'opération lors du collage d'une plage.

```csharp
public enum PasteOperationType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Aucune opération. |
| Add | `1` | Ajouter |
| Subtract | `2` | Soustraire |
| Multiply | `3` | Multiplier |
| Divide | `4` | Diviser |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassPasteOperationTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple aux cellules
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["B1"].PutValue(20);
            sheet.Cells["C1"].PutValue(30);
            
            // Créez des options de collage avec PasteOperationType.None
            var pasteOptions = new PasteOptions()
            {
                PasteType = PasteType.Values,
                OperationType = PasteOperationType.None,
                SkipBlanks = false,
                Transpose = false
            };

            // Créez une plage et copiez avec les options de collage
            Aspose.Cells.Range sourceRange = sheet.Cells.CreateRange("A1", "C1");
            Aspose.Cells.Range destRange = sheet.Cells.CreateRange("A2", "C2");
            sourceRange.Copy(destRange, pasteOptions);

            // Enregistrez le classeur
            workbook.Save("PasteOperationTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


