---
title: "Cells.ImportCSV"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Importa un archivo CSV a las celdas"
type: docs
url: /es/net/aspose.cells/cells/importcsv/
---
## ImportCSV(string, string, bool, int, int) {#importcsv_3}

Importa un archivo CSV a las celdas.

```csharp
public void ImportCSV(string fileName, string splitter, bool convertNumericData, int firstRow, 
    int firstColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | String | El nombre del archivo CSV. |
| divisor | String | El divisor |
| convertNumericData | Booleano | Indica si la cadena en el archivo de texto se convierte a datos numéricos. |
| firstRow | Int32 | El número de fila de la primera celda en la que importar. |
| firstColumn | Int32 | El número de columna de la primera celda en la que importar. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportCSVWithStringStringBooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ruta al archivo CSV
            string csvPath = "example.csv";
            
            // Importa datos CSV comenzando en la celda A1 (fila 0, columna 0)
            // Usando punto y coma como delimitador y convirtiendo datos numéricos
            cells.ImportCSV(csvPath, ";", true, 0, 0);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportCSV(Stream, string, bool, int, int) {#importcsv_1}

Importa un archivo CSV a las celdas.

```csharp
public void ImportCSV(Stream stream, string splitter, bool convertNumericData, int firstRow, 
    int firstColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | Stream | El flujo del archivo CSV. |
| divisor | String | El divisor |
| convertNumericData | Booleano | Indica si la cadena en el archivo de texto se convierte a datos numéricos. |
| firstRow | Int32 | El número de fila de la primera celda en la que importar. |
| firstColumn | Int32 | El número de columna de la primera celda en la que importar. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsMethodImportCSVWithStreamStringBooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crear datos CSV de ejemplo en memoria
            string csvData = "Name,Age,City\nJohn,30,New York\nAlice,25,London\nBob,35,Paris";
            byte[] byteArray = System.Text.Encoding.UTF8.GetBytes(csvData);
            MemoryStream csvStream = new MemoryStream(byteArray);

            try
            {
                // Llamar al método ImportCSV con los parámetros Stream, String, Boolean, Int32, Int32
                cells.ImportCSV(csvStream, ",", true, 0, 0);

                Console.WriteLine("CSV data imported successfully to worksheet.");
                Console.WriteLine($"Data range: A1 to {cells.MaxDisplayRange}");

                // Guarda el libro de trabajo
                workbook.Save("ImportCSVFromStreamDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing CSV: {ex.Message}");
            }
            finally
            {
                csvStream?.Dispose();
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

## ImportCSV(string, TxtLoadOptions, int, int) {#importcsv_2}

Importa un archivo CSV a las celdas.

```csharp
public void ImportCSV(string fileName, TxtLoadOptions options, int firstRow, int firstColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | String | El nombre del archivo CSV. |
| opciones | TxtLoadOptions | Las opciones de carga para leer el archivo de texto |
| firstRow | Int32 | El número de fila de la primera celda en la que importar. |
| firstColumn | Int32 | El número de columna de la primera celda en la que importar. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportCSVWithStringTxtLoadOptionsInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear opciones de carga CSV
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.Separator = ',';
            loadOptions.ConvertDateTimeData = true;
            loadOptions.ConvertNumericData = true;
            loadOptions.ParsingFormulaOnOpen = true;

            // Ruta del archivo CSV de ejemplo (reemplazar con la ruta real en su entorno)
            string csvFilePath = "example.csv";
            
            // Importa datos CSV comenzando en la celda A1 (fila 0, columna 0)
            worksheet.Cells.ImportCSV(csvFilePath, loadOptions, 0, 0);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [TxtLoadOptions](../../txtloadoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportCSV(Stream, TxtLoadOptions, int, int) {#importcsv}

Importa un archivo CSV a las celdas.

```csharp
public void ImportCSV(Stream stream, TxtLoadOptions options, int firstRow, int firstColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | Stream | El flujo del archivo CSV. |
| opciones | TxtLoadOptions | Las opciones de carga para leer el archivo de texto |
| firstRow | Int32 | El número de fila de la primera celda en la que importar. |
| firstColumn | Int32 | El número de columna de la primera celda en la que importar. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsMethodImportCSVWithStreamTxtLoadOptionsInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtener la colección Cells
            Cells cells = worksheet.Cells;

            // Crear datos CSV de ejemplo
            string csvData = "Name,Age,City\nJohn,30,New York\nJane,25,Los Angeles\nBob,35,Chicago";

            // Crear un flujo de memoria con los datos CSV
            MemoryStream csvStream = new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData));

            try
            {
                // Crear TxtLoadOptions para la importación de CSV
                TxtLoadOptions loadOptions = new TxtLoadOptions();
                loadOptions.Separator = ',';
                loadOptions.ConvertNumericData = true;

                // Importar datos CSV comenzando en la fila 0, columna 0
                cells.ImportCSV(csvStream, loadOptions, 0, 0);

                // Guarda el libro de trabajo
                workbook.Save("ImportCSVDemo.xlsx");

                Console.WriteLine("CSV data imported successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing CSV: {ex.Message}");
            }
            finally
            {
                // Liberar el flujo
                csvStream.Dispose();
            }
        }
    }
}
```

### Ver también

* class [TxtLoadOptions](../../txtloadoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


