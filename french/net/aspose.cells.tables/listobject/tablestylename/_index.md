---
title: "ListObject.TableStyleName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ListObject. Obtient et définit le nom du style du tableau"
type: docs
url: /fr/net/aspose.cells.tables/listobject/tablestylename/
---
## ListObject.TableStyleName property

Obtient et définit le nom du style du tableau.

```csharp
public string TableStyleName { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyTableStyleNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Créer un objet liste/tableau
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];

            // Définir et afficher le style du tableau
            table.TableStyleName = "TableStyleLight15";
            Console.WriteLine("Table style name: " + table.TableStyleName);

            // Enregistrez le classeur
            workbook.Save("TableStyleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


