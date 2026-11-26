---
title: "JsonSaveOptions.HasHeaderRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad JsonSaveOptions. Indica si el rango contiene fila de encabezado"
type: docs
url: /es/net/aspose.cells/jsonsaveoptions/hasheaderrow/
---
## JsonSaveOptions.HasHeaderRow property

Indica si el rango contiene una fila de encabezado.

```csharp
public bool HasHeaderRow { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyHasHeaderRowDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar fila de encabezado
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            
            // Agregar filas de datos
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crear rango (A1:B3)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 3, 2);

            // Exportar a JSON con HasHeaderRow = true (predeterminado)
            JsonSaveOptions options1 = new JsonSaveOptions();
            options1.HasHeaderRow = true;
            string jsonWithHeaders = Aspose.Cells.Utility.JsonUtility.ExportRangeToJson(range, options1);
            Console.WriteLine("JSON with headers:\n" + jsonWithHeaders);

            // Exportar a JSON con HasHeaderRow = false
            JsonSaveOptions options2 = new JsonSaveOptions();
            options2.HasHeaderRow = false;
            string jsonWithoutHeaders = Aspose.Cells.Utility.JsonUtility.ExportRangeToJson(range, options2);
            Console.WriteLine("\nJSON without headers:\n" + jsonWithoutHeaders);
        }
    }
}
```

### Ver también

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


