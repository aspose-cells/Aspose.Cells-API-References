---
title: "XmlSaveOptions.HasHeaderRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad XmlSaveOptions. Indica si el rango contiene fila de encabezado"
type: docs
url: /es/net/aspose.cells/xmlsaveoptions/hasheaderrow/
---
## XmlSaveOptions.HasHeaderRow property

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
    public class XmlSaveOptionsPropertyHasHeaderRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar fila de encabezado y datos
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crear opciones de guardado XML
            XmlSaveOptions saveOptions = new XmlSaveOptions();
            saveOptions.HasHeaderRow = true; // Demonstrate HasHeaderRow property
            saveOptions.SheetNameAsElementName = true;

            // Guardar como archivo XML
            workbook.Save("output.xml", saveOptions);

            Console.WriteLine("XML file saved with HasHeaderRow=true");
        }
    }
}
```

### Ver también

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


