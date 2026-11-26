---
title: "XmlSaveOptions.XmlSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor XmlSaveOptions. Crea opciones para guardar un archivo xml"
type: docs
url: /es/net/aspose.cells/xmlsaveoptions/xmlsaveoptions/
---
## XmlSaveOptions constructor

Crea opciones para guardar un archivo XML.

```csharp
public XmlSaveOptions()
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de muestra con datos de prueba
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(63);

            // Primera demostración: Guardar como XML con SheetNameAsElementName
            XmlSaveOptions saveOptions1 = new XmlSaveOptions();
            saveOptions1.SheetNameAsElementName = true;
            workbook.Save("output1.xml", saveOptions1);
            
            // Segunda demostración: Guardar como XML con SheetNameAsElementName y DataAsAttribute
            XmlSaveOptions saveOptions2 = new XmlSaveOptions();
            saveOptions2.SheetNameAsElementName = true;
            saveOptions2.DataAsAttribute = true;
            workbook.Save("output2.xml", saveOptions2);

            Console.WriteLine("XML files created successfully.");
        }
    }
}
```

### Ver también

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


