---
title: "ListObject.DataSourceType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ListObject. Obtient le type de source de données du tableau"
type: docs
url: /fr/net/aspose.cells.tables/listobject/datasourcetype/
---
## ListObject.DataSourceType property

Obtient le type de source de données du tableau.

```csharp
public TableDataSourceType DataSourceType { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyDataSourceTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue("Bob");

            // Créer un objet de liste et le récupérer de la collection
            int listObjectIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];
            listObject.DisplayName = "EmployeeTable";

            // Obtenir et afficher DataSourceType
            TableDataSourceType dataSourceType = listObject.DataSourceType;
            Console.WriteLine("ListObject DataSourceType: " + dataSourceType);

            workbook.Save("ListObjectDataSourceTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [TableDataSourceType](../../tabledatasourcetype/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


