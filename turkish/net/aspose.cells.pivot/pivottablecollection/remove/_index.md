---
title: "PivotTableCollection.Remove"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTableCollection yöntemi. Belirtilen PivotTable'ı ve PivotTable verilerini siler"
type: docs
url: /tr/net/aspose.cells.pivot/pivottablecollection/remove/
---
## Remove(PivotTable) {#remove}

Belirtilen PivotTable'ı ve PivotTable verilerini siler

```csharp
public void Remove(PivotTable pivotTable)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivotTable | PivotTable | PivotTable nesnesi |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodRemoveWithPivotTableDemo
    {
        public static void Run()
        {
            // Kaynak Excel dosyasından bir çalışma kitabı oluştur
            Workbook workbook = new Workbook("PivotTableExample.xlsx");
            
            // İlk çalışma sayfasına eriş
            Worksheet sheet = workbook.Worksheets[0];
            
            // Pivot tablo koleksiyonunu al
            PivotTableCollection pivotTables = sheet.PivotTables;
            
            // Herhangi bir özet tablo olup olmadığını kontrol et
            if (pivotTables.Count > 0)
            {
                // İlk özet tabloyu al
                PivotTable pivotTable = pivotTables[0];
                
                // Pivot tabloyu kaldır
                pivotTables.Remove(pivotTable);
                
                Console.WriteLine("Pivot table removed successfully. Count: " + pivotTables.Count);
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableRemoved.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Remove(PivotTable, bool) {#remove_1}

Belirtilen PivotTable'ı siler

```csharp
public void Remove(PivotTable pivotTable, bool keepData)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivotTable | PivotTable | PivotTable nesnesi |
| keepData | Boolean | PivotTable verilerini tutup tutmayacağı |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodRemoveWithPivotTableBooleanDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Bir pivot tablo ekle
            int index = worksheet.PivotTables.Add("A1:B4", "D5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // PivotTable ve boolean parametrelerle Remove yöntemini göster
            Console.WriteLine("Before removal - Cell D5 value: " + worksheet.Cells["D5"].StringValue);
            
            // Pivot tabloyu kaldır ancak verileri tut (true)
            worksheet.PivotTables.Remove(pivotTable, true);
            Console.WriteLine("After removal (keep data) - Cell D5 value: " + worksheet.Cells["D5"].StringValue);

            // Başka bir pivot tablo ekle
            index = worksheet.PivotTables.Add("A1:B4", "D10", "PivotTable2");
            pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            Console.WriteLine("\nBefore removal - Cell D10 value: " + worksheet.Cells["D10"].StringValue);
            
            // Pivot tabloyu kaldır ve verileri temizle (false)
            worksheet.PivotTables.Remove(pivotTable, false);
            Console.WriteLine("After removal (clear data) - Cell D10 value: " + worksheet.Cells["D10"].StringValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


