---
title: "Cells.DeleteRows"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Supprime plusieurs lignes"
type: docs
url: /fr/net/aspose.cells/cells/deleterows/
---
## DeleteRows(int, int) {#deleterows}

Supprime plusieurs lignes.

```csharp
public bool DeleteRows(int rowIndex, int totalRows)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | L'index de la première ligne à supprimer. |
| totalRows | Int32 | Nombre de lignes à supprimer. |

### Remarques

Si la plage supprimée contient la partie supérieure (pas la totalité) du tableau (ListObject), la plage ne peut pas être supprimée et aucune action ne sera effectuée. Cela fonctionne de la même manière avec MS Excel.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Remplir des données d'exemple
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    cells[i, j].PutValue($"Row {i+1}, Col {j+1}");
                }
            }

            Console.WriteLine("Before deleting rows:");
            PrintCellValues(cells, 0, 9, 0, 4);

            // Supprimer 2 lignes à partir de l'index de ligne 2 (3e ligne)
            cells.DeleteRows(2, 2);

            Console.WriteLine("\nAfter deleting rows 3-4:");
            PrintCellValues(cells, 0, 7, 0, 4);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }

        private static void PrintCellValues(Cells cells, int startRow, int endRow, int startCol, int endCol)
        {
            for (int i = startRow; i <= endRow; i++)
            {
                for (int j = startCol; j <= endCol; j++)
                {
                    Console.Write($"{cells[i, j].StringValue}\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteRows(int, int, bool) {#deleterows_2}

Supprime plusieurs lignes dans la feuille de calcul.

```csharp
public bool DeleteRows(int rowIndex, int totalRows, bool updateReference)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Index de la première ligne à supprimer. |
| totalRows | Int32 | Nombre de lignes à supprimer. |
| updateReference | Boolean | Indique si les références doivent être mises à jour dans les autres feuilles de calcul. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Importer des données dans les cellules
            worksheet.Cells.ImportTwoDimensionArray(new object[2, 2] { { "A1", "B1" }, { "A2", "B2" } }, 0, 0);

            // Créer un tableau
            ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add(0, 0, 1, 1, false)];
            table.ShowHeaderRow = false;

            Console.WriteLine("Before DeleteRows:");
            Console.WriteLine($"Table Data Range Row Count: {table.ListColumns.Count}");
            Console.WriteLine($"Table Start Row: {table.StartRow}");
            Console.WriteLine($"Table End Row: {table.EndRow}");

            // Supprimer la ligne à l'index 1 (deuxième ligne) avec mise à jour de la référence
            worksheet.Cells.DeleteRows(1, 1, true);

            Console.WriteLine("\nAfter DeleteRows:");
            Console.WriteLine($"Table Data Range Row Count: {table.ListColumns.Count}");
            Console.WriteLine($"Table Start Row: {table.StartRow}");
            Console.WriteLine($"Table End Row: {table.EndRow}");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteRows(int, int, DeleteOptions) {#deleterows_1}

Supprime plusieurs lignes dans la feuille de calcul.

```csharp
public bool DeleteRows(int rowIndex, int totalRows, DeleteOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Index de la première ligne à supprimer. |
| totalRows | Int32 | Nombre de lignes à supprimer. |
| options | DeleteOptions | Options pour l'opération de suppression |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowsWithInt32Int32DeleteOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Définir des données d'exemple et des formules
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["A3"].PutValue(30);
            cells["B1"].Formula = "=SUM(A1:A3)";
            
            // Supprimer la ligne 2 sans surveillance (car FormulaChangeMonitor n'est pas disponible)
            cells.DeleteRows(1, 1, new DeleteOptions());
            
            Console.WriteLine("Deleted row 2. Formula in B1 should now be: " + cells["B1"].Formula);
        }
    }
}
```

### Voir aussi

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


