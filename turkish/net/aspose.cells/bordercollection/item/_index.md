---
title: "BorderCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "BorderCollection özelliği. Belirtilen indeksteki Border öğesini alır"
type: docs
url: /tr/net/aspose.cells/bordercollection/item/
---
## BorderCollection indexer

Belirtilen indeksteki [`Border`](../../border/) öğesini alır.

```csharp
public Border this[BorderType borderType] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| borderType | Alınacak kenarlık. |

### Dönüş Değeri

Belirtilen indeksteki öğe.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class BorderCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Örnek bir çalışma sayfası oluşturun
            Worksheet worksheet = workbook.Worksheets[0];

            // Örneği anlamlı kılmak için bazı veriler ekleyin
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Hücreyi ve stilini alın
                Cell cell = worksheet.Cells["A1"];
                Style style = cell.GetStyle();

                // Stilden BorderCollection'a erişin
                BorderCollection borders = style.Borders;

                // Item özelliğinin mevcut değerini gösterin (okuma işlemi)
                // Not: Item özelliği yalnızca okunabilir ve bir Border nesnesi döndürür
                // Item özelliği bir BorderType parametresi gerektirir
                Border border = borders[BorderType.LeftBorder];
                Console.WriteLine("Border type: " + border.LineStyle);
                Console.WriteLine("Border color: " + border.Color);

                // Sonucu kaydet
                workbook.Save("ItemDemo.xlsx");
                Console.WriteLine("Item property has been demonstrated");
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

* class [Border](../../border/)
* enum [BorderType](../../bordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


