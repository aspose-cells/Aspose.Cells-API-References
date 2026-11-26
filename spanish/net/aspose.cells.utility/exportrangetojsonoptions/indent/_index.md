---
title: "ExportRangeToJsonOptions.Indent"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExportRangeToJsonOptions. Indica la sangría"
type: docs
url: /es/net/aspose.cells.utility/exportrangetojsonoptions/indent/
---
## ExportRangeToJsonOptions.Indent property

Indica la sangría.

```csharp
public string Indent { get; set; }
```

### Observaciones

Si la sangría es nula o vacía, el JSON exportado no está formateado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class ExportRangeToJsonOptionsPropertyIndentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rellene datos de ejemplo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crear instancia de ExportRangeToJsonOptions
            ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();
            options.HasHeaderRow = true;

            // Mostrar sangría actual (el valor predeterminado es null)
            Console.WriteLine("Current Indent value: " + (options.Indent ?? "null"));

            // Exportar con sangría predeterminada (JSON compacto)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");
            string jsonWithoutIndent = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON without indent:\n" + jsonWithoutIndent);

            // Establecer sangría a 4 espacios
            options.Indent = "    ";
            string jsonWithIndent = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("\nJSON with 4-space indent:\n" + jsonWithIndent);

            // Establecer sangría al carácter de tabulación
            options.Indent = "\t";
            string jsonWithTabIndent = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("\nJSON with tab indent:\n" + jsonWithTabIndent);
        }
    }
}
```

### Ver también

* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


