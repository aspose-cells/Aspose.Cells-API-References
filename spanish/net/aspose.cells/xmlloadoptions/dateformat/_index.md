---
title: "XmlLoadOptions.DateFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad XmlLoadOptions. Obtiene y establece el formato del valor de fecha"
type: docs
url: /es/net/aspose.cells/xmlloadoptions/dateformat/
---
## XmlLoadOptions.DateFormat property

Obtiene y establece el formato del valor de fecha.

```csharp
public string DateFormat { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyDateFormatDemo
    {
        public static void Run()
        {
            // Crea una instancia de XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // Establecer el formato de fecha para analizar fechas del XML
            options.DateFormat = "yyyy-MM-dd";
            options.ConvertNumericOrDate = true;

            // Carga un archivo XML en un Workbook usando las opciones especificadas
            Workbook workbook = new Workbook("input.xml", options);

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Mostrar algunas celdas para demostrar el formato de fecha
            Console.WriteLine("Cell A1: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("Cell A2: " + worksheet.Cells["A2"].Value);

            // Guardar el libro de trabajo en un archivo nuevo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


