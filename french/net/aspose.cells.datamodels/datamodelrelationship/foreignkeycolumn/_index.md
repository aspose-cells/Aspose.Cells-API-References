---
title: "DataModelRelationship.ForeignKeyColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataModelRelationship. Obtient le nom de la colonne de la table de clé étrangère pour cette relation"
type: docs
url: /fr/net/aspose.cells.datamodels/datamodelrelationship/foreignkeycolumn/
---
## DataModelRelationship.ForeignKeyColumn property

Obtient le nom de la colonne de la table de clé étrangère pour cette relation.

```csharp
public string ForeignKeyColumn { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelRelationshipPropertyForeignKeyColumnDemo
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
                    // Afficher la valeur de la propriété ForeignKeyColumn (lecture seule)
                    Console.WriteLine("Foreign Key Column: " + relationship.ForeignKeyColumn);
                }
                else
                {
                    Console.WriteLine("No relationships found in the data model.");
                }

                // Enregistrez le classeur
                workbook.Save("ForeignKeyColumnDemo.xlsx");
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


