---
title: "Cells.OdsCellFields"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cells. Obtient la liste des champs de ods"
type: docs
url: /fr/net/aspose.cells/cells/odscellfields/
---
## Cells.OdsCellFields property

Obtient la liste des champs d'ods.

```csharp
public OdsCellFieldCollection OdsCellFields { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsPropertyOdsCellFieldsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtenir la collection Cells
            Cells cells = worksheet.Cells;

            try
            {
                // Accéder à la propriété OdsCellFields (lecture seule)
                var odsCellFields = cells.OdsCellFields;

                // Afficher les informations sur la collection OdsCellFields
                Console.WriteLine("OdsCellFields collection count: " + odsCellFields.Count);

                // Itérer à travers la collection OdsCellFields
                for (int i = 0; i < odsCellFields.Count; i++)
                {
                    var field = odsCellFields[i];
                    Console.WriteLine($"Field {i}: Type - {field.FieldType}");
                }

                // Démontrer la mise à jour des valeurs de champ
                odsCellFields.UpdateFieldsValue();

                Console.WriteLine("OdsCellFields demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [OdsCellFieldCollection](../../../aspose.cells.ods/odscellfieldcollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


