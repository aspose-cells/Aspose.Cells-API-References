---
title: "Énumération CopyFormatType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.CopyFormatType enum. Représente le type de format de copie lors de l'insertion de lignes"
type: docs
url: /fr/net/aspose.cells/copyformattype/
---
## CopyFormatType enumeration

Représente le type de format de copie lors de l'insertion de lignes.

```csharp
public enum CopyFormatType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| SameAsAbove | `0` | Formats identiques à la ligne ci‑dessus. |
| SameAsBelow | `1` | Formats identiques à la ligne ci‑dessous. |
| Clear | `2` | Efface le formatage. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CopyFormatTypeDemo
    {
        public static void CopyFormatTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplissez quelques données dans la feuille de calcul
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");

            // Créez InsertOptions et définissez CopyFormatType
            InsertOptions insertOptions = new InsertOptions();
            insertOptions.CopyFormatType = CopyFormatType.SameAsAbove;

            // Insérez une ligne à la deuxième position avec le type de format spécifié
            worksheet.Cells.InsertRows(1, 1, insertOptions);

            // Enregistrez le classeur
            workbook.Save("CopyFormatTypeExample.xlsx");
            workbook.Save("CopyFormatTypeExample.pdf");
            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


