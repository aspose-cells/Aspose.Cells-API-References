---
title: "OdsLoadOptions.OdsLoadOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor OdsLoadOptions. Representa las opciones de carga del archivo ods"
type: docs
url: /es/net/aspose.cells/odsloadoptions/odsloadoptions/
---
## OdsLoadOptions() {#constructor}

Representa las opciones de carga de archivos ODS.

```csharp
public OdsLoadOptions()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OdsLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crear OdsLoadOptions usando el constructor
            OdsLoadOptions loadOptions = new OdsLoadOptions();
            
            // Establecer el estilo de hipervínculo para usar los valores predeterminados de Excel
            loadOptions.ApplyExcelDefaultStyleToHyperlink = true;
            
            // Cargar el archivo ODS con las opciones de carga
            Workbook workbook = new Workbook("example.ods", loadOptions);
            
            // Guardar como XLSX
            workbook.Save("output.xlsx");
            
            // Verificar que se aplicó el estilo de hipervínculo
            Console.WriteLine("Hyperlink style color: " + 
                workbook.Worksheets[0].Cells["B1"].GetStyle().Font.Color);
        }
    }
}
```

### Ver también

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## OdsLoadOptions(LoadFormat) {#constructor_1}

Representa las opciones de carga de archivos ODS.

```csharp
public OdsLoadOptions(LoadFormat type)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | LoadFormat | El tipo de formato de carga. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class OdsLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            // Crear un archivo ODS de muestra si no existe
            string inputFile = "input.ods";
            if (!File.Exists(inputFile))
            {
                using (Workbook sampleWorkbook = new Workbook())
                {
                    sampleWorkbook.Worksheets[0].Hyperlinks.Add("A1", 1, 1, "https://example.com");
                    sampleWorkbook.Save(inputFile, SaveFormat.Ods);
                }
            }

            // Crear OdsLoadOptions con el parámetro LoadFormat
            OdsLoadOptions loadOptions = new OdsLoadOptions(LoadFormat.Ods);
            loadOptions.ApplyExcelDefaultStyleToHyperlink = true;

            try
            {
                // Cargar el libro de trabajo con las opciones de carga creadas
                using (Workbook workbook = new Workbook(inputFile, loadOptions))
                {
                    Console.WriteLine($"Hyperlink style applied: {loadOptions.ApplyExcelDefaultStyleToHyperlink}");
                    
                    // Guardar para demostrar la carga exitosa
                    workbook.Save("OdsLoadOptionsCtorDemo.xlsx");
                }
            }
            catch (FileNotFoundException)
            {
                Console.WriteLine("Error: Created sample file missing - please verify permissions");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading ODS file: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [LoadFormat](../../loadformat/)
* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


