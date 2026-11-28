---
title: "XmlSaveOptions.SheetIndexes"
second_title: "Aspose.Cells için .NET API Referansı"
description: "XmlSaveOptions özelliği. Dışa aktarılan sayfaların indekslerini temsil eder"
type: docs
url: /tr/net/aspose.cells/xmlsaveoptions/sheetindexes/
---
## XmlSaveOptions.SheetIndexes property

Dışa aktarılan sayfaların indekslerini temsil eder.

```csharp
public int[] SheetIndexes { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XmlSaveOptionsPropertySheetIndexesDemo
    {
        public static void Run()
        {
            // Birden çok sayfa içeren yeni bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Tüm sayfalara bazı veriler ekleyin
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet sheet = workbook.Worksheets[i];
                sheet.Cells["A1"].PutValue("Data in " + sheet.Name);
            }

            // XmlSaveOptions örneği oluşturun
            XmlSaveOptions options = new XmlSaveOptions();

            // Başlangıçta tüm sayfaları dışa aktar (SheetIndexes null'dur)
            Console.WriteLine("Initial SheetIndexes value: " + (options.SheetIndexes == null ? "null (all sheets)" : string.Join(",", options.SheetIndexes)));

            // Yalnızca birinci ve üçüncü sayfaları dışa aktaracak şekilde ayarlayın (indeksler 0 ve 2)
            options.SheetIndexes = new int[] { 0, 2 };

            // Yalnızca seçilen sayfalarla kaydedin
            workbook.Save("XmlExportSelectedSheets.xml", options);

            // Yalnızca ikinci sayfayı dışa aktaracak şekilde değiştirin (indeks 1)
            options.SheetIndexes = new int[] { 1 };

            // Farklı sayfa seçimiyle kaydedin
            workbook.Save("XmlExportSingleSheet.xml", options);

            // Tüm sayfaları dışa aktarmak için SheetIndexes'i null olarak ayarlayın
            options.SheetIndexes = null;
            workbook.Save("XmlExportAllSheets.xml", options);
        }
    }
}
```

### Ayrıca Bakınız

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


