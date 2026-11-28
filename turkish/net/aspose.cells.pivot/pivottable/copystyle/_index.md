---
title: "PivotTable.CopyStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable yöntemi. Başka bir pivot tablodan adlandırılmış stili kopyalar"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/copystyle/
---
## PivotTable.CopyStyle method

Başka bir pivot tablodan adlandırılmış stili kopyalar.

```csharp
public void CopyStyle(PivotTable pivotTable)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivotTable | PivotTable | Kaynak pivot tablo. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCopyStyleWithPivotTableDemo
    {
        public static void Run()
        {
            // Pivot tablo içeren kaynak çalışma kitabını oluştur
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            sourceSheet.Cells["A1"].PutValue("Product");
            sourceSheet.Cells["B1"].PutValue("Sales");
            sourceSheet.Cells["A2"].PutValue("A");
            sourceSheet.Cells["B2"].PutValue(100);
            sourceSheet.Cells["A3"].PutValue("B");
            sourceSheet.Cells["B3"].PutValue(200);
            
            // Kaynak pivot tablo oluştur (pivot tablo nesnesini açıkça al)
            PivotTable sourcePivotTable = sourceSheet.PivotTables[sourceSheet.PivotTables.Add("PivotTable1", "A1:B3", "C3")];
            sourcePivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            sourcePivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Kaynak pivot tabloya stil uygula
            sourcePivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            
            // Pivot tablo içeren hedef çalışma kitabını oluştur
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Aynı veri yapısını ekle
            destSheet.Cells["A1"].PutValue("Product");
            destSheet.Cells["B1"].PutValue("Sales");
            destSheet.Cells["A2"].PutValue("A");
            destSheet.Cells["B2"].PutValue(150);
            destSheet.Cells["A3"].PutValue("B");
            destSheet.Cells["B3"].PutValue(250);
            
            // Hedef pivot tablo oluştur (pivot tablo nesnesini açıkça al)
            PivotTable destPivotTable = destSheet.PivotTables[destSheet.PivotTables.Add("PivotTable2", "A1:B3", "C3")];
            destPivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            destPivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Stili kaynak pivot tablodan hedef pivot tabloya kopyala
            destPivotTable.CopyStyle(sourcePivotTable);
            
            // Sonucu kaydet
            destWorkbook.Save("PivotTableStyleCopied.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


