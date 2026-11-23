---
title: "ListObject.DataRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ListObject. Obtient la plage de données du tableau"
type: docs
url: /fr/net/aspose.cells.tables/listobject/datarange/
---
## ListObject.DataRange property

Obtient la plage de données du tableau.

```csharp
public Range DataRange { get; }
```

### Exemples

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyDataRangeDemo
    {
        public static void Run()
        {
            Encoding.RegisterProvider(CodePagesEncodingProvider.Instance);
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            // Créer un ListObject (Table)
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "EmployeeTable";

            // Obtenir la plage de données du tableau
            Aspose.Cells.Range dataRange = table.DataRange;

            // Démontrer l'utilisation de DataRange
            Console.WriteLine("Table Data Range: " + dataRange.Address);
            Console.WriteLine("Row Count: " + dataRange.RowCount);
            Console.WriteLine("Column Count: " + dataRange.ColumnCount);

            // Ajouter une formule à la dernière colonne en utilisant DataRange
            string formula = "=CONCATENATE(\"ID-\", [ID])";
            int lastColIndex = dataRange.ColumnCount - 1;
            dataRange[0, lastColIndex].PutValue("FormattedID");
            for (int i = 1; i < dataRange.RowCount; i++)
            {
                dataRange[i, lastColIndex].Formula = formula;
            }

            // Enregistrez le classeur
            workbook.Save("ListObjectDataRangeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Range](../../../aspose.cells/range/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


