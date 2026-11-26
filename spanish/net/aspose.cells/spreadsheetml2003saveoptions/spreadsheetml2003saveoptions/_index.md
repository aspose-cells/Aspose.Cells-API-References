---
title: "SpreadsheetML2003SaveOptions.SpreadsheetML2003SaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor de SpreadsheetML2003SaveOptions. Crea las opciones para guardar un archivo spreadml de Excel 2003"
type: docs
url: /es/net/aspose.cells/spreadsheetml2003saveoptions/spreadsheetml2003saveoptions/
---
## SpreadsheetML2003SaveOptions() {#constructor}

Crea las opciones para guardar un archivo spreadml de Excel 2003.

```csharp
public SpreadsheetML2003SaveOptions()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetML2003SaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo y agregar algunos datos de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(DateTime.Now);

            // Crear SpreadsheetML2003SaveOptions con el constructor
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();
            
            // Establecer opciones
            saveOptions.LimitAsXls = true;
            saveOptions.ExportColumnIndexOfCell = true;

            // Guardar con las opciones
            workbook.Save("output.xml", saveOptions);
            
            Console.WriteLine("File saved with SpreadsheetML2003SaveOptions");
        }
    }
}
```

### Ver también

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SpreadsheetML2003SaveOptions(SaveFormat) {#constructor_1}

Crea las opciones para guardar un archivo spreadml de Excel 2003.

```csharp
[Obsolete("Use SpreadsheetML2003SaveOptions() constructor instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SpreadsheetML2003SaveOptions(SaveFormat saveFormat)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| saveFormat | SaveFormat | El formato de guardado. |

### Observaciones

NOTA: Este constructor está ahora obsoleto. En su lugar, utilice el constructor SpreadsheetML2003SaveOptions(). Esta propiedad será eliminada 12 meses después, desde enero de 2021. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SpreadsheetML2003SaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue(123.45);

            try
            {
                // Llamar al método #ctor con el parámetro SaveFormat
                SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();

                // Establecer algunas propiedades de las opciones de guardado
                saveOptions.IsIndentedFormatting = true;
                saveOptions.LimitAsXls = false;
                saveOptions.ExportColumnIndexOfCell = true;

                Console.WriteLine("SpreadsheetML2003SaveOptions created successfully with SaveFormat parameter");

                // Guardar el libro de trabajo usando las opciones de guardado creadas
                workbook.Save("SpreadsheetML2003Output.xml", saveOptions);
                Console.WriteLine("Workbook saved successfully with SpreadsheetML2003SaveOptions");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SpreadsheetML2003SaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [SaveFormat](../../saveformat/)
* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


