---
title: "DataModelRelationship.ForeignKeyTable"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataModelRelationship. Obtient le nom de la table de clé étrangère pour cette relation"
type: docs
url: /fr/net/aspose.cells.datamodels/datamodelrelationship/foreignkeytable/
---
## DataModelRelationship.ForeignKeyTable property

Obtient le nom de la table de clé étrangère pour cette relation.

```csharp
public string ForeignKeyTable { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelRelationshipPropertyForeignKeyTableDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour créer un contexte significatif
            worksheet.Cells["A1"].PutValue("Orders");
            worksheet.Cells["A2"].PutValue("OrderID");
            worksheet.Cells["A3"].PutValue("CustomerID");

            worksheet.Cells["C1"].PutValue("Customers");
            worksheet.Cells["C2"].PutValue("CustomerID");
            worksheet.Cells["C3"].PutValue("CustomerName");

            try
            {
                // Accéder à la première relation si elle existe
                DataModelRelationship relationship = workbook.DataModel?.Relationships?[0];

                if (relationship != null)
                {
                    // Afficher la valeur de la propriété ForeignKeyTable (lecture seule)
                    Console.WriteLine("Foreign Key Table: " + relationship.ForeignKeyTable);
                }
                else
                {
                    Console.WriteLine("No relationships found in the data model.");
                }

                // Enregistrez le classeur
                workbook.Save("ForeignKeyTableDemo.xlsx");
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

* class [DataModelRelationship](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


