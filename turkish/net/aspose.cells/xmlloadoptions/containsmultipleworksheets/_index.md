---
title: "XmlLoadOptions.ContainsMultipleWorksheets"
second_title: "Aspose.Cells için .NET API Referansı"
description: "XmlLoadOptions özelliği. XML'in birden fazla çalışma sayfası olarak içe aktarılıp aktarılmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells/xmlloadoptions/containsmultipleworksheets/
---
## XmlLoadOptions.ContainsMultipleWorksheets property

XML'in birden çok çalışma sayfası olarak içe aktarılıp aktarılmadığını gösterir.

```csharp
public bool ContainsMultipleWorksheets { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyContainsMultipleWorksheetsDemo
    {
        public static void Run()
        {
            // Birden fazla çalışma sayfasına sahip örnek bir Excel dosyası oluşturun
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets[0].Cells["A1"].PutValue("Data from Sheet1");
            workbook.Worksheets[1].Cells["A1"].PutValue("Data from Sheet2");
            workbook.Save("output.xlsx", SaveFormat.Xlsx);

            // Birden fazla çalışma sayfası ile XML olarak kaydedin
            XmlSaveOptions saveOptions = new XmlSaveOptions();
            saveOptions.SheetNameAsElementName = false;
            workbook.Save("output.xml", saveOptions);

            // ContainsMultipleWorksheets=true ile XML'i yükleyin
            XmlLoadOptions loadOptions = new XmlLoadOptions();
            loadOptions.ContainsMultipleWorksheets = true;
            Workbook loadedWorkbook = new Workbook("output.xml", loadOptions);

            // Her iki çalışma sayfasının da yüklendiğini doğrulayın
            Console.WriteLine("Worksheet Count: " + loadedWorkbook.Worksheets.Count);
            Console.WriteLine("Sheet1 Data: " + loadedWorkbook.Worksheets[0].Cells["A1"].StringValue);
            Console.WriteLine("Sheet2 Data: " + loadedWorkbook.Worksheets[1].Cells["A1"].StringValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


