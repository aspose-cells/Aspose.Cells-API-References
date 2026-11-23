---
title: "Enum OdsCellFieldType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.Ods.OdsCellFieldType. Représente le type de champ de cellule du ods"
type: docs
url: /fr/net/aspose.cells.ods/odscellfieldtype/
---
## OdsCellFieldType enumeration

Représente le type de champ de cellule d'ods.

```csharp
public enum OdsCellFieldType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Date | `0` | Date actuelle. |
| SheetName | `1` | Le nom de la feuille. |
| Title | `2` | Le nom du fichier. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;

    public class OdsCellFieldTypeDemo
    {
        public static void OdsCellFieldTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une OdsCellFieldCollection
            OdsCellFieldCollection odsCellFields = worksheet.Cells.OdsCellFields;

            // Ajouter un nouveau OdsCellField pour la date actuelle
            int rowIndex = 0;
            int columnIndex = 0;
            string customFormat = "yyyy-mm-dd";
            odsCellFields.Add(rowIndex, columnIndex, OdsCellFieldType.Date, customFormat);

            // Ajouter un autre OdsCellField pour le nom de la feuille
            rowIndex = 1;
            columnIndex = 0;
            odsCellFields.Add(rowIndex, columnIndex, OdsCellFieldType.SheetName, null);

            // Ajouter un autre OdsCellField pour le titre
            rowIndex = 2;
            columnIndex = 0;
            odsCellFields.Add(rowIndex, columnIndex, OdsCellFieldType.Title, null);

            // Mettre à jour la valeur des champs dans les cellules
            odsCellFields.UpdateFieldsValue();

            // Afficher les valeurs dans la console
            for (int i = 0; i < odsCellFields.Count; i++)
            {
                OdsCellField field = odsCellFields[i];
                worksheet.Cells[field.Row, field.Column].PutValue($"Field Type: {field.FieldType}, Custom Format: {field.CustomFormat}");
            }

            // Enregistrez le classeur
            workbook.Save("OdsCellFieldTypeExample.ods");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


