---
title: "XmlSaveOptions.DataAsAttribute"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad XmlSaveOptions. Indica si los datos se exportan como atributos del elemento"
type: docs
url: /es/net/aspose.cells/xmlsaveoptions/dataasattribute/
---
## XmlSaveOptions.DataAsAttribute property

Indica si se exportan los datos como atributos del elemento.

```csharp
public bool DataAsAttribute { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertyDataAsAttributeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // Crear opciones de guardado XML con DataAsAttribute establecido en verdadero
            XmlSaveOptions saveOptions = new XmlSaveOptions
            {
                DataAsAttribute = true,
                SheetNameAsElementName = true
            };

            // Guardar con datos como atributos
            workbook.Save("DataAsAttribute_True.xml", saveOptions);

            // Cambiar para guardar datos como elementos
            saveOptions.DataAsAttribute = false;
            workbook.Save("DataAsAttribute_False.xml", saveOptions);
        }
    }
}
```

### Ver también

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


