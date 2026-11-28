---
title: "Cells.InsertCutCells"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Kesilmiş aralığı ekle"
type: docs
url: /tr/net/aspose.cells/cells/insertcutcells/
---
## Cells.InsertCutCells method

Kesilen aralığı ekle.

```csharp
public void InsertCutCells(Range cutRange, int row, int column, ShiftType shiftType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cutRange | Aralık | Kesilen aralık. |
| satır | Int32 | Satır. |
| sütun | Int32 | Sütun. |
| shiftType | ShiftType | Kesilen aralık eklenirken hedef aralıktaki diğer nesnelerin nasıl kaydırılacağını gösterir. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertCutCellsWithRangeInt32Int32ShiftTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına ve hücrelerine erişin.
            Worksheet sourceSheet = workbook.Worksheets[0];
            Cells sourceCells = sourceSheet.Cells;
            
            // Kaynak hücrelere bazı veriler ekleyin
            sourceCells["A1"].PutValue("Source A1");
            sourceCells["B1"].PutValue("Source B1");
            sourceCells["A2"].PutValue("Source A2");
            sourceCells["B2"].PutValue("Source B2");
            
            // Hedef olarak ikinci bir çalışma sayfası oluşturun
            Worksheet destSheet = workbook.Worksheets.Add("Sheet2");
            Cells destCells = destSheet.Cells;
            
            // Hedefe bazı başlangıç verileri ekleyin
            destCells["A1"].PutValue("Dest A1");
            destCells["B1"].PutValue("Dest B1");
            
            // Kesmek için bir aralık oluşturun (kaynak sayfadan A1:B2)
            Aspose.Cells.Range cutRange = sourceCells.CreateRange("A1:B2");
            
            // Kesilen hücreleri hedef sayfada B2 konumuna ekleyin, hücreleri aşağı kaydırarak
            destCells.InsertCutCells(cutRange, 1, 1, ShiftType.Down);
            
            // Çalışma kitabını kaydedin
            workbook.Save("InsertCutCellsDemo.xlsx");
            
            Console.WriteLine("InsertCutCells demo executed successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../../range/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


