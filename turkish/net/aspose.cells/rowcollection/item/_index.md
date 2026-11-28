---
title: "RowCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RowCollection özelliği. Verilen satır indeksine göre bir Row nesnesi alır. Verilen satır indeksine ait Row nesnesi, daha önce mevcut değilse oluşturulur."
type: docs
url: /tr/net/aspose.cells/rowcollection/item/
---
## RowCollection indexer

Verilen satır indeksine göre bir [`Row`](../../row/) nesnesi alır. Verilen satır indeksine ait Row nesnesi, daha önce mevcut değilse oluşturulur.

```csharp
public Row this[int rowIndex] { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Sütunlar için standart genişliği ayarla
            cells.StandardWidth = 20.0;

            // Item özelliğini kullanarak satırları eriş ve biçimlendir
            for (int i = 0; i < 5; i++)
            {
                Row row = cells.Rows[i]; // Using Item property
                Style rowStyle = workbook.CreateStyle();
                rowStyle.Font.IsBold = true;
                rowStyle.Font.Color = System.Drawing.Color.Blue;
                row.ApplyStyle(rowStyle, new StyleFlag { Font = true });
                
                // Satırdaki hücreye eriş ve biçimlendir
                Cell cell = cells[i, i]; // Using Cells indexer instead of row[i]
                cell.PutValue($"Row {i}, Col {i}");
                Style cellStyle = workbook.CreateStyle();
                cellStyle.BackgroundColor = System.Drawing.Color.LightYellow;
                cell.SetStyle(cellStyle);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("RowCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Row](../../row/)
* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


