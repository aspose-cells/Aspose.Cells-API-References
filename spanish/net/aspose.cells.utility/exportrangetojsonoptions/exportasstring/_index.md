---
title: "ExportRangeToJsonOptions.ExportAsString"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExportRangeToJsonOptions. Exporta el valor de cadena de las celdas a json"
type: docs
url: /es/net/aspose.cells.utility/exportrangetojsonoptions/exportasstring/
---
## ExportRangeToJsonOptions.ExportAsString property

Exporta el valor de cadena de las celdas a json.

```csharp
public bool ExportAsString { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class ExportRangeToJsonOptionsPropertyExportAsStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar celdas con diferentes tipos de datos
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("String");
            worksheet.Cells["B2"].PutValue("Hello");
            worksheet.Cells["A3"].PutValue("Number");
            worksheet.Cells["B3"].PutValue(123.45);
            worksheet.Cells["A4"].PutValue("Date");
            worksheet.Cells["B4"].PutValue(DateTime.Now);

            // Crear instancia de ExportRangeToJsonOptions
            ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();
            options.HasHeaderRow = true;

            // Mostrar valor actual de ExportAsString
            Console.WriteLine("Current ExportAsString value: " + options.ExportAsString);

            // Exportar sin ExportAsString (comportamiento predeterminado)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B4");
            string jsonWithoutString = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON without ExportAsString:\n" + jsonWithoutString);

            // Establecer ExportAsString a true
            options.ExportAsString = true;

            // Exportar con ExportAsString
            string jsonWithString = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON with ExportAsString:\n" + jsonWithString);

            // Guarda el libro de trabajo
            workbook.Save("ExportAsStringDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


