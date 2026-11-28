---
title: "TableStyle.TableStyleElements"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TableStyle özelliği. Tablo stilinin tüm öğelerini alır"
type: docs
url: /tr/net/aspose.cells.tables/tablestyle/tablestyleelements/
---
## TableStyle.TableStyleElements property

Tablo stilinin tüm öğelerini alır.

```csharp
public TableStyleElementCollection TableStyleElements { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStylePropertyTableStyleElementsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Tablo için örnek veri oluştur
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Bir tablo oluştur
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.ShowTableStyleFirstColumn = true;

            // Tablo stilini al (yeni bir stil oluşturmak yerine mevcut stili kullan)
            TableStyle style = workbook.Worksheets.TableStyles[0];

            // Tablo stil öğelerini değiştir
            TableStyleElement wholeTableElement = style.TableStyleElements[TableStyleElementType.WholeTable];
            Style wholeTableStyle = wholeTableElement.GetElementStyle();
            wholeTableStyle.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            wholeTableStyle.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;

            // Değiştirilmiş stili tabloya uygula
            table.TableStyleName = style.Name;

            // Çalışma kitabını kaydedin
            workbook.Save("TableStyleElementsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TableStyleElementCollection](../../tablestyleelementcollection/)
* class [TableStyle](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


