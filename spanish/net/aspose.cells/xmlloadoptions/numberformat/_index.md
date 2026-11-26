---
title: "XmlLoadOptions.NumberFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad XmlLoadOptions. Obtiene y establece el formato del valor numérico"
type: docs
url: /es/net/aspose.cells/xmlloadoptions/numberformat/
---
## XmlLoadOptions.NumberFormat property

Obtiene y establece el formato del valor numérico.

```csharp
public string NumberFormat { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyNumberFormatDemo
    {
        public static void Run()
        {
            // Crea una instancia de XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // Establecer la propiedad NumberFormat para mostrar números con 2 decimales
            options.NumberFormat = "0.00";

            // Carga un archivo XML en un Workbook usando las opciones especificadas
            Workbook workbook = new Workbook("input.xml", options);

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer algunos valores numéricos para demostrar el formato de números
            worksheet.Cells["A1"].PutValue(123);
            worksheet.Cells["A2"].PutValue(45.678);
            worksheet.Cells["A3"].PutValue(0.5);

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


