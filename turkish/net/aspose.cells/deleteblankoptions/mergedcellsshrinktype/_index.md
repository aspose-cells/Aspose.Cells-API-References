---
title: "DeleteBlankOptions.MergedCellsShrinkType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DeleteBlankOptions özelliği. Boş satır/sütunları silerken birleştirilmiş hücrelerin nasıl işleneceğini gösterir"
type: docs
url: /tr/net/aspose.cells/deleteblankoptions/mergedcellsshrinktype/
---
## DeleteBlankOptions.MergedCellsShrinkType property

Boş satırları/sütunları silerken birleştirilmiş hücrelerin nasıl işleneceğini gösterir.

```csharp
public MergedCellsShrinkType MergedCellsShrinkType { get; set; }
```

### Açıklamalar

KeepHeaderOnly için, içindeki tüm hücreler boş kabul edilir, yalnızca boş olmayan sol‑üst hücre hariçtir. Bu, özelliğin varsayılan değeridir. None için, içindeki tüm hücreler boş olmayan olarak kabul edilir. ShrinkToFit için, içerik görüntüleme alanının dışındaki tüm hücreler boş kabul edilir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyMergedCellsShrinkTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            Cells cells = ws.Cells;

            // Birleştirilmiş hücrelerle örnek veri ayarla
            cells.Merge(0, 0, 3, 1);
            cells[0, 0].PutValue("Merged Header");
            cells[3, 0].PutValue("Data after blank");
            
            // Farklı sıkıştırma tipleriyle silme seçenekleri oluştur
            DeleteBlankOptions options = new DeleteBlankOptions();
            
            // Durum 1: KeepHeaderOnly
            options.MergedCellsShrinkType = MergedCellsShrinkType.KeepHeaderOnly;
            cells.DeleteBlankRows(options);
            Console.WriteLine("After KeepHeaderOnly - Merged area preserved: " + 
                (cells.MergedCells.Count > 0 ? cells.MergedCells[0].ToString() : "No merged cells"));

            // Çalışma sayfasını sıfırla
            cells.ClearContents(0, 0, cells.MaxDataRow + 1, cells.MaxDataColumn + 1);
            cells.UnMerge(0, 0, 3, 1);
            cells.Merge(0, 0, 3, 1);
            cells[0, 0].PutValue("Merged Header");
            cells[3, 0].PutValue("Data after blank");

            // Durum 2: ShrinkToFit
            options.MergedCellsShrinkType = MergedCellsShrinkType.ShrinkToFit;
            cells.DeleteBlankRows(options);
            Console.WriteLine("After ShrinkToFit - Merged area adjusted: " + 
                (cells.MergedCells.Count > 0 ? cells.MergedCells[0].ToString() : "No merged cells"));

            // Çalışma sayfasını sıfırla
            cells.ClearContents(0, 0, cells.MaxDataRow + 1, cells.MaxDataColumn + 1);
            cells.UnMerge(0, 0, 3, 1);
            cells.Merge(0, 0, 3, 1);
            cells[0, 0].PutValue("Merged Header");
            cells[3, 0].PutValue("Data after blank");

            // Durum 3: None
            options.MergedCellsShrinkType = MergedCellsShrinkType.None;
            cells.DeleteBlankRows(options);
            Console.WriteLine("After None - Merged area unchanged: " + 
                (cells.MergedCells.Count > 0 ? cells.MergedCells[0].ToString() : "No merged cells"));
        }
    }
}
```

### Ayrıca Bakınız

* enum [MergedCellsShrinkType](../../mergedcellsshrinktype/)
* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


