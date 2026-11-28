---
title: "Cells.PreserveString"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells özelliği. Tüm çalışma sayfası değerlerinin dize olarak korunup korunmayacağını belirten bir değeri alır veya ayarlar. Varsayılan değer false'tur"
type: docs
url: /tr/net/aspose.cells/cells/preservestring/
---
## Cells.PreserveString property

Tüm çalışma sayfası değerlerinin dize olarak korunup korunmayacağını gösteren değeri alır veya ayarlar. Varsayılan false'tur.

```csharp
public bool PreserveString { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyPreserveStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // PreserveString özelliğini true olarak ayarla
            cells.PreserveString = true;

            // Hücrelere dize değerleri ekle
            cells["A1"].PutValue("Preserved String 1");
            cells["B1"].PutValue("Preserved String 2");

            // Değerlere eriş (dizeler olarak korunacaklar)
            Console.WriteLine("Cell A1 value: " + cells["A1"].StringValue);
            Console.WriteLine("Cell B1 value: " + cells["B1"].StringValue);

            // Çalışma kitabını kaydedin
            workbook.Save("PreserveStringDemo.xlsx", SaveFormat.Xlsx);

            // Korumanın doğrulanması için kaydedilmiş çalışma kitabını yükle
            Workbook loadedWorkbook = new Workbook("PreserveStringDemo.xlsx");
            Cells loadedCells = loadedWorkbook.Worksheets[0].Cells;

            // Korunan değerleri çıktı olarak göster
            Console.WriteLine("\nAfter loading:");
            Console.WriteLine("Cell A1 value: " + loadedCells["A1"].StringValue);
            Console.WriteLine("Cell B1 value: " + loadedCells["B1"].StringValue);

            // PreserveString özelliği karşılaştırmasını göster
            Console.WriteLine("\nPreserveString property matches: " + 
                (cells.PreserveString == loadedCells.PreserveString));
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


