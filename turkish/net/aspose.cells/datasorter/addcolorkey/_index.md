---
title: "DataSorter.AddColorKey"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataSorter yöntemi. Renk sıralama anahtarı ekler"
type: docs
url: /tr/net/aspose.cells/datasorter/addcolorkey/
---
## DataSorter.AddColorKey method

Renk sıralama anahtarı ekler.

```csharp
public void AddColorKey(int key, SortOnType type, SortOrder order, Color color)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| anahtar | Int32 | Sıralanmış sütun indeksi (mutlak konum, A sütunu 0, B 1, ...) |
| type | SortOnType | Sıralanmış renk değeri türü. |
| sıralama | SortOrder | Sıralama düzeni. |
| color | Color | Özel sıralama rengi. |

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodAddColorKeyWithInt32SortOnTypeSortOrderColorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Renkli hücrelerle örnek veri ekle
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue(5);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["A4"].PutValue(7);
            
            // Hücrelere renk uygulayın
            Style styleRed = workbook.CreateStyle();
            styleRed.ForegroundColor = Color.Red;
            styleRed.Pattern = BackgroundType.Solid;
            worksheet.Cells["A2"].SetStyle(styleRed);
            
            Style styleBlue = workbook.CreateStyle();
            styleBlue.ForegroundColor = Color.Blue;
            styleBlue.Pattern = BackgroundType.Solid;
            worksheet.Cells["A3"].SetStyle(styleBlue);
            
            Style styleGreen = workbook.CreateStyle();
            styleGreen.ForegroundColor = Color.Green;
            styleGreen.Pattern = BackgroundType.Solid;
            worksheet.Cells["A4"].SetStyle(styleGreen);

            // Veri sıralayıcı oluştur ve renk anahtarını ekle
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true;
            sorter.AddColorKey(0, SortOnType.CellColor, SortOrder.Ascending, Color.Red);

            // Verileri sırala
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "A4"));

            // Sıralanmış değerleri çıktıla (gösterim için)
            Console.WriteLine("Sorted values:");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + (i + 1)].IntValue);
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [SortOnType](../../sortontype/)
* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


