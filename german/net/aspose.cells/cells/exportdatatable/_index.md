---
title: "Cells.ExportDataTable"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Exportiert Daten aus der Cells-Sammlung in ein DataTable-Objekt"
type: docs
url: /de/net/aspose.cells/cells/exportdatatable/
---
## ExportDataTable(int, int, int, int) {#exportdatatable}

Exportiert Daten aus der [`Cells`](../) Sammlung in ein DataTable-Objekt.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns)
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

Wenn Sie diese Methode verwenden, um einen Datenblock zu exportieren, stellen Sie bitte sicher, dass die Daten in einer Spalte denselben Datentyp haben. Andernfalls verwenden Sie stattdessen die Methode [`ExportDataTableAsString`](../exportdatatableasstring/).

### Beispiele

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["C1"].PutValue("City");
            
            for (int i = 1; i <= 5; i++)
            {
                worksheet.Cells[i, 0].PutValue($"Person {i}");
                worksheet.Cells[i, 1].PutValue(20 + i);
                worksheet.Cells[i, 2].PutValue($"City {i}");
            }

            // Daten in DataTable exportieren (beginnend bei Zeile 0, Spalte 0, mit 5 Zeilen und 3 Spalten)
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 5, 3);

            // Zeige die exportierten Daten an
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine($"{row[0]}, {row[1]}, {row[2]}");
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

## ExportDataTable(int, int, int, int, bool) {#exportdatatable_2}

Exportiert Daten aus der [`Cells`](../) Sammlung in ein DataTable-Objekt.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool exportColumnName)
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

### Beispiele

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableWithInt32Int32Int32Int32BooleanDemo
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

            // Daten in DataTable exportieren (erste Zeile enthält Überschriften)
            DataTable dt = worksheet.Cells.ExportDataTable(0, 0, 3, 2, true);

            // Zeige die exportierten Daten an
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dt.Rows)
            {
                Console.WriteLine($"{row["Name"]}, {row["Age"]}");
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

## ExportDataTable(int, int, int, int, ExportTableOptions) {#exportdatatable_1}

Exportiert Daten aus der [`Cells`](../) Sammlung in ein DataTable-Objekt.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    ExportTableOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstRow | Int32 | Die Zeilennummer der ersten zu exportierenden Zelle. |
| firstColumn | Int32 | Die Spaltennummer der ersten zu exportierenden Zelle. |
| totalRows | Int32 | Anzahl der zu importierenden Zeilen. |
| totalColumns | Int32 | Anzahl der zu importierenden Spalten. |
| Optionen | ExportTableOptions | Alle Export-Tabellenoptionen |

### Rückgabewert

Exportiertes DataTable-Objekt.

### Beispiele

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableWithInt32Int32Int32Int32ExportTablDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Wert und Format für Zelle A1 festlegen
            cells["A1"].PutValue(1.23356);
            Style style = cells["A1"].GetStyle();
            style.Custom = "0.00";
            cells["A1"].SetStyle(style);

            // Erstelle Exportoptionen
            ExportTableOptions etOpt = new ExportTableOptions();
            etOpt.ExportColumnName = false;
            etOpt.ExportAsString = true;

            // Export mit CellStyle-Formatstrategie
            etOpt.FormatStrategy = CellValueFormatStrategy.CellStyle;
            DataTable dt1 = cells.ExportDataTable(0, 0, 1, 1, etOpt);
            Console.WriteLine("CellStyle format: " + dt1.Rows[0][0].ToString());

            // Export mit None-Formatstrategie
            etOpt.FormatStrategy = CellValueFormatStrategy.None;
            DataTable dt2 = cells.ExportDataTable(0, 0, 1, 1, etOpt);
            Console.WriteLine("None format: " + dt2.Rows[0][0].ToString());

            // Export mit DisplayStyle-Formatstrategie
            etOpt.FormatStrategy = CellValueFormatStrategy.DisplayStyle;
            DataTable dt3 = cells.ExportDataTable(0, 0, 1, 1, etOpt);
            Console.WriteLine("DisplayStyle format: " + dt3.Rows[0][0].ToString());
        }
    }
}
```

### Siehe auch

* class [ExportTableOptions](../../exporttableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


