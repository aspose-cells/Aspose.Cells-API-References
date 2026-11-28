---
title: "UnionRange.RefersTo"
second_title: "Aspose.Cells için .NET API Referansı"
description: "UnionRange özelliği. Başvurduğu aralıkları alır"
type: docs
url: /tr/net/aspose.cells/unionrange/refersto/
---
## UnionRange.RefersTo property

Aralığın referansını alır.

```csharp
public string RefersTo { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyRefersToDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bazı verileri doldurun
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(800);

            // Adlandırılmış bir aralık oluştur
            Aspose.Cells.Range namedRange = worksheet.Cells.CreateRange("B2:B3");
            namedRange.Name = "ProductPrices";

            // Adlandırılmış aralığımızı içeren bir birleşik aralık oluştur
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B3").UnionRanges(new Aspose.Cells.Range[] { namedRange });

            // Birleşik aralığın RefersTo özelliğini göster
            Console.WriteLine("UnionRange RefersTo: " + unionRange.RefersTo);

            // Başka bir aralık oluştur ve onun RefersTo özelliğini göster
            Aspose.Cells.Range singleRange = worksheet.Cells.CreateRange("C1:D3");
            Console.WriteLine("Single Range RefersTo: " + singleRange.RefersTo);

            // RefersTo kullanarak aralık bileşimini tanımlamayı göster
            Console.WriteLine("Does union range contain named range? " + 
                unionRange.RefersTo.Contains("ProductPrices"));

            // Aralıklar değiştirildiğinde RefersTo'un nasıl değiştiğini göster
            Aspose.Cells.Range newRange = worksheet.Cells.CreateRange("A1:C3");
            UnionRange modifiedUnion = newRange.UnionRanges(new Aspose.Cells.Range[] { namedRange });
            Console.WriteLine("Modified UnionRange RefersTo: " + modifiedUnion.RefersTo);

            // Çalışma kitabını kaydedin
            workbook.Save("UnionRangeRefersToDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


