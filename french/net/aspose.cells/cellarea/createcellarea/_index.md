---
title: "CellArea.CreateCellArea"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "CellArea méthode. Crée une zone de cellule"
type: docs
url: /fr/net/aspose.cells/cellarea/createcellarea/
---
## CreateCellArea(int, int, int, int) {#createcellarea}

Crée une zone de cellules.

```csharp
public static CellArea CreateCellArea(int startRow, int startColumn, int endRow, int endColumn)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | Int32 | La ligne de départ. |
| startColumn | Int32 | La colonne de départ. |
| endRow | Int32 | La ligne de fin. |
| endColumn | Int32 | La colonne de fin. |

### Valeur de retour

Retourner un [`CellArea`](../).

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaMethodCreateCellAreaWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Remplir les cellules avec des données d'exemple
            int[] values = { 1, 3, 2, 6, 4, 5, 8, 9, 7 };
            for (int i = 0; i < values.Length; i++)
            {
                cells[i, i / 3].PutValue(values[i]);
            }

            // Créer et configurer le tri de données
            DataSorter sorter = wb.DataSorter;
            sorter.Clear();
            sorter.Order1 = SortOrder.Ascending;
            sorter.Key1 = 2;
            sorter.Order2 = SortOrder.Ascending;
            sorter.Key2 = 1;
            sorter.Order3 = SortOrder.Ascending;
            sorter.Key3 = 0;

            // Trier en utilisant CreateCellArea avec des paramètres Int32
            sorter.Sort(cells, CellArea.CreateCellArea(0, 0, 8, 2));

            // Afficher les valeurs triées
            Console.WriteLine("Sorted values:");
            for (int i = 0; i < 9; i++)
            {
                Console.WriteLine(cells[i, 2 - i / 3].IntValue);
            }
        }
    }
}
```

### Voir aussi

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateCellArea(string, string) {#createcellarea_1}

Crée une zone de cellules.

```csharp
public static CellArea CreateCellArea(string startCellName, string endCellName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startCellName | String | La cellule en haut à gauche de la plage. |
| endCellName | String | La cellule en bas à droite de la plage. |

### Valeur de retour

Retourner un [`CellArea`](../).

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaMethodCreateCellAreaWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Remplir certaines données dans la colonne A
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue($"Data {i}");
            }

            // Créer une zone de cellules de B1 à B10
            CellArea area = CellArea.CreateCellArea("B1", "B10");
            
            // Insérer une plage en décalant les cellules vers le bas
            cells.InsertRange(area, ShiftType.Down);
            
            // Vérifier l'opération en contrôlant les valeurs des cellules
            Console.WriteLine("Inserted range from B1 to B10. Total rows: " + cells.Rows.Count);
        }
    }
}
```

### Voir aussi

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


