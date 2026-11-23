---
title: "ListObject.AutoFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ListObject. Obtient le filtre automatique de ce tableau"
type: docs
url: /fr/net/aspose.cells.tables/listobject/autofilter/
---
## ListObject.AutoFilter property

Obtient le filtre automatique de ce tableau.

```csharp
public AutoFilter AutoFilter { get; }
```

### Remarques

Cela fonctionne uniquement lorsque [`HasAutoFilter`](../hasautofilter/) est faux.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyAutoFilterDemo
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
            worksheet.Cells["A3"].PutValue("Mary");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Peter");
            worksheet.Cells["B4"].PutValue(35);

            // Créer un ListObject
            int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject listObject = worksheet.ListObjects[index];

            // Redimensionner l'objet de liste pour inclure toutes les données
            listObject.Resize(0, 0, 4, 2, true);

            // Accéder et démontrer la fonctionnalité AutoFilter
            if (listObject.AutoFilter != null)
            {
                // Appliquer le filtre sur la colonne Âge (colonne 2)
                listObject.AutoFilter.Filter(1, "25");
                
                // Afficher les données filtrées
                Console.WriteLine("Filtered Data:");
                for (int row = 1; row <= 4; row++)
                {
                    if (!worksheet.Cells.Rows[row].IsHidden)
                    {
                        Console.WriteLine($"{worksheet.Cells[row, 0].StringValue} - {worksheet.Cells[row, 1].IntValue}");
                    }
                }

                // Effacer le filtre
                listObject.AutoFilter.RemoveFilter(1);
            }

            // Enregistrez le classeur
            workbook.Save("ListObjectAutoFilterDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [AutoFilter](../../../aspose.cells/autofilter/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


