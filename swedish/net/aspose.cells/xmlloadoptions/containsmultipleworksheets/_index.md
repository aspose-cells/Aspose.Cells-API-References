---
title: "XmlLoadOptions.ContainsMultipleWorksheets"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XmlLoadOptions‑egenskap. Anger om XML importeras som flera arbetsblad"
type: docs
url: /sv/net/aspose.cells/xmlloadoptions/containsmultipleworksheets/
---
## XmlLoadOptions.ContainsMultipleWorksheets property

Anger om xml importeras som flera kalkylblad.

```csharp
public bool ContainsMultipleWorksheets { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyContainsMultipleWorksheetsDemo
    {
        public static void Run()
        {
            // Skapa en exempel‑Excel‑fil med flera arbetsblad
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets[0].Cells["A1"].PutValue("Data from Sheet1");
            workbook.Worksheets[1].Cells["A1"].PutValue("Data from Sheet2");
            workbook.Save("output.xlsx", SaveFormat.Xlsx);

            // Spara som XML med flera arbetsblad
            XmlSaveOptions saveOptions = new XmlSaveOptions();
            saveOptions.SheetNameAsElementName = false;
            workbook.Save("output.xml", saveOptions);

            // Läs in XML‑filen med ContainsMultipleWorksheets=true
            XmlLoadOptions loadOptions = new XmlLoadOptions();
            loadOptions.ContainsMultipleWorksheets = true;
            Workbook loadedWorkbook = new Workbook("output.xml", loadOptions);

            // Verifiera att båda arbetsbladen har lästs in
            Console.WriteLine("Worksheet Count: " + loadedWorkbook.Worksheets.Count);
            Console.WriteLine("Sheet1 Data: " + loadedWorkbook.Worksheets[0].Cells["A1"].StringValue);
            Console.WriteLine("Sheet2 Data: " + loadedWorkbook.Worksheets[1].Cells["A1"].StringValue);
        }
    }
}
```

### Se även

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


