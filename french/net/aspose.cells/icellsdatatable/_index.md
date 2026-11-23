---
title: "Interface ICellsDataTable"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Interface Aspose.Cells.ICellsDataTable. Représente une table de données"
type: docs
url: /fr/net/aspose.cells/icellsdatatable/
---
## ICellsDataTable interface

Représente le tableau de données.

```csharp
public interface ICellsDataTable
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Columns](../../aspose.cells/icellsdatatable/columns/) { get; } | Obtient le nom des colonnes. |
| [Count](../../aspose.cells/icellsdatatable/count/) { get; } | Obtient le nombre d'enregistrements. -1 pour un nombre d'enregistrements inconnu. |
| [Item](../../aspose.cells/icellsdatatable/item/) { get; } | Obtient les données stockées dans la colonne spécifiée par l'index. (2 indexeurs) |

## Méthodes

| Nom | Description |
| --- | --- |
| [BeforeFirst](../../aspose.cells/icellsdatatable/beforefirst/)() | Déplacez le curseur au début de cet objet, juste avant la première ligne. |
| [Next](../../aspose.cells/icellsdatatable/next/)() | Déplace le curseur d'une ligne vers le bas depuis sa position actuelle. |

### Exemples

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassICellsDataTableDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();

            ArrayList dataLists = new ArrayList();
            ArrayList list1 = new ArrayList();
            list1.AddRange(new object[] { "Name", "Age", "Gender" });
            ArrayList list2 = new ArrayList();
            list2.AddRange(new object[] { "Alice", 30, "Female" });
            ArrayList list3 = new ArrayList();
            list3.AddRange(new object[] { "Bob", 25, "Male" });
            ArrayList list4 = new ArrayList();
            list4.AddRange(new object[] { "Charlie", 35, "Male" });
            dataLists.Add(list1);
            dataLists.Add(list2);
            dataLists.Add(list3);
            dataLists.Add(list4);

            ICellsDataTable dt = wb.CellsDataTableFactory.GetInstance(dataLists, true);
            
            wb.Worksheets[0].Cells.ImportData(dt, 0, 0, new ImportTableOptions());
            Console.WriteLine("First worksheet A2 value: " + wb.Worksheets[0].Cells["A2"].StringValue);

            wb.Worksheets.Add();
            wb.Worksheets[1].Cells.ImportArrayList(dataLists, 0, 0, true);
            Console.WriteLine("Second worksheet A3 value: " + wb.Worksheets[1].Cells["A3"].StringValue);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


