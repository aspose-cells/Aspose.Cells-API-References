---
title: "Sınıf TableStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Tables.TableStyle sınıfı. Tablo stilini temsil eder"
type: docs
url: /tr/net/aspose.cells.tables/tablestyle/
---
## TableStyle class

Tablonun stilini temsil eder.

```csharp
public class TableStyle
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Name](../../aspose.cells.tables/tablestyle/name/) { get; } | Tablo stilinin adını alır. |
| [TableStyleElements](../../aspose.cells.tables/tablestyle/tablestyleelements/) { get; } | Tablo stilinin tüm öğelerini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| static [Create](../../aspose.cells.tables/tablestyle/create/)(string, WorksheetCollection) | Boş bir tablo/pivot tablo stili oluşturur. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleDemo
    {
        public static void TableStyleExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk ve son sütunlar için stiller oluştur
            Style firstColumnStyle = workbook.CreateStyle();
            firstColumnStyle.Pattern = BackgroundType.Solid;
            firstColumnStyle.BackgroundColor = System.Drawing.Color.Red;

            Style lastColumnStyle = workbook.CreateStyle();
            lastColumnStyle.Font.IsBold = true;
            lastColumnStyle.Pattern = BackgroundType.Solid;
            lastColumnStyle.BackgroundColor = System.Drawing.Color.Red;

            // Özel bir tablo stili adı tanımla
            string tableStyleName = "Custom1";

            // Tablo stilleri koleksiyonuna eriş
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

            // Koleksiyona yeni bir tablo stili ekle
            int index1 = tableStyles.AddTableStyle(tableStyleName);
            TableStyle tableStyle = tableStyles[index1];

            // Tablo stili öğeleri koleksiyonuna eriş
            TableStyleElementCollection elements = tableStyle.TableStyleElements;

            // İlk sütun için stil ekle ve ayarla
            index1 = elements.Add(TableStyleElementType.FirstColumn);
            TableStyleElement element = elements[index1];
            element.SetElementStyle(firstColumnStyle);

            // Son sütun için stil ekle ve ayarla
            index1 = elements.Add(TableStyleElementType.LastColumn);
            element = elements[index1];
            element.SetElementStyle(lastColumnStyle);

            // İlk çalışma sayfasının hücrelerine eriş
            Cells cells = workbook.Worksheets[0].Cells;

            // İlk satırı sütun adlarıyla doldur
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }

            // Kalan hücreleri örnek veriyle doldur
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Çalışma sayfasına bir tablo ekle
            ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Özel tablo stilini tabloya uygula
            table.ShowTableStyleFirstColumn = true;
            table.ShowTableStyleLastColumn = true;
            table.TableStyleName = tableStyleName;

            // Çalışma kitabını kaydedin
            workbook.Save("TableStyleExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


