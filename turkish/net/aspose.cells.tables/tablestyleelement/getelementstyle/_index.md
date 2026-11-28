---
title: "TableStyleElement.GetElementStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TableStyleElement yöntemi. Öğenin stilini alır"
type: docs
url: /tr/net/aspose.cells.tables/tablestyleelement/getelementstyle/
---
## TableStyleElement.GetElementStyle method

Öğe stilini alır.

```csharp
public Style GetElementStyle()
```

### Dönüş Değeri

[`Style`](../../../aspose.cells/style/) nesnesini döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleElementMethodGetElementStyleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);
            
            // Bir tablo oluştur
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            
            // Çalışma kitabının tablo stil koleksiyonundan tablo stilini al
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            TableStyle style = tableStyles[0];
            table.TableStyleName = style.Name;
            
            // Tüm tablo stil öğesine eriş
            TableStyleElement element = style.TableStyleElements[TableStyleElementType.WholeTable];
            
            // Öğenin stilini al
            Style tableStyle = element.GetElementStyle();
            
            // Stil özelliklerini değiştir
            tableStyle.Font.Name = "Arial";
            tableStyle.Font.Size = 12;
            tableStyle.Font.IsBold = true;
            tableStyle.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            tableStyle.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            tableStyle.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            tableStyle.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            
            // Değiştirilen stili geri ayarla
            element.SetElementStyle(tableStyle);
            
            // Çalışma kitabını kaydedin
            workbook.Save("TableStyleElementDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../../aspose.cells/style/)
* class [TableStyleElement](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


