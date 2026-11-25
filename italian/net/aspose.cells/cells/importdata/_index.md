---
title: "Cells.ImportData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Importa dati da un oggetto IDataReader"
type: docs
url: /it/net/aspose.cells/cells/importdata/
---
## ImportData(IDataReader, int, int) {#importdata_3}

Importa dati da un oggetto IDataReader.

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| lettore | IDataReader | L'oggetto IDataReader che contiene i dati. |
| firstRow | Int32 | Il numero di riga della prima cella in cui importare. |
| firstColumn | Int32 | Il numero di colonna della prima cella in cui importare. |

### Valore di ritorno

Numero totale di righe importate.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una tabella di dati di esempio
            DataTable dataTable = new DataTable("Employees");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Department", typeof(string));
            
            dataTable.Rows.Add(1, "John Doe", "Engineering");
            dataTable.Rows.Add(2, "Jane Smith", "Marketing");
            dataTable.Rows.Add(3, "Mike Johnson", "Sales");

            try
            {
                // Crea IDataReader da DataTable
                using (IDataReader dataReader = dataTable.CreateDataReader())
                {
                    // Chiama il metodo ImportData iniziando dalla cella A1 (riga 0, colonna 0)
                    int importedRows = worksheet.Cells.ImportData(dataReader, 0, 0);
                    
                    Console.WriteLine($"Imported {importedRows} rows successfully.");
                    Console.WriteLine($"Data starts at: A1 (Row 0, Column 0)");
                }

                // Adatta automaticamente le colonne per una migliore visibilità
                worksheet.AutoFitColumns();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportData method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("ImportDataWithIDataReader.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(IDataReader, int, int, ImportTableOptions) {#importdata_4}

Importa dati da un oggetto IDataReader.

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| lettore | IDataReader | L'oggetto IDataReader che contiene i dati. |
| firstRow | Int32 | Il numero di riga della prima cella in cui importare. |
| firstColumn | Int32 | Il numero di colonna della prima cella in cui importare. |
| opzioni | ImportTableOptions | Le opzioni di importazione della tabella. |

### Valore di ritorno

Numero totale di righe importate.

### Esempi

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
            // Crea un DataTable di esempio
            DataTable dt = new DataTable("TestData");
            dt.Columns.Add("Column1", typeof(string));
            dt.Columns.Add("Column2", typeof(int));
            dt.Columns.Add("Column3", typeof(DateTime));
            
            // Aggiungi dati di esempio
            dt.Rows.Add("Data1", 100, DateTime.Now);
            dt.Rows.Add("Data2", 200, DateTime.Now.AddDays(1));
            dt.Rows.Add("Data3", 300, DateTime.Now.AddDays(2));

            // Crea DataTableReader
            DataTableReader reader = dt.CreateDataReader();

            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta le opzioni di importazione
            ImportTableOptions options = new ImportTableOptions();
            options.IsFieldNameShown = true;
            options.InsertRows = true;
            options.ConvertNumericData = true;
            options.DateFormat = "MM/dd/yyyy";

            // Importa dati iniziando dalla riga 5, colonna 0
            int rowsImported = worksheet.Cells.ImportData(reader, 5, 0, options);

            // Salva la cartella di lavoro
            workbook.Save("ImportDataOutput.xlsx");
        }
    }
}
```

### Vedi anche

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(ICellsDataTable, int, int, ImportTableOptions) {#importdata}

Importa dati da una tabella dati personalizzata.

```csharp
public int ImportData(ICellsDataTable table, int firstRow, int firstColumn, 
    ImportTableOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| tabella | ICellsDataTable | La tabella di dati personalizzata. |
| firstRow | Int32 | Indice della prima riga. |
| firstColumn | Int32 | Indice della prima colonna. |
| opzioni | ImportTableOptions | Le opzioni di importazione |

### Esempi

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

### Vedi anche

* interface [ICellsDataTable](../../icellsdatatable/)
* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(DataTable, int, int, ImportTableOptions) {#importdata_1}

Importa dati da una tabella dati personalizzata.

```csharp
public int ImportData(DataTable table, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| tabella | DataTable | L'oggetto DataTable da importare. |
| firstRow | Int32 | Indice della prima riga. |
| firstColumn | Int32 | Indice della prima colonna. |
| opzioni | ImportTableOptions | Le opzioni di importazione |

### Valore di ritorno

Numero totale di righe importate.

### Esempi

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

            // Crea un DataTable di esempio
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("Product_ID", typeof(int));
            dataTable.Columns.Add("Product_Name", typeof(string));
            dataTable.Columns.Add("Units_In_Stock", typeof(int));

            // Aggiungi dati di esempio
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

            // Imposta le opzioni di importazione
            ImportTableOptions importOptions = new ImportTableOptions();
            importOptions.IsFieldNameShown = true;

            // Importa i dati a partire dalla riga 5, colonna 5
            cells.ImportData(dataTable, 5, 5, importOptions);

            // Salva la cartella di lavoro
            workbook.Save("ImportDataDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(DataView, int, int, ImportTableOptions) {#importdata_2}

Importa dati da una vista dati.

```csharp
public int ImportData(DataView dataView, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dataView | DataView | L'oggetto DataView da importare. |
| firstRow | Int32 | Indice della prima riga. |
| firstColumn | Int32 | Indice della prima colonna. |
| opzioni | ImportTableOptions | Le opzioni di importazione |

### Valore di ritorno

Numero totale di righe importate.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Crea una tabella di dati di esempio
            DataTable dataTable = new DataTable("TestTable");
            dataTable.Columns.Add("Column1", typeof(string));
            dataTable.Columns.Add("Column2", typeof(int));
            
            // Aggiungi dati di esempio
            dataTable.Rows.Add("Data1", 100);
            dataTable.Rows.Add("Data2", 200);
            dataTable.Rows.Add("Data3", 300);

            // Crea ImportTableOptions
            ImportTableOptions options = new ImportTableOptions();
            options.IsFieldNameShown = true;
            options.InsertRows = true;

            // Importa i dati da DataView alle celle a partire dalla riga 0, colonna 0
            cells.ImportData(dataTable.DefaultView, 0, 0, options);

            // Salva la cartella di lavoro
            workbook.Save("ImportDataOutput.xlsx");
        }
    }
}
```

### Vedi anche

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


