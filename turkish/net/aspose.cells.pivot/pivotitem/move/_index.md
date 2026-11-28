---
title: "PivotItem.Move"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotItem yöntemi. Öğeyi yukarı veya aşağı hareket ettirir"
type: docs
url: /tr/net/aspose.cells.pivot/pivotitem/move/
---
## Move(int, bool) {#move_1}

Öğeyi yukarı veya aşağı hareket ettirir

```csharp
[Obsolete("Use PivotTable.MoveItem(PivotFieldType, string[],bool,int) method  or PivotItem.Move(int) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Move(int offset, bool isSameParent)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ofset | Int32 | Yukarı veya aşağı hareket sayısı. Bu değer sıfırdan küçükse öğeyi yukarı, sıfırdan büyükse aşağı hareket ettir. |
| isSameParent | Boolean | Taşıma işleminin aynı üst düğümde olup olmadığını belirler |

### Açıklamalar

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotTable.MoveItem(PivotFieldType, string[],bool,int) veya PivotItem.Move(int) yöntemini kullanın. Bu yöntem Kasım 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemMethodMoveWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Özet tablo için örnek veri oluştur
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["B4"].PutValue(300);

            // Pivot tablo ekle
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Satır alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Pivot öğeleri alın ve Move yöntemini gösterin
            PivotItemCollection items = pivotTable.RowFields[0].PivotItems;
            
            // İlk öğeyi, alt öğelerle birlikte 1. konuma (ikinci konum) taşı
            items[0].Move(1, true);
            
            // Çalışma kitabını kaydedin
            wb.Save("PivotItemMoveDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Move(int) {#move}

Öğeyi pivot alanında yukarı ya da aşağı hareket ettirir

```csharp
public void Move(int offset)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ofset | Int32 | Yukarı veya aşağı hareket sayısı. Bu değer sıfırdan küçükse öğeyi yukarı, sıfırdan büyükse aşağı hareket ettir. |

### Ayrıca Bakınız

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


