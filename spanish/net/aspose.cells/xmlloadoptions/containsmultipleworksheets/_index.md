---
title: "XmlLoadOptions.ContainsMultipleWorksheets"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de XmlLoadOptions. Indica si se importa xml como varias hojas de cálculo"
type: docs
url: /es/net/aspose.cells/xmlloadoptions/containsmultipleworksheets/
---
## XmlLoadOptions.ContainsMultipleWorksheets property

Indica si se importa XML como múltiples hojas de cálculo.

```csharp
public bool ContainsMultipleWorksheets { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyContainsMultipleWorksheetsDemo
    {
        public static void Run()
        {
            // Crear un archivo Excel de ejemplo con varias hojas de cálculo
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets[0].Cells["A1"].PutValue("Data from Sheet1");
            workbook.Worksheets[1].Cells["A1"].PutValue("Data from Sheet2");
            workbook.Save("output.xlsx", SaveFormat.Xlsx);

            // Guardar como XML con varias hojas de cálculo
            XmlSaveOptions saveOptions = new XmlSaveOptions();
            saveOptions.SheetNameAsElementName = false;
            workbook.Save("output.xml", saveOptions);

            // Cargar el XML con ContainsMultipleWorksheets=true
            XmlLoadOptions loadOptions = new XmlLoadOptions();
            loadOptions.ContainsMultipleWorksheets = true;
            Workbook loadedWorkbook = new Workbook("output.xml", loadOptions);

            // Verificar que ambas hojas de cálculo fueron cargadas
            Console.WriteLine("Worksheet Count: " + loadedWorkbook.Worksheets.Count);
            Console.WriteLine("Sheet1 Data: " + loadedWorkbook.Worksheets[0].Cells["A1"].StringValue);
            Console.WriteLine("Sheet2 Data: " + loadedWorkbook.Worksheets[1].Cells["A1"].StringValue);
        }
    }
}
```

### Ver también

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


