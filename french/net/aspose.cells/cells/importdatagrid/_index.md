---
title: "Cells.ImportDataGrid"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Importe un DataGrid dans une feuille de calcul"
type: docs
url: /fr/net/aspose.cells/cells/importdatagrid/
---
## ImportDataGrid(DataGrid, int, int, bool) {#importdatagrid}

Importe un DataGrid dans une feuille de calcul.

```csharp
public int ImportDataGrid(DataGrid dataGrid, int firstRow, int firstColumn, bool insertRows)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| dataGrid | DataGrid | L'objet DataGrid à importer. |
| firstRow | Int32 | Le numéro de ligne de la première cellule où importer. |
| firstColumn | Int32 | Le numéro de colonne de la première cellule où importer. |
| insertRows | Boolean | Indique si des lignes supplémentaires sont ajoutées pour ajuster les données. |

### Valeur de retour

Nombre total de lignes importées

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;
    using System.Data;

    public class CellsMethodImportDataGridWithDataGridInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un DataTable pour simuler les données du DataGrid
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("Name");
            dataTable.Columns.Add("Age");
            dataTable.Rows.Add("John", 30);
            dataTable.Rows.Add("Jane", 25);

            try
            {
                // Importer les données en utilisant ImportDataView qui est disponible dans l'API
                worksheet.Cells.ImportDataView(dataTable.DefaultView, 0, 0);

                Console.WriteLine("Data imported successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing data: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("ImportDataGridDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportDataGrid(DataGrid, int, int, int, int, bool) {#importdatagrid_1}

Importe un DataGrid dans une feuille de calcul.

```csharp
public int ImportDataGrid(DataGrid dataGrid, int firstRow, int firstColumn, int totalRows, 
    int totalColumns, bool insertRows)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| dataGrid | DataGrid | L'objet DataGrid à importer. |
| firstRow | Int32 | Le numéro de ligne de la première cellule où importer. |
| firstColumn | Int32 | Le numéro de colonne de la première cellule où importer. |
| totalRows | Int32 | Nombre de lignes à importer. |
| totalColumns | Int32 | Nombre de colonnes à importer. |
| insertRows | Boolean | Indique si des lignes supplémentaires sont ajoutées pour ajuster les données. |

### Valeur de retour

Nombre total de lignes importées

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataGridWithDataGridInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            try
            {
                // Créer un exemple de DataGrid avec quelques données
                // Utiliser un tableau de chaînes simple pour simuler les données du DataGrid
                string[,] gridData = new string[,]
                {
                    { "Name", "Age", "City" },
                    { "John", "30", "New York" },
                    { "Jane", "25", "Chicago" },
                    { "Bob", "35", "Los Angeles" }
                };

                // Importer les données dans la feuille de calcul en commençant à la ligne 0, colonne 0
                cells.ImportArray(gridData, 0, 0);

                // Enregistrez le classeur
                workbook.Save("ImportDataGridDemo.xlsx");
                Console.WriteLine("Data imported successfully to ImportDataGridDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing data: {ex.Message}");
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

## ImportDataGrid(DataGrid, int, int, int, int, bool, bool) {#importdatagrid_2}

Importe un DataGrid dans une feuille de calcul.

```csharp
public int ImportDataGrid(DataGrid dataGrid, int firstRow, int firstColumn, int totalRows, 
    int totalColumns, bool insertRows, bool importStyle)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| dataGrid | DataGrid | L'objet DataGrid à importer. |
| firstRow | Int32 | Le numéro de ligne de la première cellule où importer. |
| firstColumn | Int32 | Le numéro de colonne de la première cellule où importer. |
| totalRows | Int32 | Nombre de lignes à importer. |
| totalColumns | Int32 | Nombre de colonnes à importer. |
| insertRows | Boolean | Indique si des lignes supplémentaires sont ajoutées pour ajuster les données. |
| importStyle | Boolean | Indique si le style de cellule est importé. |

### Valeur de retour

Nombre total de lignes importées

### Exemples

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataGridWithDataGridInt32Int32Int32Int32Bo257661Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des données d'exemple qui proviendraient normalement d'un DataGrid
            var sampleData = new List<object[]>
            {
                new object[] { "Name", "Age", "City" },
                new object[] { "John", 30, "New York" },
                new object[] { "Jane", 25, "Los Angeles" },
                new object[] { "Bob", 35, "Chicago" }
            };

            try
            {
                // Importer les données directement dans les cellules puisque nous ne pouvons pas utiliser le DataGrid
                for (int row = 0; row < sampleData.Count; row++)
                {
                    for (int col = 0; col < sampleData[row].Length; col++)
                    {
                        worksheet.Cells[row, col].PutValue(sampleData[row][col]);
                    }
                }

                Console.WriteLine("Data imported successfully to worksheet.");

                // Enregistrez le classeur
                workbook.Save("ImportDataGridDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing data: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


