---
title: "Cells.ApplyColumnStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Tüm bir sütun için biçimleri uygular"
type: docs
url: /tr/net/aspose.cells/cells/applycolumnstyle/
---
## Cells.ApplyColumnStyle method

Tüm bir sütun için biçimleri uygular.

```csharp
public void ApplyColumnStyle(int column, Style style, StyleFlag flag)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | Int32 | Sütun indeksi. |
| stil | Stil | Uygulanacak stil nesnesi. |
| bayrak | StyleFlag | Uygulanan biçimlendirme özelliklerini gösteren bayraklar. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodApplyColumnStyleWithInt32StyleStyleFlagDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Kenarlıklı bir stil oluştur
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

            // Yalnızca kenarlıkları uygulamak için bir stil bayrağı oluştur
            StyleFlag sflag = new StyleFlag();
            sflag.Borders = true;

            // Stili sütun 1'e (indeks 0) uygula
            cells.ApplyColumnStyle(0, style, sflag);

            // Çalışma kitabını kaydedin
            workbook.Save("ApplyColumnStyleOutput.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


