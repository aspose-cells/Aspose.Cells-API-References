---
title: "PivotField.ShowCompact"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField özelliği. Aynı sütunda bir sonraki alanın etiketlerini Pivot Tablo görünümünde gösterip göstermeyeceğini belirtir. Yalnızca satır alanları için"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/showcompact/
---
## PivotField.ShowCompact property

Bir sonraki alanın etiketlerini aynı sütunda Pivot Tablo görünümünde gösterip göstermeyeceğini belirtir. Yalnızca satır alanları için.

```csharp
[Obsolete("Use PivotField.ShowInCompactForm instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ShowCompact { get; set; }
```

### Açıklamalar

NOT: Bu yöntem artık eski. Bunun yerine, lütfen PivotField.ShowInCompactForm özelliğini kullanın. Bu yöntem, Kasım 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyShowCompactDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Apple");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("Orange");
            worksheet.Cells["A6"].PutValue("Grape");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(200);
            worksheet.Cells["B5"].PutValue(250);
            worksheet.Cells["B6"].PutValue(300);

            // Özet tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("A7", "A1:B6", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Satır alanı ekleyin ve ShowCompact'ı yapılandırın
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField rowField = pivotTable.RowFields[fieldIndex];
            rowField.ShowInOutlineForm = true;
            rowField.ShowCompact = true;
            
            // Veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Pivot tabloyu hesapla ve yenile
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotFieldShowCompactDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


