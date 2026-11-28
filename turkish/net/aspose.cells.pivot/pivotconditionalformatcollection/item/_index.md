---
title: "PivotConditionalFormatCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotConditionalFormatCollection özelliği. Belirli indeksteki pivot FormatCondition nesnesini alır"
type: docs
url: /tr/net/aspose.cells.pivot/pivotconditionalformatcollection/item/
---
## PivotConditionalFormatCollection indexer

Belirli indeksteki pivot FormatCondition nesnesini alır.

```csharp
public PivotConditionalFormat this[int index] { get; }
```

### Dönüş Değeri

pivot FormatCondition nesnesi.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotConditionalFormatCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri oluştur
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 120;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 85;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 95;

            // Özet tablo oluştur
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Koşullu biçim ekle
            int formatIndex = pivotTable.ConditionalFormats.Add();
            PivotConditionalFormat pfc = pivotTable.ConditionalFormats[formatIndex]; // Using Item property
            pfc.AddCellArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 10, EndColumn = 10 });

            // Biçim koşulu ekleyin
            int conditionIndex = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition condition = pfc.FormatConditions[conditionIndex];
            condition.Formula1 = "90";
            condition.Operator = OperatorType.GreaterOrEqual;
            condition.Style.BackgroundColor = System.Drawing.Color.LightGreen;

            // Pivot tablosunu hesapla ve kaydet
            pivotTable.CalculateData();
            workbook.Save("PivotConditionalFormatExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotConditionalFormat](../../pivotconditionalformat/)
* class [PivotConditionalFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


