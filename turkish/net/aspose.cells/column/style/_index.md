---
title: "Column.Style"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Column özelliği. Bu sütunun stilini alır"
type: docs
url: /tr/net/aspose.cells/column/style/
---
## Column.Style property

Bu sütunun stilini alır.

```csharp
[Obsolete("Use Column.GetStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Style Style { get; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine, bu sütunun varsayılan stilini almak için lütfen Column.GetStyle() yöntemini kullanın. Bu özellik, Aralık 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnPropertyStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // İlk sütuna eriş
            Column column = worksheet.Cells.Columns[0];
            
            // Style özelliğini kullanarak mevcut stili al
            Style originalStyle = column.Style;
            Console.WriteLine("Original column style - Background: " + originalStyle.BackgroundColor);
            
            // Yeni bir stil oluştur ve özellikleri değiştir
            Style newStyle = workbook.CreateStyle();
            newStyle.BackgroundColor = Color.LightBlue;
            newStyle.Font.IsBold = true;
            newStyle.HorizontalAlignment = TextAlignmentType.Center;
            
            // Yeni stili sütuna uygula
            column.SetStyle(newStyle);
            
            // Stil uygulamasını göstermek için veri ekle
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue("Data 2");
            
            // Stil değişikliklerini doğrula
            Console.WriteLine("New column style applied - Background: " + column.GetStyle().BackgroundColor);
            
            // Sütun genişliği ayarıyla kaydet
            column.Width = 15;
            workbook.Save("ColumnStyleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


