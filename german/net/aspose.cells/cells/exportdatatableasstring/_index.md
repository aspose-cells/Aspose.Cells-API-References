---
title: "Cells.ExportDataTableAsString"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Exportiert Daten aus der Cells-Sammlung in ein DataTable-Objekt"
type: docs
url: /de/net/aspose.cells/cells/exportdatatableasstring/
---
## ExportDataTableAsString(int, int, int, int) {#exportdatatableasstring}

Exportiert Daten aus der [`Cells`](../) Sammlung in ein DataTable-Objekt.

```csharp
public DataTable ExportDataTableAsString(int firstRow, int firstColumn, int totalRows, 
    int totalColumns)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstRow | Int32 | Die Zeilennummer der ersten zu exportierenden Zelle. |
| firstColumn | Int32 | Die Spaltennummer der ersten zu exportierenden Zelle. |
| totalRows | Int32 | Anzahl der zu importierenden Zeilen. |
| totalColumns | Int32 | Anzahl der zu importierenden Spalten. |

### Rückgabewert

Exportiertes DataTable-Objekt.

### Hinweise

Alle Daten in der [`Cells`](../)-Sammlung werden in Zeichenketten konvertiert.

### Beispiele

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableAsStringWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Füge Beispieldaten zu Zellen hinzu
            cells["A1"].PutValue("Column1");
            cells["B1"].PutValue("Column2");
            cells["A2"].PutValue("Value1");
            cells["B2"].PutValue("Value2");

            // Daten als Zeichenketten in DataTable exportieren
            DataTable dataTable = cells.ExportDataTableAsString(0, 0, 2, 2);

            // Zeige die exportierten Daten an
            Console.WriteLine("Exported DataTable:");
            foreach (DataColumn column in dataTable.Columns)
            {
                Console.Write(column.ColumnName + "\t");
            }
            Console.WriteLine();
            
            foreach (DataRow row in dataTable.Rows)
            {
                foreach (var item in row.ItemArray)
                {
                    Console.Write(item.ToString() + "\t");
                }
                Console.WriteLine();
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

## ExportDataTableAsString(int, int, int, int, bool) {#exportdatatableasstring_1}

Exportiert Daten aus der [`Cells`](../) Sammlung in ein DataTable-Objekt.

```csharp
public DataTable ExportDataTableAsString(int firstRow, int firstColumn, int totalRows, 
    int totalColumns, bool exportColumnName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstRow | Int32 | Die Zeilennummer der ersten zu exportierenden Zelle. |
| firstColumn | Int32 | Die Spaltennummer der ersten zu exportierenden Zelle. |
| totalRows | Int32 | Anzahl der zu importierenden Zeilen. |
| totalColumns | Int32 | Anzahl der zu importierenden Spalten. |
| exportColumnName | Boolean | Gibt an, ob die Daten in der ersten Zeile zum Spaltennamen der DataTable exportiert werden. |

### Rückgabewert

Exportiertes DataTable-Objekt.

### Hinweise

Alle Daten in der [`Cells`](../)-Sammlung werden in Zeichenketten konvertiert.

### Beispiele

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableAsStringWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Daten in DataTable exportieren
            int maxRow = worksheet.Cells.MaxDataRow + 1;
            int maxCol = worksheet.Cells.MaxDataColumn + 1;
            DataTable dataTable = worksheet.Cells.ExportDataTableAsString(0, 0, maxRow, maxCol, true);

            // Zeige die exportierten Daten an
            foreach (DataRow row in dataTable.Rows)
            {
                foreach (DataColumn col in dataTable.Columns)
                {
                    Console.Write(row[col] + "\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


