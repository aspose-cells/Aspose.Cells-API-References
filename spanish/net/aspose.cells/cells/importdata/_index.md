---
title: "Cells.ImportData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Importa datos de un objeto IDataReader"
type: docs
url: /es/net/aspose.cells/cells/importdata/
---
## ImportData(IDataReader, int, int) {#importdata_3}

Importa datos de un objeto IDataReader.

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| lector | IDataReader | El objeto IDataReader que contiene datos. |
| firstRow | Int32 | El número de fila de la primera celda en la que importar. |
| firstColumn | Int32 | El número de columna de la primera celda en la que importar. |

### Valor de retorno

Número total de filas importadas.

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear tabla de datos de ejemplo
            DataTable dataTable = new DataTable("Employees");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Department", typeof(string));
            
            dataTable.Rows.Add(1, "John Doe", "Engineering");
            dataTable.Rows.Add(2, "Jane Smith", "Marketing");
            dataTable.Rows.Add(3, "Mike Johnson", "Sales");

            try
            {
                // Crear IDataReader a partir de DataTable
                using (IDataReader dataReader = dataTable.CreateDataReader())
                {
                    // Llamar al método ImportData comenzando en la celda A1 (fila 0, columna 0)
                    int importedRows = worksheet.Cells.ImportData(dataReader, 0, 0);
                    
                    Console.WriteLine($"Imported {importedRows} rows successfully.");
                    Console.WriteLine($"Data starts at: A1 (Row 0, Column 0)");
                }

                // Ajustar automáticamente las columnas para una mejor visibilidad
                worksheet.AutoFitColumns();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportData method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("ImportDataWithIDataReader.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(IDataReader, int, int, ImportTableOptions) {#importdata_4}

Importa datos de un objeto IDataReader.

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| lector | IDataReader | El objeto IDataReader que contiene datos. |
| firstRow | Int32 | El número de fila de la primera celda en la que importar. |
| firstColumn | Int32 | El número de columna de la primera celda en la que importar. |
| opciones | ImportTableOptions | Las opciones de importación de la tabla. |

### Valor de retorno

Número total de filas importadas.

### Ejemplos

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
            // Crear un DataTable de ejemplo
            DataTable dt = new DataTable("TestData");
            dt.Columns.Add("Column1", typeof(string));
            dt.Columns.Add("Column2", typeof(int));
            dt.Columns.Add("Column3", typeof(DateTime));
            
            // Agregar datos de ejemplo
            dt.Rows.Add("Data1", 100, DateTime.Now);
            dt.Rows.Add("Data2", 200, DateTime.Now.AddDays(1));
            dt.Rows.Add("Data3", 300, DateTime.Now.AddDays(2));

            // Crear DataTableReader
            DataTableReader reader = dt.CreateDataReader();

            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer opciones de importación
            ImportTableOptions options = new ImportTableOptions();
            options.IsFieldNameShown = true;
            options.InsertRows = true;
            options.ConvertNumericData = true;
            options.DateFormat = "MM/dd/yyyy";

            // Importar datos comenzando en la fila 5, columna 0
            int rowsImported = worksheet.Cells.ImportData(reader, 5, 0, options);

            // Guarda el libro de trabajo
            workbook.Save("ImportDataOutput.xlsx");
        }
    }
}
```

### Ver también

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(ICellsDataTable, int, int, ImportTableOptions) {#importdata}

Importa datos de una tabla de datos personalizada.

```csharp
public int ImportData(ICellsDataTable table, int firstRow, int firstColumn, 
    ImportTableOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tabla | ICellsDataTable | La tabla de datos personalizada. |
| firstRow | Int32 | Índice de la primera fila. |
| firstColumn | Int32 | Índice de primera columna. |
| opciones | ImportTableOptions | Las opciones de importación |

### Ejemplos

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

### Ver también

* interface [ICellsDataTable](../../icellsdatatable/)
* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(DataTable, int, int, ImportTableOptions) {#importdata_1}

Importa datos de una tabla de datos personalizada.

```csharp
public int ImportData(DataTable table, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tabla | DataTable | El objeto DataTable que se importará. |
| firstRow | Int32 | Índice de la primera fila. |
| firstColumn | Int32 | Índice de primera columna. |
| opciones | ImportTableOptions | Las opciones de importación |

### Valor de retorno

Número total de filas importadas.

### Ejemplos

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

            // Crear DataTable de ejemplo
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("Product_ID", typeof(int));
            dataTable.Columns.Add("Product_Name", typeof(string));
            dataTable.Columns.Add("Units_In_Stock", typeof(int));

            // Agregar datos de ejemplo
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

            // Establecer opciones de importación
            ImportTableOptions importOptions = new ImportTableOptions();
            importOptions.IsFieldNameShown = true;

            // Importar datos comenzando en la fila 5, columna 5
            cells.ImportData(dataTable, 5, 5, importOptions);

            // Guarda el libro de trabajo
            workbook.Save("ImportDataDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(DataView, int, int, ImportTableOptions) {#importdata_2}

Importa datos de una vista de datos.

```csharp
public int ImportData(DataView dataView, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dataView | DataView | El objeto DataView a importar. |
| firstRow | Int32 | Índice de la primera fila. |
| firstColumn | Int32 | Índice de primera columna. |
| opciones | ImportTableOptions | Las opciones de importación |

### Valor de retorno

Número total de filas importadas.

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Crear tabla de datos de ejemplo
            DataTable dataTable = new DataTable("TestTable");
            dataTable.Columns.Add("Column1", typeof(string));
            dataTable.Columns.Add("Column2", typeof(int));
            
            // Agregar datos de ejemplo
            dataTable.Rows.Add("Data1", 100);
            dataTable.Rows.Add("Data2", 200);
            dataTable.Rows.Add("Data3", 300);

            // Crear ImportTableOptions
            ImportTableOptions options = new ImportTableOptions();
            options.IsFieldNameShown = true;
            options.InsertRows = true;

            // Importar datos desde DataView a celdas comenzando en la fila 0, columna 0
            cells.ImportData(dataTable.DefaultView, 0, 0, options);

            // Guarda el libro de trabajo
            workbook.Save("ImportDataOutput.xlsx");
        }
    }
}
```

### Ver también

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


