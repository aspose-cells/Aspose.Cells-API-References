---
title: "Cells.ImportData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Importiert Daten aus einem IDataReader-Objekt"
type: docs
url: /de/net/aspose.cells/cells/importdata/
---
## ImportData(IDataReader, int, int) {#importdata_3}

Importiert Daten aus einem IDataReader-Objekt.

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Leser | IDataReader | Das IDataReader-Objekt, das Daten enthält. |
| firstRow | Int32 | Die Zeilennummer der ersten Zelle, in die importiert werden soll. |
| firstColumn | Int32 | Die Spaltennummer der ersten Zelle, in die importiert werden soll. |

### Rückgabewert

Gesamtzahl der importierten Zeilen.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class CellsMethodImportDataWithIDataReaderInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieltabelle erstellen
            DataTable dataTable = new DataTable("Employees");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Department", typeof(string));
            
            dataTable.Rows.Add(1, "John Doe", "Engineering");
            dataTable.Rows.Add(2, "Jane Smith", "Marketing");
            dataTable.Rows.Add(3, "Mike Johnson", "Sales");

            try
            {
                // IDataReader aus DataTable erstellen
                using (IDataReader dataReader = dataTable.CreateDataReader())
                {
                    // Rufen Sie die ImportData-Methode auf, beginnend bei Zelle A1 (Zeile 0, Spalte 0)
                    int importedRows = worksheet.Cells.ImportData(dataReader, 0, 0);
                    
                    Console.WriteLine($"Imported {importedRows} rows successfully.");
                    Console.WriteLine($"Data starts at: A1 (Row 0, Column 0)");
                }

                // Spalten automatisch anpassen für bessere Sichtbarkeit
                worksheet.AutoFitColumns();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportData method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("ImportDataWithIDataReader.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(IDataReader, int, int, ImportTableOptions) {#importdata_4}

Importiert Daten aus einem IDataReader-Objekt.

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Leser | IDataReader | Das IDataReader-Objekt, das Daten enthält. |
| firstRow | Int32 | Die Zeilennummer der ersten Zelle, in die importiert werden soll. |
| firstColumn | Int32 | Die Spaltennummer der ersten Zelle, in die importiert werden soll. |
| Optionen | ImportTableOptions | Die Optionen für das Importieren der Tabelle. |

### Rückgabewert

Gesamtzahl der importierten Zeilen.

### Beispiele

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataWithIDataReaderInt32Int32ImportTabDemo
    {
        public static void Run()
        {
            // Erstelle ein Beispiel-DataTable
            DataTable dt = new DataTable("TestData");
            dt.Columns.Add("Column1", typeof(string));
            dt.Columns.Add("Column2", typeof(int));
            dt.Columns.Add("Column3", typeof(DateTime));
            
            // Fügen Sie Beispieldaten hinzu
            dt.Rows.Add("Data1", 100, DateTime.Now);
            dt.Rows.Add("Data2", 200, DateTime.Now.AddDays(1));
            dt.Rows.Add("Data3", 300, DateTime.Now.AddDays(2));

            // DataTableReader erstellen
            DataTableReader reader = dt.CreateDataReader();

            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Importoptionen festlegen
            ImportTableOptions options = new ImportTableOptions();
            options.IsFieldNameShown = true;
            options.InsertRows = true;
            options.ConvertNumericData = true;
            options.DateFormat = "MM/dd/yyyy";

            // Daten importieren, beginnend bei Zeile 5, Spalte 0
            int rowsImported = worksheet.Cells.ImportData(reader, 5, 0, options);

            // Speichere die Arbeitsmappe
            workbook.Save("ImportDataOutput.xlsx");
        }
    }
}
```

### Siehe auch

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(ICellsDataTable, int, int, ImportTableOptions) {#importdata}

Importiert Daten aus einer benutzerdefinierten Datentabelle.

```csharp
public int ImportData(ICellsDataTable table, int firstRow, int firstColumn, 
    ImportTableOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Tabelle | ICellsDataTable | Die benutzerdefinierte Datentabelle. |
| firstRow | Int32 | Index der ersten Zeile. |
| firstColumn | Int32 | Erster Spaltenindex. |
| Optionen | ImportTableOptions | Die Importoptionen |

### Beispiele

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataWithICellsDataTableInt32Int32ImporDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            
            ArrayList dataLists = new ArrayList();
            dataLists.Add(new object[] { "Name", "Age", "Gender" });
            dataLists.Add(new object[] { "Alice", 30, "Female" });
            dataLists.Add(new object[] { "Bob", 25, "Male" });
            dataLists.Add(new object[] { "Charlie", 35, "Male" });

            ICellsDataTable dt = wb.CellsDataTableFactory.GetInstance(dataLists, true);
            
            wb.Worksheets[0].Cells.ImportData(dt, 0, 0, new ImportTableOptions());
            
            Console.WriteLine("Data imported to first worksheet:");
            Console.WriteLine(wb.Worksheets[0].Cells["A2"].StringValue);
            
            wb.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* interface [ICellsDataTable](../../icellsdatatable/)
* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(DataTable, int, int, ImportTableOptions) {#importdata_1}

Importiert Daten aus einer benutzerdefinierten Datentabelle.

```csharp
public int ImportData(DataTable table, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Tabelle | DataTable | Das zu importierende DataTable-Objekt. |
| firstRow | Int32 | Index der ersten Zeile. |
| firstColumn | Int32 | Erster Spaltenindex. |
| Optionen | ImportTableOptions | Die Importoptionen |

### Rückgabewert

Gesamtzahl der importierten Zeilen.

### Beispiele

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataWithDataTableInt32Int32ImportTableDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Beispiel-DataTable erstellen.
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("Product_ID", typeof(int));
            dataTable.Columns.Add("Product_Name", typeof(string));
            dataTable.Columns.Add("Units_In_Stock", typeof(int));

            // Fügen Sie Beispieldaten hinzu
            DataRow row = dataTable.NewRow();
            row[0] = 1;
            row[1] = "Aniseed Syrup";
            row[2] = 15;
            dataTable.Rows.Add(row);

            row = dataTable.NewRow();
            row[0] = 2;
            row[1] = "Boston Crab Meat";
            row[2] = 123;
            dataTable.Rows.Add(row);

            // Importoptionen festlegen
            ImportTableOptions importOptions = new ImportTableOptions();
            importOptions.IsFieldNameShown = true;

            // Daten importieren, beginnend bei Zeile 5, Spalte 5
            cells.ImportData(dataTable, 5, 5, importOptions);

            // Speichere die Arbeitsmappe
            workbook.Save("ImportDataDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(DataView, int, int, ImportTableOptions) {#importdata_2}

Importiert Daten aus einer Datenansicht.

```csharp
public int ImportData(DataView dataView, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dataView | DataView | Das zu importierende DataView-Objekt. |
| firstRow | Int32 | Index der ersten Zeile. |
| firstColumn | Int32 | Erster Spaltenindex. |
| Optionen | ImportTableOptions | Die Importoptionen |

### Rückgabewert

Gesamtzahl der importierten Zeilen.

### Beispiele

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataWithDataViewInt32Int32ImportTableODemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Beispieltabelle erstellen
            DataTable dataTable = new DataTable("TestTable");
            dataTable.Columns.Add("Column1", typeof(string));
            dataTable.Columns.Add("Column2", typeof(int));
            
            // Fügen Sie Beispieldaten hinzu
            dataTable.Rows.Add("Data1", 100);
            dataTable.Rows.Add("Data2", 200);
            dataTable.Rows.Add("Data3", 300);

            // Erstelle ImportTableOptions
            ImportTableOptions options = new ImportTableOptions();
            options.IsFieldNameShown = true;
            options.InsertRows = true;

            // Daten aus DataView in Zellen importieren, beginnend bei Zeile 0, Spalte 0
            cells.ImportData(dataTable.DefaultView, 0, 0, options);

            // Speichere die Arbeitsmappe
            workbook.Save("ImportDataOutput.xlsx");
        }
    }
}
```

### Siehe auch

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


