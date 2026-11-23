---
title: "Classe DataModelTable"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.DataModels.DataModelTable. Représente les propriétés d'une seule table dans le modèle de données de la feuille de calcul"
type: docs
url: /fr/net/aspose.cells.datamodels/datamodeltable/
---
## DataModelTable class

Représente les propriétés d'une seule table dans le modèle de données de la feuille de calcul.

```csharp
public class DataModelTable
```

## Propriétés

| Nom | Description |
| --- | --- |
| [ConnectionName](../../aspose.cells.datamodels/datamodeltable/connectionname/) { get; } | Obtient le nom de connexion de la table du modèle de données. |
| [Id](../../aspose.cells.datamodels/datamodeltable/id/) { get; } | Obtient l'ID de la table du modèle de données. |
| [Name](../../aspose.cells.datamodels/datamodeltable/name/) { get; } | Obtient le nom de la table du modèle de données. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using Aspose.Cells.Tables;
    using Aspose.Cells.Pivot;
    using System;

    public class DataModelsClassDataModelTableDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple pour créer une table
            worksheet.Cells["A1"].PutValue("ProductID");
            worksheet.Cells["B1"].PutValue("ProductName");
            worksheet.Cells["A2"].PutValue(101);
            worksheet.Cells["B2"].PutValue("Laptop");
            worksheet.Cells["A3"].PutValue(102);
            worksheet.Cells["B3"].PutValue("Monitor");

            // Créez un ListObject (table)
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "ProductsTable";

            // Accédez à la DataModelTable
            DataModelTable dataModelTable = workbook.DataModel.Tables[0];

            // Afficher les propriétés de la DataModelTable
            Console.WriteLine("Data Model Table Properties:");
            Console.WriteLine($"ID: {dataModelTable.Id}");
            Console.WriteLine($"Name: {dataModelTable.Name}");
            Console.WriteLine($"Connection Name: {dataModelTable.ConnectionName}");

            // Créez un tableau croisé dynamique en utilisant la DataModelTable
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");
            int pivotIndex = pivotSheet.PivotTables.Add("PivotTable1", "A1", dataModelTable.Name);
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "ProductName");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "ProductID");

            // Enregistrez le classeur
            workbook.Save("DataModelTableDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)


