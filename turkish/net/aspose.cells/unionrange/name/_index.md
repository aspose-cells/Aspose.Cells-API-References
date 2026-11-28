---
title: "UnionRange.Name"
second_title: "Aspose.Cells için .NET API Referansı"
description: "UnionRange özelliği. Aralığın adını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/unionrange/name/
---
## UnionRange.Name property

Aralığın adını alır veya ayarlar.

```csharp
public string Name { get; set; }
```

### Açıklamalar

Adlandırılmış aralık desteklenir. Örneğin,

range.Name = "Sheet1!MyRange";

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı veriler ekle
            worksheet.Cells["A1"].Value = "First Range";
            worksheet.Cells["B2"].Value = "Second Range";

            try
            {
                // Aralıklar oluşturun ve bunları bir birleşim aralığına birleştirin
                Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:A1");
                Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("B2:B2");
                UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

                // Name özelliğinin mevcut değerini göster
                Console.WriteLine("Initial Name value: " + unionRange.Name);

                // Birleşim aralığı için yeni bir ad ayarlayın
                unionRange.Name = "MyUnionRange";
                Console.WriteLine("Updated Name value: " + unionRange.Name);

                // Adın tekrar değiştirilebileceğini gösterin
                unionRange.Name = "CustomUnionRange";
                Console.WriteLine("Final Name value: " + unionRange.Name);

                // Çalışma kitabını kaydedin
                workbook.Save("UnionRangeNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


