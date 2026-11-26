---
title: "Cells.ExportDataTable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Exporta datos de la colección Cells a un objeto DataTable"
type: docs
url: /es/net/aspose.cells/cells/exportdatatable/
---
## ExportDataTable(int, int, int, int) {#exportdatatable}

Exporta datos de la colección [`Cells`](../) a un objeto DataTable.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | Int32 | El número de fila de la primera celda a exportar. |
| firstColumn | Int32 | El número de columna de la primera celda a exportar. |
| totalRows | Int32 | Número de filas a importar. |
| totalColumns | Int32 | Número de columnas a importar. |

### Valor de retorno

Objeto DataTable exportado.

### Observaciones

Si utiliza este método para exportar un bloque de datos, asegúrese de que los datos en una columna sean del mismo tipo. De lo contrario, use el método [`ExportDataTableAsString`](../exportdatatableasstring/) en su lugar.

### Ejemplos

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
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["C1"].PutValue("City");
            
            for (int i = 1; i <= 5; i++)
            {
                worksheet.Cells[i, 0].PutValue($"Person {i}");
                worksheet.Cells[i, 1].PutValue(20 + i);
                worksheet.Cells[i, 2].PutValue($"City {i}");
            }

            // Exportar datos a DataTable (comenzando desde la fila 0, columna 0, con 5 filas y 3 columnas)
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 5, 3);

            // Mostrar los datos exportados
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine($"{row[0]}, {row[1]}, {row[2]}");
            }
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ExportDataTable(int, int, int, int, bool) {#exportdatatable_2}

Exporta datos de la colección [`Cells`](../) a un objeto DataTable.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool exportColumnName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | Int32 | El número de fila de la primera celda a exportar. |
| firstColumn | Int32 | El número de columna de la primera celda a exportar. |
| totalRows | Int32 | Número de filas a importar. |
| totalColumns | Int32 | Número de columnas a importar. |
| exportColumnName | Booleano | Indica si los datos de la primera fila se exportan al nombre de columna del DataTable. |

### Valor de retorno

Objeto DataTable exportado.

### Ejemplos

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
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Exportar datos a DataTable (la primera fila contiene encabezados)
            DataTable dt = worksheet.Cells.ExportDataTable(0, 0, 3, 2, true);

            // Mostrar los datos exportados
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dt.Rows)
            {
                Console.WriteLine($"{row["Name"]}, {row["Age"]}");
            }
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ExportDataTable(int, int, int, int, ExportTableOptions) {#exportdatatable_1}

Exporta datos de la colección [`Cells`](../) a un objeto DataTable.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    ExportTableOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | Int32 | El número de fila de la primera celda a exportar. |
| firstColumn | Int32 | El número de columna de la primera celda a exportar. |
| totalRows | Int32 | Número de filas a importar. |
| totalColumns | Int32 | Número de columnas a importar. |
| opciones | ExportTableOptions | Todas las opciones de exportación de tabla |

### Valor de retorno

Objeto DataTable exportado.

### Ejemplos

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
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Establecer valor y formato para la celda A1
            cells["A1"].PutValue(1.23356);
            Style style = cells["A1"].GetStyle();
            style.Custom = "0.00";
            cells["A1"].SetStyle(style);

            // Crea opciones de exportación
            ExportTableOptions etOpt = new ExportTableOptions();
            etOpt.ExportColumnName = false;
            etOpt.ExportAsString = true;

            // Exportar con la estrategia de formato CellStyle
            etOpt.FormatStrategy = CellValueFormatStrategy.CellStyle;
            DataTable dt1 = cells.ExportDataTable(0, 0, 1, 1, etOpt);
            Console.WriteLine("CellStyle format: " + dt1.Rows[0][0].ToString());

            // Exportar con la estrategia de formato None
            etOpt.FormatStrategy = CellValueFormatStrategy.None;
            DataTable dt2 = cells.ExportDataTable(0, 0, 1, 1, etOpt);
            Console.WriteLine("None format: " + dt2.Rows[0][0].ToString());

            // Exportar con la estrategia de formato DisplayStyle
            etOpt.FormatStrategy = CellValueFormatStrategy.DisplayStyle;
            DataTable dt3 = cells.ExportDataTable(0, 0, 1, 1, etOpt);
            Console.WriteLine("DisplayStyle format: " + dt3.Rows[0][0].ToString());
        }
    }
}
```

### Ver también

* class [ExportTableOptions](../../exporttableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


