---
title: "DataSorter.Sort"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode DataSorter. Trie les données de la zone"
type: docs
url: /fr/net/aspose.cells/datasorter/sort/
---
## Sort(Cells, int, int, int, int) {#sort_2}

Trie les données de la zone.

```csharp
public int[] Sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cellules | Cellules | Les cellules contiennent la zone de données. |
| startRow | Int32 | La ligne de départ de la zone. |
| startColumn | Int32 | La colonne de départ de la zone. |
| endRow | Int32 | La ligne de fin de la zone. |
| endColumn | Int32 | La colonne de fin de la zone. |

### Valeur de retour

les indices originaux (position absolue, par exemple, la colonne A est 0, B est 1, ...) des lignes/colonnes triées. Si aucune ligne/colonne ne doit être déplacée par cette opération de tri, null sera retourné.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodSortWithCellsInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Remplissez des données d'exemple
            for (int i = 0; i < 6; i++)
            {
                cells[i, 0].PutValue(6 - i);
            }
            
            // Masquer une ligne pour démontrer le tri avec des lignes masquées
            cells.Rows[1].IsHidden = true;
            
            // Créer et configurer le trieur
            DataSorter sorter = wb.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);
            
            // Démontrer la méthode Sort avec les paramètres Cells et Int32
            sorter.Sort(cells, 0, 0, 5, 0);
            
            // Afficher les résultats dans la console
            for (int i = 0; i < 6; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {cells[i, 0].IntValue}");
            }
            Console.WriteLine($"Is row 2 hidden? {cells.Rows[1].IsHidden}");
        }
    }
}
```

### Voir aussi

* class [Cells](../../cells/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Sort(Cells, CellArea) {#sort_1}

Trie les données de la zone.

```csharp
public int[] Sort(Cells cells, CellArea area)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cellules | Cellules | Les cellules contiennent la zone de données. |
| zone | CellArea | La zone nécessaire pour trier |

### Valeur de retour

les indices originaux (position absolue, par exemple, la colonne A est 0, B est 1, ...) des lignes/colonnes triées. Si aucune ligne/colonne ne doit être déplacée par cette opération de tri, null sera retourné.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodSortWithCellsCellAreaDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Year");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue(1995);
            worksheet.Cells["B2"].PutValue(10000);
            worksheet.Cells["A3"].PutValue(1996);
            worksheet.Cells["B3"].PutValue(15000);
            worksheet.Cells["A4"].PutValue(1997);
            worksheet.Cells["B4"].PutValue(12000);
            worksheet.Cells["A5"].PutValue(1998);
            worksheet.Cells["B5"].PutValue(18000);

            // Créer un trieur de données
            DataSorter dataSorter = workbook.DataSorter;
            dataSorter.HasHeaders = true;
            dataSorter.Key1 = 0; // Sort by first column (Year)
            dataSorter.Order1 = SortOrder.Descending;

            // Définir la zone de tri
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 4;
            area.EndColumn = 1;

            // Effectuer le tri
            dataSorter.Sort(worksheet.Cells, area);

            // Enregistrez le classeur
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../../cells/)
* struct [CellArea](../../cellarea/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Sort() {#sort}

Trie les données dans la plage.

```csharp
public int[] Sort()
```

### Valeur de retour

les indices originaux (position absolue, par exemple, la colonne A est 0, B est 1, ...) des lignes/colonnes triées. Si aucune ligne/colonne ne doit être déplacée par cette opération de tri, null sera retourné.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodSortDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple à trier
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("C");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["B3"].PutValue(10);
            worksheet.Cells["A4"].PutValue("B");
            worksheet.Cells["B4"].PutValue(20);

            // Créer un objet tableau/liste
            int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[index];
            table.ShowTotals = true;

            // Trier les données par la première colonne
            table.AutoFilter.Sorter.Sort();

            // Enregistrez le classeur
            workbook.Save("SortedData.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


