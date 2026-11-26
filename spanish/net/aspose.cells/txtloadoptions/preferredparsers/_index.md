---
title: "TxtLoadOptions.PreferredParsers"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TxtLoadOptions. Obtiene y establece analizadores de valores preferidos para cargar archivos de texto"
type: docs
url: /es/net/aspose.cells/txtloadoptions/preferredparsers/
---
## TxtLoadOptions.PreferredParsers property

Obtiene y establece los analizadores de valores preferidos para cargar un archivo de texto.

```csharp
public ICustomParser[] PreferredParsers { get; set; }
```

### Observaciones

parsers[0] es el analizador que se usará para la primera columna en el archivo de plantilla de texto, parsers[1] es el analizador que se usará para la segunda columna, ...etc. El último (parsers[parsers.length-1]) se usará para todas las demás columnas a partir de parsers.length-1. Si un elemento es null, la columna correspondiente será analizada por el analizador predeterminado de Aspose.Cells.

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyPreferredParsersDemo
    {
        private class StringParser : ICustomParser
        {
            public bool Parse(string value, out object result)
            {
                result = value; // Always return as string
                return true;
            }

            public object ParseObject(string value)
            {
                return value; // Always return as string
            }

            public string GetFormat()
            {
                return "String"; // Return format description
            }
        }

        public static void Run()
        {
            // Crear opciones de carga CSV
            TxtLoadOptions options = new TxtLoadOptions(LoadFormat.Csv);
            
            // Establece analizadores preferidos - primero prueba el analizador de cadena personalizado, luego los analizadores predeterminados
            options.PreferredParsers = new ICustomParser[] { new StringParser(), null };

            // Datos CSV de ejemplo con fechas
            string csvData = "\"2018-10-08\",2018-10-08\n\"2018-10-08\",2018-10-08";
            
            // Cargar libro de trabajo con opciones
            Workbook workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);
            Cells cells = workbook.Worksheets[0].Cells;

            // Verifica los resultados del análisis
            Console.WriteLine("A1 Type: " + cells[0, 0].Type); // Should be string
            Console.WriteLine("A1 Value: " + cells[0, 0].StringValue); // "2018-10-08"
            Console.WriteLine("B1 Type: " + cells[0, 1].Type); // Should be DateTime
            Console.WriteLine("B1 Value: " + cells[0, 1].DateTimeValue); // 10/8/2018
        }
    }
}
```

### Ver también

* interface [ICustomParser](../../icustomparser/)
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


