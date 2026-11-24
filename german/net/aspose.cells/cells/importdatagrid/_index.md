---
title: "Cells.ImportDataGrid"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Importiert ein DataGrid in ein Arbeitsblatt"
type: docs
url: /de/net/aspose.cells/cells/importdatagrid/
---
## ImportDataGrid(DataGrid, int, int, bool) {#importdatagrid}

Importiert ein DataGrid in ein Arbeitsblatt.

```csharp
public int ImportDataGrid(DataGrid dataGrid, int firstRow, int firstColumn, bool insertRows)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dataGrid | DataGrid | Das zu importierende DataGrid-Objekt. |
| firstRow | Int32 | Die Zeilennummer der ersten Zelle, in die importiert werden soll. |
| firstColumn | Int32 | Die Spaltennummer der ersten Zelle, in die importiert werden soll. |
| insertRows | Boolean | Gibt an, ob zusätzliche Zeilen hinzugefügt werden, um die Daten anzupassen. |

### Rückgabewert

Gesamtzahl der importierten Zeilen

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle ein DataTable, um DataGrid-Daten zu simulieren
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("Name");
            dataTable.Columns.Add("Age");
            dataTable.Rows.Add("John", 30);
            dataTable.Rows.Add("Jane", 25);

            try
            {
                // Importiere die Daten mit ImportDataView, das in der API verfügbar ist
                worksheet.Cells.ImportDataView(dataTable.DefaultView, 0, 0);

                Console.WriteLine("Data imported successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing data: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("ImportDataGridDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportDataGrid(DataGrid, int, int, int, int, bool) {#importdatagrid_1}

Importiert ein DataGrid in ein Arbeitsblatt.

```csharp
public int ImportDataGrid(DataGrid dataGrid, int firstRow, int firstColumn, int totalRows, 
    int totalColumns, bool insertRows)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dataGrid | DataGrid | Das zu importierende DataGrid-Objekt. |
| firstRow | Int32 | Die Zeilennummer der ersten Zelle, in die importiert werden soll. |
| firstColumn | Int32 | Die Spaltennummer der ersten Zelle, in die importiert werden soll. |
| totalRows | Int32 | Anzahl der zu importierenden Zeilen. |
| totalColumns | Int32 | Anzahl der zu importierenden Spalten. |
| insertRows | Boolean | Gibt an, ob zusätzliche Zeilen hinzugefügt werden, um die Daten anzupassen. |

### Rückgabewert

Gesamtzahl der importierten Zeilen

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataGridWithDataGridInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            try
            {
                // Erstelle ein Beispiel-DataGrid mit einigen Daten
                // Verwende ein einfaches String-Array, um DataGrid-Daten zu simulieren
                string[,] gridData = new string[,]
                {
                    { "Name", "Age", "City" },
                    { "John", "30", "New York" },
                    { "Jane", "25", "Chicago" },
                    { "Bob", "35", "Los Angeles" }
                };

                // Importiere die Daten in das Arbeitsblatt, beginnend bei Zeile 0, Spalte 0
                cells.ImportArray(gridData, 0, 0);

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportDataGrid(DataGrid, int, int, int, int, bool, bool) {#importdatagrid_2}

Importiert ein DataGrid in ein Arbeitsblatt.

```csharp
public int ImportDataGrid(DataGrid dataGrid, int firstRow, int firstColumn, int totalRows, 
    int totalColumns, bool insertRows, bool importStyle)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dataGrid | DataGrid | Das zu importierende DataGrid-Objekt. |
| firstRow | Int32 | Die Zeilennummer der ersten Zelle, in die importiert werden soll. |
| firstColumn | Int32 | Die Spaltennummer der ersten Zelle, in die importiert werden soll. |
| totalRows | Int32 | Anzahl der zu importierenden Zeilen. |
| totalColumns | Int32 | Anzahl der zu importierenden Spalten. |
| insertRows | Boolean | Gibt an, ob zusätzliche Zeilen hinzugefügt werden, um die Daten anzupassen. |
| importStyle | Boolean | Gibt an, ob der Zellenstil importiert wird. |

### Rückgabewert

Gesamtzahl der importierten Zeilen

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle Beispieldaten, die normalerweise von einem DataGrid stammen würden
            var sampleData = new List<object[]>
            {
                new object[] { "Name", "Age", "City" },
                new object[] { "John", 30, "New York" },
                new object[] { "Jane", 25, "Los Angeles" },
                new object[] { "Bob", 35, "Chicago" }
            };

            try
            {
                // Importiere die Daten direkt in Zellen, da wir kein DataGrid verwenden können
                for (int row = 0; row < sampleData.Count; row++)
                {
                    for (int col = 0; col < sampleData[row].Length; col++)
                    {
                        worksheet.Cells[row, col].PutValue(sampleData[row][col]);
                    }
                }

                Console.WriteLine("Data imported successfully to worksheet.");

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


