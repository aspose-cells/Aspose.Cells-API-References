---
title: "XmlLoadOptions.IsXmlMap"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad XmlLoadOptions. Indica si se mapea xml a Excel. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/xmlloadoptions/isxmlmap/
---
## XmlLoadOptions.IsXmlMap property

Indica si se mapea xml a Excel. El valor predeterminado es false.

```csharp
public bool IsXmlMap { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyIsXmlMapDemo
    {
        public static void Run()
        {
            // Crea una instancia de XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // Habilitar el mapeo XML al cargar el archivo
            options.IsXmlMap = true;

            // Carga un archivo XML en un Workbook usando las opciones especificadas
            Workbook workbook = new Workbook("sample.xml", options);

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Mostrar algunos datos del XML cargado para demostrar el mapeo exitoso
            Console.WriteLine("Data from loaded XML:");
            Console.WriteLine(worksheet.Cells["A1"].StringValue);
            Console.WriteLine(worksheet.Cells["A2"].StringValue);

            // Guardar el libro de trabajo en un nuevo archivo Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


