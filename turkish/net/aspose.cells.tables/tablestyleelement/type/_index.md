---
title: "TableStyleElement.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TableStyleElement özelliği. Öğenin tipini alır"
type: docs
url: /tr/net/aspose.cells.tables/tablestyleelement/type/
---
## TableStyleElement.Type property

Öğe tipini alır.

```csharp
public TableStyleElementType Type { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleElementPropertyTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir tablo oluşturmak için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Bir tablo oluştur
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.TableStyleType = TableStyleType.TableStyleMedium9;

            // Tablo stilini al (yeni bir tane oluşturmak yerine stil adını kullanarak)
            string styleName = table.TableStyleName;
            TableStyle style = workbook.Worksheets.TableStyles[styleName];

            // Tablo stil öğelerine eriş
            TableStyleElement element = style.TableStyleElements[TableStyleElementType.HeaderRow];

            // Öğenin mevcut tipini göster
            Console.WriteLine("Current Type value: " + element.Type);

            // Not: Type özelliği yalnızca okunabilir, bu yüzden ayarlayamazız
            // element.Type = TableStyleElementType.TotalRow; // Bu bir derleme hatasına neden olur

            // Farklı öğe tiplerinin tabloyu nasıl etkilediğini göster
            Console.WriteLine("\nAvailable table style elements:");
            foreach (TableStyleElementType type in Enum.GetValues(typeof(TableStyleElementType)))
            {
                try
                {
                    TableStyleElement testElement = style.TableStyleElements[type];
                    Console.WriteLine($"Element type {type} exists in this style");
                }
                catch
                {
                    Console.WriteLine($"Element type {type} not available in this style");
                }
            }

            // Çalışma kitabını kaydedin
            workbook.Save("TableStyleElementTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [TableStyleElementType](../../tablestyleelementtype/)
* class [TableStyleElement](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


