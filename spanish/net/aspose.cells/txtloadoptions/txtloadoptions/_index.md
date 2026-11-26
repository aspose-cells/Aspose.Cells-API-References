---
title: "TxtLoadOptions.TxtLoadOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor TxtLoadOptions. Crea las opciones para cargar un archivo de texto"
type: docs
url: /es/net/aspose.cells/txtloadoptions/txtloadoptions/
---
## TxtLoadOptions() {#constructor}

Crea las opciones para cargar un archivo de texto.

```csharp
public TxtLoadOptions()
```

### Observaciones

El tipo de archivo de carga predeterminado es CSV.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crea un nuevo TxtLoadOptions usando el constructor
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            
            // Establece el separador para el archivo CSV
            loadOptions.Separator = ',';
            
            // Crea un libro de trabajo con opciones de carga
            Workbook workbook = new Workbook("example.csv", loadOptions);
            
            // Muestra información del archivo cargado
            Console.WriteLine("Worksheet count: " + workbook.Worksheets.Count);
            Console.WriteLine("First cell value: " + workbook.Worksheets[0].Cells["A1"].Value);
        }
    }
}
```

### Ver también

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## TxtLoadOptions(LoadFormat) {#constructor_1}

Crea las opciones para cargar un archivo de texto.

```csharp
public TxtLoadOptions(LoadFormat loadFormat)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| loadFormat | LoadFormat | El formato de carga |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class TxtLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            // Crea contenido CSV de ejemplo y un archivo temporal
            string csvData = "Column1,Column2,Column3\nData1,Data2,Data3";
            string tempFile = Path.GetTempFileName();
            File.WriteAllText(tempFile, csvData);

            try
            {
                // Crea TxtLoadOptions con LoadFormat.Csv
                TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv);
                loadOptions.Separator = ',';
                loadOptions.HasTextQualifier = true;

                // Carga CSV usando las opciones configuradas
                Workbook workbook = new Workbook(tempFile, loadOptions);
                Worksheet worksheet = workbook.Worksheets[0];

                // Demuestra los datos cargados
                Console.WriteLine($"A1 Cell Value: {worksheet.Cells["A1"].StringValue}");
                Console.WriteLine($"B2 Cell Value: {worksheet.Cells["B2"].StringValue}");

                // Guardar libro de trabajo procesado
                workbook.Save("TxtLoadOptionsCtorDemoOutput.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing constructor: {ex.Message}");
            }
            finally
            {
                // Eliminar archivo temporal
                if (File.Exists(tempFile))
                {
                    File.Delete(tempFile);
                }
            }
        }
    }
}
```

### Ver también

* enum [LoadFormat](../../loadformat/)
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


