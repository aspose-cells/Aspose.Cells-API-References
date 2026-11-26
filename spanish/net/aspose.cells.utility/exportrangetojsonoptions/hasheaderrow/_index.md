---
title: "ExportRangeToJsonOptions.HasHeaderRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExportRangeToJsonOptions. Indica si el rango contiene fila de encabezado"
type: docs
url: /es/net/aspose.cells.utility/exportrangetojsonoptions/hasheaderrow/
---
## ExportRangeToJsonOptions.HasHeaderRow property

Indica si el rango contiene una fila de encabezado.

```csharp
public bool HasHeaderRow { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class ExportRangeToJsonOptionsPropertyHasHeaderRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar datos de muestra con encabezados
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            // Crear rango para exportar
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            // Crear instancia de ExportRangeToJsonOptions
            ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();

            // Mostrar valor actual de HasHeaderRow (el predeterminado es false)
            Console.WriteLine("Current HasHeaderRow value: " + options.HasHeaderRow);

            // Establecer HasHeaderRow a true
            options.HasHeaderRow = true;
            Console.WriteLine("New HasHeaderRow value: " + options.HasHeaderRow);

            // Exportar a JSON con encabezados
            string jsonWithHeaders = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON with headers:\n" + jsonWithHeaders);

            // Establecer HasHeaderRow a false
            options.HasHeaderRow = false;
            Console.WriteLine("New HasHeaderRow value: " + options.HasHeaderRow);

            // Exportar a JSON sin encabezados
            string jsonWithoutHeaders = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON without headers:\n" + jsonWithoutHeaders);

            // Guarda el libro de trabajo
            workbook.Save("PropertyHasHeaderRowDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


