---
title: "PivotItem.IsFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotItem özelliği. Bu pivot öğesinin hesaplanmış bir formül öğesi olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.pivot/pivotitem/isformula/
---
## PivotItem.IsFormula property

Bu pivot öğesinin hesaplanmış bir formül öğesi olup olmadığını gösterir.

```csharp
[Obsolete("Use PivotItem.IsCalculatedItem property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsFormula { get; set; }
```

### Açıklamalar

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotItem.IsCalculatedItem özelliğini kullanın. Bu özellik Kasım 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemPropertyIsFormulaDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Pivot tablo için örnek veri ekle
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["B4"].Value = 30;

            // Bir pivot tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // İlk pivot öğesini al
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItem pivotItem = pivotField.PivotItems[0];

            // Mevcut IsFormula değerini göster (kullanımdan kaldırılmış özellik)
            Console.WriteLine("Current IsFormula value: " + pivotItem.IsFormula);

            // IsFormula için yeni bir değer ayarla (kullanımdan kaldırılmış özellik)
            pivotItem.IsFormula = true;

            // Etkiyi göster - bu, pivot öğesini bir formül öğesi olarak işaretler
            Console.WriteLine("After setting IsFormula to true: " + pivotItem.IsFormula);

            // Not: Gerçek kullanımda, IsFormula artık kullanılmadığı için yerine IsCalculatedItem kullanmalısınız
            Console.WriteLine("IsCalculatedItem (recommended property): " + pivotItem.IsCalculatedItem);

            // Sonucu kaydet
            workbook.Save("PivotItemPropertyIsFormulaDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


