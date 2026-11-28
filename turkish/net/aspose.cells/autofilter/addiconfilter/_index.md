---
title: "AutoFilter.AddIconFilter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AutoFilter yöntemi. Bir simge filtresi ekler"
type: docs
url: /tr/net/aspose.cells/autofilter/addiconfilter/
---
## AutoFilter.AddIconFilter method

Bir simge filtresi ekler.

```csharp
public void AddIconFilter(int fieldIndex, IconSetType iconSetType, int iconId)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldIndex | Int32 | Filtreyi temellendirmek istediğiniz alanın tam sayı ofseti (listenin solundan; en soldaki alan field 0'dır). |
| iconSetType | IconSetType | Simge seti türü. |
| iconId | Int32 | Simge kimliği. |

### Açıklamalar

Yalnızca simge filtresi eklemeyi destekler. Filtre bir simge filtresi ise hangi satırın görünür olduğunu kontrol etmeyi desteklemez.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodAddIconFilterWithInt32IconSetTypeInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A sütununa örnek veri doldurun
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["A6"].PutValue(50);
            cell = worksheet.Cells["B1"];
            cell.PutValue("Values2");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);
            worksheet.Cells["B6"].PutValue(50);

            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            FormatConditionCollection fcs = cfs[cfs.Add()];
            fcs.AddArea(CellArea.CreateCellArea(1, 0, 5, 1));
            FormatCondition fc = fcs[fcs.AddCondition(FormatConditionType.IconSet)];

            // Otomatik filtre örneğini al
            AutoFilter autoFilter = worksheet.AutoFilter;
            
            // autofilter aralığını (A1:A6) startRow, startColumn, endRow kullanarak ayarla
            autoFilter.SetRange(0, 0, 1);

            try
            {
                // İlk sütuna (fieldIndex: 0) simge filtresi ekle
                // 3 Traffic Lights simge seti kullanarak (IconSetType.TrafficLights31)
                // Set içindeki ilk simgeyi filtreleme (iconId: 0)
                autoFilter.AddIconFilter(0, IconSetType.TrafficLights31, 0);
                
                // Değişiklikleri uygulamak için filtreyi yenile
                autoFilter.Refresh();

                Console.WriteLine("Added icon filter to column A showing items with first traffic light icon");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddIconFilter: {ex.Message}");
            }

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("AutoFilterMethodAddIconFilterWithInt32IconSetTypeInt32Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [IconSetType](../../iconsettype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


