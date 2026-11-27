---
title: "Cells.ImportData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metoden. Importerar data från ett IDataReader-objekt"
type: docs
url: /sv/net/aspose.cells/cells/importdata/
---
## ImportData(IDataReader, int, int) {#importdata_3}

Importerar data från ett IDataReader-objekt.

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| läsare | IDataReader | IDataReader-objektet som innehåller data. |
| firstRow | Int32 | Radnumret för den första cellen att importera i. |
| firstColumn | Int32 | Kolumnnumret för den första cellen att importera i. |

### Returvärde

Totalt antal importerade rader.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldatatabell
            DataTable dataTable = new DataTable("Employees");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Department", typeof(string));
            
            dataTable.Rows.Add(1, "John Doe", "Engineering");
            dataTable.Rows.Add(2, "Jane Smith", "Marketing");
            dataTable.Rows.Add(3, "Mike Johnson", "Sales");

            try
            {
                // Skapa IDataReader från DataTable
                using (IDataReader dataReader = dataTable.CreateDataReader())
                {
                    // Anropa ImportData-metoden med start i cell A1 (rad 0, kolumn 0)
                    int importedRows = worksheet.Cells.ImportData(dataReader, 0, 0);
                    
                    Console.WriteLine($"Imported {importedRows} rows successfully.");
                    Console.WriteLine($"Data starts at: A1 (Row 0, Column 0)");
                }

                // Autoanpassa kolumner för bättre synlighet
                worksheet.AutoFitColumns();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportData method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("ImportDataWithIDataReader.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(IDataReader, int, int, ImportTableOptions) {#importdata_4}

Importerar data från ett IDataReader-objekt.

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| läsare | IDataReader | IDataReader-objektet som innehåller data. |
| firstRow | Int32 | Radnumret för den första cellen att importera i. |
| firstColumn | Int32 | Kolumnnumret för den första cellen att importera i. |
| alternativ | ImportTableOptions | Alternativen för att importera tabellen. |

### Returvärde

Totalt antal importerade rader.

### Exempel

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
            // Skapa en exempel-DataTable
            DataTable dt = new DataTable("TestData");
            dt.Columns.Add("Column1", typeof(string));
            dt.Columns.Add("Column2", typeof(int));
            dt.Columns.Add("Column3", typeof(DateTime));
            
            // Lägg till exempeldata
            dt.Rows.Add("Data1", 100, DateTime.Now);
            dt.Rows.Add("Data2", 200, DateTime.Now.AddDays(1));
            dt.Rows.Add("Data3", 300, DateTime.Now.AddDays(2));

            // Skapa DataTableReader
            DataTableReader reader = dt.CreateDataReader();

            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ställ in importalternativ
            ImportTableOptions options = new ImportTableOptions();
            options.IsFieldNameShown = true;
            options.InsertRows = true;
            options.ConvertNumericData = true;
            options.DateFormat = "MM/dd/yyyy";

            // Importera data med start i rad 5, kolumn 0
            int rowsImported = worksheet.Cells.ImportData(reader, 5, 0, options);

            // Spara arbetsboken
            workbook.Save("ImportDataOutput.xlsx");
        }
    }
}
```

### Se även

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(ICellsDataTable, int, int, ImportTableOptions) {#importdata}

Importera data från en anpassad datatabell.

```csharp
public int ImportData(ICellsDataTable table, int firstRow, int firstColumn, 
    ImportTableOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| tabell | ICellsDataTable | Den anpassade datatabellen. |
| firstRow | Int32 | Första radens index. |
| firstColumn | Int32 | Första kolumnens index. |
| alternativ | ImportTableOptions | Importalternativen |

### Exempel

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

### Se även

* interface [ICellsDataTable](../../icellsdatatable/)
* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(DataTable, int, int, ImportTableOptions) {#importdata_1}

Importera data från en anpassad datatabell.

```csharp
public int ImportData(DataTable table, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| tabell | DataTable | DataTable-objektet som ska importeras. |
| firstRow | Int32 | Första radens index. |
| firstColumn | Int32 | Första kolumnens index. |
| alternativ | ImportTableOptions | Importalternativen |

### Returvärde

Totalt antal importerade rader.

### Exempel

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

            // Skapa exempel på DataTable
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("Product_ID", typeof(int));
            dataTable.Columns.Add("Product_Name", typeof(string));
            dataTable.Columns.Add("Units_In_Stock", typeof(int));

            // Lägg till exempeldata
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

            // Ställ in importalternativ
            ImportTableOptions importOptions = new ImportTableOptions();
            importOptions.IsFieldNameShown = true;

            // Importera data med start i rad 5, kolumn 5
            cells.ImportData(dataTable, 5, 5, importOptions);

            // Spara arbetsboken
            workbook.Save("ImportDataDemo.xlsx");
        }
    }
}
```

### Se även

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(DataView, int, int, ImportTableOptions) {#importdata_2}

Importera data från en datavy.

```csharp
public int ImportData(DataView dataView, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dataView | DataView | DataView-objektet som ska importeras. |
| firstRow | Int32 | Första radens index. |
| firstColumn | Int32 | Första kolumnens index. |
| alternativ | ImportTableOptions | Importalternativen |

### Returvärde

Totalt antal importerade rader.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Skapa exempeldatatabell
            DataTable dataTable = new DataTable("TestTable");
            dataTable.Columns.Add("Column1", typeof(string));
            dataTable.Columns.Add("Column2", typeof(int));
            
            // Lägg till exempeldata
            dataTable.Rows.Add("Data1", 100);
            dataTable.Rows.Add("Data2", 200);
            dataTable.Rows.Add("Data3", 300);

            // Skapa ImportTableOptions
            ImportTableOptions options = new ImportTableOptions();
            options.IsFieldNameShown = true;
            options.InsertRows = true;

            // Importera data från DataView till celler med start i rad 0, kolumn 0
            cells.ImportData(dataTable.DefaultView, 0, 0, options);

            // Spara arbetsboken
            workbook.Save("ImportDataOutput.xlsx");
        }
    }
}
```

### Se även

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


