---
title: "LoadOptions.LoadOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor LoadOptions. Crea una opción de carga del archivo"
type: docs
url: /es/net/aspose.cells/loadoptions/loadoptions/
---
## LoadOptions() {#constructor}

Crea una opción de carga del archivo.

```csharp
public LoadOptions()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LoadOptionsMethodSharpctorDemo
    {
        public static void Run()
        {
            string tempCsvPath = "temp_input.csv";

            try
            {
                // Crea contenido CSV de ejemplo
                File.WriteAllText(tempCsvPath, "Name,Age\nJohn,30\nJane,25");

                // Demostrar el constructor predeterminado
                LoadOptions defaultOptions = new LoadOptions();
                Console.WriteLine("Default LoadFormat: " + defaultOptions.LoadFormat);

                // Demostrar el constructor con el parámetro LoadFormat
                LoadOptions csvOptions = new LoadOptions(LoadFormat.Csv);
                Console.WriteLine("CSV LoadFormat: " + csvOptions.LoadFormat);

                // Cargar archivo CSV con las opciones especificadas
                Workbook workbook = new Workbook(tempCsvPath, csvOptions);

                // Verificar que los datos se cargaron correctamente
                Worksheet worksheet = workbook.Worksheets[0];
                Console.WriteLine($"Cell A1: {worksheet.Cells["A1"].StringValue}");
                Console.WriteLine($"Cell B2: {worksheet.Cells["B2"].StringValue}");

                // Guardar como XLSX para demostrar la conversión
                workbook.Save("CsvToExcel.xlsx");
                Console.WriteLine("CSV file successfully loaded and converted to XLSX");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
            finally
            {
                if (File.Exists(tempCsvPath))
                    File.Delete(tempCsvPath);
            }
        }
    }
}
```

### Ver también

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## LoadOptions(LoadFormat) {#constructor_1}

Crea una opción de carga del archivo.

```csharp
public LoadOptions(LoadFormat loadFormat)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| loadFormat | LoadFormat | El formato de carga. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            string tempCsvPath = "temp_input.csv";
            
            try
            {
                // Crea contenido CSV de ejemplo
                File.WriteAllText(tempCsvPath, "Column1,Column2\nData1,Data2");

                // Crear LoadOptions con LoadFormat.Csv
                LoadOptions options = new LoadOptions(LoadFormat.Csv);

                // Cargar archivo CSV con las opciones creadas
                Workbook workbook = new Workbook(tempCsvPath, options);

                // Demostrar carga exitosa leyendo la celda
                Worksheet worksheet = workbook.Worksheets[0];
                Console.WriteLine($"A1 cell value: {worksheet.Cells["A1"].StringValue}");
                Console.WriteLine($"B2 cell value: {worksheet.Cells["B2"].StringValue}");

                // Guardar como XLSX para mostrar la capacidad de conversión
                workbook.Save("CsvLoadedAsExcel.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during CSV loading: {ex.Message}");
            }
            finally
            {
                if (File.Exists(tempCsvPath))
                    File.Delete(tempCsvPath);
            }
        }
    }
}
```

### Ver también

* enum [LoadFormat](../../loadformat/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


