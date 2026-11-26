---
title: "XmlSaveOptions.SheetNameAsElementName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad XmlSaveOptions. Indica si se exporta el nombre de las hojas como el nombre del elemento"
type: docs
url: /es/net/aspose.cells/xmlsaveoptions/sheetnameaselementname/
---
## XmlSaveOptions.SheetNameAsElementName property

Indica si se exporta el nombre de la hoja como el nombre del elemento.

```csharp
public bool SheetNameAsElementName { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertySheetNameAsElementNameDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo con datos
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "EmployeeData";
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John Doe");

            // Guardar con SheetNameAsElementName = true (predeterminado)
            XmlSaveOptions saveOptions = new XmlSaveOptions();
            saveOptions.SheetNameAsElementName = true;
            workbook.Save("output_with_sheetname.xml", saveOptions);

            // Guardar con SheetNameAsElementName = false
            saveOptions.SheetNameAsElementName = false;
            workbook.Save("output_without_sheetname.xml", saveOptions);

            Console.WriteLine("XML files created successfully with different SheetNameAsElementName settings.");
        }
    }
}
```

### Ver también

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


