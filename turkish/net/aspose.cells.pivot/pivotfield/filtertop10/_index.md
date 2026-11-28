---
title: "PivotField.FilterTop10"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField yöntemi. Veri pivot alanının değerlerine göre filtreler"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/filtertop10/
---
## PivotField.FilterTop10 method

Veri pivot alanının değerlerine göre filtreler.

```csharp
public PivotFilter FilterTop10(int valueFieldIndex, PivotFilterType type, bool isTop, int itemCount)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| valueFieldIndex | Int32 | Veri bölgesindeki veri alanının indeksi. |
| type | PivotFilterType | Veri filtreleme türü. Sadece Sayım, Toplam ve Yüzde olabilir. |
| isTop | Boolean | Filtrenin üstten mi yoksa alttan mı uygulanacağını gösterir |
| itemCount | Int32 | Öğe sayısı |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodFilterTop10WithInt32PivotFilterTypeBooleanIntDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["A6"].Value = "Orange";
            worksheet.Cells["A7"].Value = "Banana";
            worksheet.Cells["A8"].Value = "Apple";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["B4"].Value = 30;
            worksheet.Cells["B5"].Value = 40;
            worksheet.Cells["B6"].Value = 50;
            worksheet.Cells["B7"].Value = 60;
            worksheet.Cells["B8"].Value = 70;

            // Özet tablo oluştur
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B8", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Satır alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Üst 10 filtresini uygula
            pivotTable.BaseFields[0].FilterTop10(0, PivotFilterType.Count, false, 2);
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableFilterTop10.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


