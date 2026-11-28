---
title: "Cells.ApplyRowStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Tüm bir satır için biçimlendirmeleri uygular"
type: docs
url: /tr/net/aspose.cells/cells/applyrowstyle/
---
## Cells.ApplyRowStyle method

Tüm satır için biçimleri uygular.

```csharp
public void ApplyRowStyle(int row, Style style, StyleFlag flag)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Satır indeksi. |
| stil | Stil | Uygulanacak stil nesnesi. |
| bayrak | StyleFlag | Uygulanan biçimlendirme özelliklerini gösteren bayraklar. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodApplyRowStyleWithInt32StyleStyleFlagDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Kenarlıklı bir stil oluştur
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

            // Kenarlıklar için stil bayrağı oluşturun
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Borders = true;

            // Stili ilk satıra uygulayın
            cells.ApplyRowStyle(0, style, styleFlag);

            // Çalışma kitabını kaydedin
            workbook.Save("ApplyRowStyleDemo.xlsx");
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


