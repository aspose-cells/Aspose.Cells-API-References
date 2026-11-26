---
title: "JsonLayoutOptions.DateFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad JsonLayoutOptions. Obtiene y establece el formato del valor de fecha"
type: docs
url: /es/net/aspose.cells.utility/jsonlayoutoptions/dateformat/
---
## JsonLayoutOptions.DateFormat property

Obtiene y establece el formato del valor de fecha.

```csharp
public string DateFormat { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyDateFormatDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Configurar opciones de importación JSON con formato de fecha personalizado
            JsonLayoutOptions layoutOptions = new JsonLayoutOptions();
            layoutOptions.ArrayAsTable = true;
            layoutOptions.ConvertNumericOrDate = true;
            layoutOptions.DateFormat = "DD-MM-YYYY";

            // Importar datos JSON con valores de fecha
            string jsonData = "{\"date\":\"15-05-2023\",\"name\":\"John Doe\"}";
            JsonUtility.ImportData(jsonData, worksheet.Cells, 0, 0, layoutOptions);

            // Verificar que la fecha se haya importado con el formato correcto
            Cell dateCell = worksheet.Cells["A2"];
            Console.WriteLine("Imported date value: " + dateCell.StringValue);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


