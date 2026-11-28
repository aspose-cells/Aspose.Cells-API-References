---
title: "TableStyleElement.Size"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TableStyleElement özelliği. Tek bir şerit bandındaki satır veya sütun sayısı. Yalnızca tip firstRowStripe, secondRowStripe, firstColumnStripe veya secondColumnStripe olduğunda uygulanır."
type: docs
url: /tr/net/aspose.cells.tables/tablestyleelement/size/
---
## TableStyleElement.Size property

Tek bir şerit bandındaki satır veya sütun sayısı. Yalnızca tip firstRowStripe, secondRowStripe, firstColumnStripe veya secondColumnStripe olduğunda uygulanır.

```csharp
public int Size { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleElementPropertySizeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir tablo oluşturmak için örnek veri ekle
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Bir tablo oluştur
            int tableIndex = worksheet.ListObjects.Add(0, 0, 9, 4, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.TableStyleType = TableStyleType.TableStyleMedium9;

            // Çalışma kitabının stil koleksiyonunu kullanarak bir tablo stili oluştur
            TableStyleCollection styleCollection = workbook.Worksheets.TableStyles;
            int styleIndex = styleCollection.AddTableStyle("CustomStyle");
            TableStyle style = styleCollection[styleIndex];
            table.TableStyleName = style.Name;

            // Size özelliğini göstermek için şerit öğeleri ekle
            style.TableStyleElements.Add(TableStyleElementType.FirstRowStripe);
            style.TableStyleElements.Add(TableStyleElementType.SecondRowStripe);

            // Şerit öğelerine eriş
            TableStyleElement firstStripe = style.TableStyleElements[TableStyleElementType.FirstRowStripe];
            TableStyleElement secondStripe = style.TableStyleElements[TableStyleElementType.SecondRowStripe];

            // Mevcut Size değerlerini göster
            Console.WriteLine("Initial First Stripe Size: " + firstStripe.Size);
            Console.WriteLine("Initial Second Stripe Size: " + secondStripe.Size);

            // Şerit boyutlarını değiştir
            firstStripe.Size = 2;
            secondStripe.Size = 3;

            // Değiştirilmiş değerleri göster
            Console.WriteLine("Modified First Stripe Size: " + firstStripe.Size);
            Console.WriteLine("Modified Second Stripe Size: " + secondStripe.Size);

            // Etkileri görmek için çalışma kitabını kaydedin
            workbook.Save("TableStyleElementSizeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TableStyleElement](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


