---
title: "XmlLoadOptions.IgnoreRootAttributes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad XmlLoadOptions. Indica si se ignoran los atributos del elemento raíz"
type: docs
url: /es/net/aspose.cells/xmlloadoptions/ignorerootattributes/
---
## XmlLoadOptions.IgnoreRootAttributes property

Indica si se deben ignorar los atributos del elemento raíz.

```csharp
public bool IgnoreRootAttributes { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyIgnoreRootAttributesDemo
    {
        public static void Run()
        {
            // Crear opciones de carga XML y establecer IgnoreRootAttributes
            XmlLoadOptions options = new XmlLoadOptions();
            options.IgnoreRootAttributes = true;

            // Cargar el archivo XML con las opciones
            Workbook workbook = new Workbook("example.xml", options);

            // Acceder a los datos del XML cargado
            string cellValue = workbook.Worksheets[0].Cells["AH8"].StringValue;
            Console.WriteLine("Cell AH8 value: " + cellValue);

            // Guardar como XLSX
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


