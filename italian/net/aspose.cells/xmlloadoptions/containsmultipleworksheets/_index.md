---
title: "XmlLoadOptions.ContainsMultipleWorksheets"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà XmlLoadOptions. Indica se l'importazione xml avviene come più fogli di lavoro"
type: docs
url: /it/net/aspose.cells/xmlloadoptions/containsmultipleworksheets/
---
## XmlLoadOptions.ContainsMultipleWorksheets property

Indica se importare XML come più fogli di lavoro.

```csharp
public bool ContainsMultipleWorksheets { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyContainsMultipleWorksheetsDemo
    {
        public static void Run()
        {
            // Crea un file Excel di esempio con più fogli di lavoro
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets[0].Cells["A1"].PutValue("Data from Sheet1");
            workbook.Worksheets[1].Cells["A1"].PutValue("Data from Sheet2");
            workbook.Save("output.xlsx", SaveFormat.Xlsx);

            // Salva come XML con più fogli di lavoro
            XmlSaveOptions saveOptions = new XmlSaveOptions();
            saveOptions.SheetNameAsElementName = false;
            workbook.Save("output.xml", saveOptions);

            // Carica l'XML con ContainsMultipleWorksheets=true
            XmlLoadOptions loadOptions = new XmlLoadOptions();
            loadOptions.ContainsMultipleWorksheets = true;
            Workbook loadedWorkbook = new Workbook("output.xml", loadOptions);

            // Verifica che entrambi i fogli di lavoro siano stati caricati
            Console.WriteLine("Worksheet Count: " + loadedWorkbook.Worksheets.Count);
            Console.WriteLine("Sheet1 Data: " + loadedWorkbook.Worksheets[0].Cells["A1"].StringValue);
            Console.WriteLine("Sheet2 Data: " + loadedWorkbook.Worksheets[1].Cells["A1"].StringValue);
        }
    }
}
```

### Vedi anche

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


