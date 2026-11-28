---
title: "Sınıf ListColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Tables.ListColumn sınıfı. Bir tabloda sütunu temsil eder"
type: docs
url: /tr/net/aspose.cells.tables/listcolumn/
---
## ListColumn class

Bir Tablo'daki sütunu temsil eder.

```csharp
public class ListColumn
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Formula](../../aspose.cells.tables/listcolumn/formula/) { get; set; } | Liste sütununun formülünü alır ve ayarlar. |
| [IsArrayFormula](../../aspose.cells.tables/listcolumn/isarrayformula/) { get; } | Formülün dizi formülü olup olmadığını gösterir. |
| [Name](../../aspose.cells.tables/listcolumn/name/) { get; set; } | Sütunun adını alır ve ayarlar. |
| [Range](../../aspose.cells.tables/listcolumn/range/) { get; } | Bu liste sütununun aralığını alır. |
| [TotalsCalculation](../../aspose.cells.tables/listcolumn/totalscalculation/) { get; set; } | Liste sütununun Toplamlar satırındaki hesaplama tipini alır ve ayarlar. |
| [TotalsRowLabel](../../aspose.cells.tables/listcolumn/totalsrowlabel/) { get; set; } | Toplam satırının görüntüleme etiketlerini alır ve ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetCustomCalculatedFormula](../../aspose.cells.tables/listcolumn/getcustomcalculatedformula/)(bool, bool) | Bu liste sütununun formülünü alır. |
| [GetCustomTotalsRowFormula](../../aspose.cells.tables/listcolumn/getcustomtotalsrowformula/)(bool, bool) | Bu liste sütununun toplam satırının formülünü alır. |
| [GetDataStyle](../../aspose.cells.tables/listcolumn/getdatastyle/)() | Tablodaki bu sütundaki verinin stilini alır. |
| [SetCustomCalculatedFormula](../../aspose.cells.tables/listcolumn/setcustomcalculatedformula/)(string, bool, bool) | Bu liste sütunu için formülü ayarlar. |
| [SetCustomTotalsRowFormula](../../aspose.cells.tables/listcolumn/setcustomtotalsrowformula/)(string, bool, bool) | Bu liste sütununun toplam satırının formülünü alır. |
| [SetDataStyle](../../aspose.cells.tables/listcolumn/setdatastyle/)(Style) | Tablodaki bu sütundaki verinin stilini ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListColumnDemo
    {
        public static void ListColumnExample()
        {
            // Yeni bir çalışma kitabı oluştur ve ilk çalışma sayfasına eriş.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Çalışma sayfasını bazı verilerle doldurun
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 4; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Çalışma sayfasına bir ListObject (tablo) ekle
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];
            table.ShowTotals = true;

            // ListColumn'a eriş ve özelliklerini ayarla
            ListColumn listColumn = table.ListColumns[4];
            listColumn.TotalsCalculation = TotalsCalculation.Sum;
            listColumn.Formula = "=[A]";
            listColumn.Name = "CustomColumn";
            listColumn.TotalsRowLabel = "Total";

            // Çalışma kitabını kaydedin
            workbook.Save("ListColumnExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


