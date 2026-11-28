---
title: "DataSorterKey.IconId"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataSorterKey özelliği. Simge seti türünün kimliğini temsil eder"
type: docs
url: /tr/net/aspose.cells/datasorterkey/iconid/
---
## DataSorterKey.IconId property

Simge seti türünün kimliğini temsil eder.

```csharp
public int IconId { get; }
```

### Açıklamalar

Yalnızca [`Type`](../type/) Icon olduğunda etkili olur.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataSorterKeyPropertyIconIdDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Simge setleri kullanabilecek değerlerle örnek veri ekle
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

            // Veri sıralayıcı oluştur ve anahtar ekle
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Verileri sırala
            sorter.Sort(worksheet.Cells, area);

            try
            {
                // Sıralayıcı anahtarlardan IconId özelliğini göster
                foreach (DataSorterKey key in sorter.Keys)
                {
                    Console.WriteLine($"IconId: {key.IconId}");
                    Console.WriteLine($"IconSetType: {key.IconSetType}");
                }

                // Çalışma kitabını kaydedin
                workbook.Save("IconIdDemo.xlsx");
                Console.WriteLine("IconId demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


