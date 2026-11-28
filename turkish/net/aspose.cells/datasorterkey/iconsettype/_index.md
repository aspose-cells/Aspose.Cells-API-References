---
title: "DataSorterKey.IconSetType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataSorterKey özelliği. Simge seti türünü temsil eder"
type: docs
url: /tr/net/aspose.cells/datasorterkey/iconsettype/
---
## DataSorterKey.IconSetType property

Simge seti türünü temsil eder.

```csharp
public IconSetType IconSetType { get; }
```

### Açıklamalar

Yalnızca [`Type`](../type/) Icon olduğunda etkili olur.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyIconSetTypeDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı nesnesi oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Simge seti koşullu biçimlendirmeli örnek veri ekle
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Simge seti koşullu biçimlendirmesi ekle
            ConditionalFormattingCollection cfc = worksheet.ConditionalFormattings;
            int index = cfc.Add();
            FormatConditionCollection fcc = cfc[index];
            CellArea area = CellArea.CreateCellArea("A1", "A5");
            fcc.AddArea(area);
            fcc.AddCondition(FormatConditionType.IconSet);
            fcc[0].IconSet.Type = IconSetType.Arrows3;

            // Simge seti türüyle veri sıralayıcı oluştur
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Verileri sırala
            sorter.Sort(worksheet.Cells, area);

            // Sıralayıcı anahtarından simge seti türünü göster
            foreach (DataSorterKey key in sorter.Keys)
            {
                Console.WriteLine($"IconSetType used for sorting: {key.IconSetType}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("IconSetTypeSortingDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [IconSetType](../../iconsettype/)
* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


