---
title: "DataModelTable.ConnectionName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataModelTable. Obtient le nom de connexion de la table du modèle de données."
type: docs
url: /fr/net/aspose.cells.datamodels/datamodeltable/connectionname/
---
## DataModelTable.ConnectionName property

Obtient le nom de connexion de la table du modèle de données.

```csharp
public string ConnectionName { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using Aspose.Cells.Tables;
    using Aspose.Cells.Pivot;
    using System;

    public class DataModelTablePropertyConnectionNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple pour créer une table
            worksheet.Cells["A1"].PutValue("OrderID");
            worksheet.Cells["B1"].PutValue("Customer");
            worksheet.Cells["A2"].PutValue(1001);
            worksheet.Cells["B2"].PutValue("John Doe");
            worksheet.Cells["A3"].PutValue(1002);
            worksheet.Cells["B3"].PutValue("Jane Smith");

            // Créez un ListObject (table)
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "OrdersTable";

            // Accédez à la DataModelTable
            DataModelTable dataModelTable = workbook.DataModel.Tables[0];

            // Afficher la valeur actuelle de ConnectionName.
            Console.WriteLine("Current ConnectionName: " + dataModelTable.ConnectionName);

            // Créer un tableau croisé dynamique en utilisant la connexion de DataModelTable.
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotReport");
            int pivotIndex = pivotSheet.PivotTables.Add("PivotTable1", "A1", dataModelTable.Name);
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Customer");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "OrderID");

            // Remarque : ConnectionName est en lecture seule, nous ne pouvons pas le définir.
            // Cela montre comment utiliser le nom de connexion existant.
            if (!string.IsNullOrEmpty(dataModelTable.ConnectionName))
            {
                Console.WriteLine("This table is connected via: " + dataModelTable.ConnectionName);
            }

            // Enregistrez le classeur
            workbook.Save("DataModelTableConnectionNameDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [DataModelTable](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


