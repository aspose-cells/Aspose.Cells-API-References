---
title: "AbstractTextLoadOptions.ConvertDateTimeData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AbstractTextLoadOptions. Obtiene o establece un valor que indica si la cadena en el archivo de texto se convierte en datos de fecha. El valor predeterminado es true"
type: docs
url: /es/net/aspose.cells/abstracttextloadoptions/convertdatetimedata/
---
## AbstractTextLoadOptions.ConvertDateTimeData property

Obtiene o establece un valor que indica si la cadena en el archivo de texto se convierte en datos de fecha. El valor predeterminado es true.

```csharp
public bool ConvertDateTimeData { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyConvertDateTimeDataDemo
    {
        public static void Run()
        {
            // Crear datos CSV con una cadena de fecha
            string csvData = "\"2023-05-15\",\"123.45\"";

            // Crear opciones de carga de texto con ConvertDateTimeData establecido en false
            TxtLoadOptions options = new TxtLoadOptions(LoadFormat.Csv);
            options.ConvertDateTimeData = false;
            options.ConvertNumericData = false;

            // Cargar los datos CSV
            Workbook workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);
            Worksheet worksheet = workbook.Worksheets[0];

            // Mostrar los valores (deberían permanecer como cadenas)
            Console.WriteLine("Cell A1 value: " + worksheet.Cells[0, 0].StringValue); // Outputs "2023-05-15" as string
            Console.WriteLine("Cell B1 value: " + worksheet.Cells[0, 1].StringValue); // Outputs "123.45" as string

            // Ahora cargue con ConvertDateTimeData configurado en true
            options.ConvertDateTimeData = true;
            options.ConvertNumericData = true;
            workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);
            worksheet = workbook.Worksheets[0];

            // Salida de los valores convertidos
            Console.WriteLine("Cell A1 value (converted): " + worksheet.Cells[0, 0].DateTimeValue); // Outputs DateTime
            Console.WriteLine("Cell B1 value (converted): " + worksheet.Cells[0, 1].DoubleValue);  // Outputs 123.45 as double
        }
    }
}
```

### Ver también

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


