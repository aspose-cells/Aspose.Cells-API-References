---
title: "LoadOptions.LoadFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LoadOptions özelliği. Yükleme formatını alır"
type: docs
url: /tr/net/aspose.cells/loadoptions/loadformat/
---
## LoadOptions.LoadFormat property

Yükleme biçimini alır.

```csharp
public LoadFormat LoadFormat { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LoadOptionsPropertyLoadFormatDemo
    {
        public static void Run()
        {
            // Örnek CSV dosyası oluştur
            File.WriteAllText("sample.csv", "Name,Age\nJohn,30\nAlice,25");

            // CSV formatı için LoadOptions oluştur ve özelliği göster
            LoadOptions csvOptions = new LoadOptions(LoadFormat.Csv);
            Console.WriteLine("CSV LoadFormat: " + csvOptions.LoadFormat);

            // Doğru seçeneklerle CSV'yi yükle
            Workbook csvWorkbook = new Workbook("sample.csv", csvOptions);
            Console.WriteLine("CSV loaded cells: " + csvWorkbook.Worksheets[0].Cells["B1"].Value);

            // XLSX formatı için LoadOptions oluştur ve özelliği göster
            LoadOptions xlsxOptions = new LoadOptions(LoadFormat.Xlsx);
            Console.WriteLine("\nXLSX LoadFormat: " + xlsxOptions.LoadFormat);

            // Örnek XLSX dosyası oluştur/kaydet
            Workbook newWorkbook = new Workbook();
            newWorkbook.Worksheets[0].Cells["A1"].PutValue("XLSX LoadFormat demo");
            newWorkbook.Save("sample.xlsx");

            // Doğru seçeneklerle XLSX'i yükle
            Workbook xlsxWorkbook = new Workbook("sample.xlsx", xlsxOptions);
            Console.WriteLine("XLSX loaded cell: " + xlsxWorkbook.Worksheets[0].Cells["A1"].Value);

            // Geçici dosyaları temizle
            File.Delete("sample.csv");
            File.Delete("sample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [LoadFormat](../../loadformat/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


