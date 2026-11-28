---
title: "PivotTableFormatCollection.FormatArea"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTableFormatCollection metodu. Seçili alanı biçimler"
type: docs
url: /tr/net/aspose.cells.pivot/pivottableformatcollection/formatarea/
---
## PivotTableFormatCollection.FormatArea method

Seçili alanı biçimler.

```csharp
public PivotTableFormat FormatArea(PivotFieldType axisType, int fieldPosition, 
    PivotFieldSubtotalType subtotalType, PivotTableSelectionType selectionType, bool isGrandRow, 
    bool isGrandColumn, Style style)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| axisType | PivotFieldType | Bu kuralın uygulandığı PivotTable bölgesi. |
| fieldPosition | Int32 | Bu kuralın uygulandığı eksen içindeki alanın konumu. |
| subtotalType | PivotFieldSubtotalType | Pivot alanının alt toplam filtre türü |
| selectionType | PivotTableSelectionType | Verilerin nasıl seçileceğini gösterir. |
| isGrandRow | Boolean | Genel toplam satırlarını seçip seçmediğini gösterir. |
| isGrandColumn | Boolean | Genel toplam sütunlarını seçip seçmediğini gösterir. |
| stil | Stil | Pivot tablo alanına uygulanan stil. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotTableFormatCollectionMethodFormatAreaWithPivotFieldTypeInt32PivotFieldSDemo
    {
        public static void Run()
        {
            // Kaynak dosyadan bir çalışma kitabı oluştur
            Workbook workbook = new Workbook("example.xlsx");
            
            // Pivot tabloya eriş
            PivotTable pt = workbook.Worksheets["PIVOT_VBA_SUBTOTALS"].PivotTables[0];
            
            // Biçimlendirme için bir stil oluştur
            Style style = workbook.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, Color.Red);
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.LightGray;
            style.BackgroundColor = Color.LightGray;

            // Pivot tablo alanını biçimlendir
            pt.PivotFormats.FormatArea(
                PivotFieldType.Row, 
                0, 
                PivotFieldSubtotalType.Automatic, 
                PivotTableSelectionType.DataAndLabel, 
                false, 
                false, 
                style);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTableFormat](../../pivottableformat/)
* enum [PivotFieldType](../../pivotfieldtype/)
* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* enum [PivotTableSelectionType](../../pivottableselectiontype/)
* class [Style](../../../aspose.cells/style/)
* class [PivotTableFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


