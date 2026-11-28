---
title: "JsonSaveOptions.SheetIndexes"
second_title: "Aspose.Cells için .NET API Referansı"
description: "JsonSaveOptions özelliği. Dışa aktarılan sayfaların indekslerini temsil eder"
type: docs
url: /tr/net/aspose.cells/jsonsaveoptions/sheetindexes/
---
## JsonSaveOptions.SheetIndexes property

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

    public class JsonSaveOptionsPropertySheetIndexesDemo
    {
        public static void Run()
        {
            // Birden çok sayfa içeren yeni bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Her sayfada bazı verileri doldur
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet sheet = workbook.Worksheets[i];
                sheet.Cells["A1"].PutValue($"Data from Sheet {i + 1}");
            }

            // JsonSaveOptions örneği oluştur
            JsonSaveOptions options = new JsonSaveOptions();

            // Mevcut SheetIndexes'i göster (varsayılan olarak null - tüm sayfaları dışa aktarır)
            Console.WriteLine("Current SheetIndexes: " + (options.SheetIndexes == null ? "Exporting all sheets" : string.Join(",", options.SheetIndexes)));

            // Yalnızca birinci ve üçüncü sayfaları dışa aktaracak şekilde ayarlayın (indeksler 0 ve 2)
            options.SheetIndexes = new int[] { 0, 2 };

            // Seçili sayfalarla JSON'a kaydet
            workbook.Save("JsonSaveOptionsPropertySheetIndexesDemo.json", options);

            // JSON'ı yükleyerek doğrula
            string jsonContent = System.IO.File.ReadAllText("JsonSaveOptionsPropertySheetIndexesDemo.json");
            Console.WriteLine("JSON Content:");
            Console.WriteLine(jsonContent);

            // Yalnızca ikinci sayfayı dışa aktaracak şekilde değiştirin (indeks 1)
            options.SheetIndexes = new int[] { 1 };
            workbook.Save("JsonSaveOptionsPropertySheetIndexesDemo_SingleSheet.json", options);

            // Tek sayfa dışa aktarmayı doğrula
            jsonContent = System.IO.File.ReadAllText("JsonSaveOptionsPropertySheetIndexesDemo_SingleSheet.json");
            Console.WriteLine("Single Sheet JSON Content:");
            Console.WriteLine(jsonContent);
        }
    }
}
```

### Ayrıca Bakınız

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


