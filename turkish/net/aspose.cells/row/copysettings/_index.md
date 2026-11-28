---
title: "Row.CopySettings"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Satır yöntemi. Stil, yükseklik, görünürlük vb. gibi satır ayarlarını kopyalar"
type: docs
url: /tr/net/aspose.cells/row/copysettings/
---
## Row.CopySettings method

Satırın ayarlarını kopyalar, örneğin stil, yükseklik, görünürlük, ... vb.

```csharp
public void CopySettings(Row source, bool checkStyle)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| kaynak | Row | ayarları bu satıra kopyalanacak kaynak satır |
| checkStyle | Boolean | stil kontrolü ve toplama yapılıp yapılmayacağını belirler. Yalnızca iki satır nesnesi farklı çalışma kitaplarına ait olduğunda ve iki çalışma kitabının stilleri farklı olduğunda etkili olur ve gerekir. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RowMethodCopySettingsWithRowBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Kaynak satırı oluştur ve stil ver
            Row sourceRow = worksheet.Cells.Rows[0];
            Style sourceStyle = workbook.CreateStyle();
            sourceStyle.BackgroundColor = Color.Blue;
            sourceRow.ApplyStyle(sourceStyle, new StyleFlag { All = true });
            sourceRow.Height = 25;
            sourceRow.IsHidden = false;

            // Hedef satırı oluştur
            Row targetRow = worksheet.Cells.Rows[1];
            
            // copyStyle=true ile CopySettings'i göster
            targetRow.CopySettings(sourceRow, true);

            // Ayarların kopyalandığını doğrula
            Console.WriteLine($"Target row height: {targetRow.Height}");
            Console.WriteLine($"Target row is hidden: {targetRow.IsHidden}");

            workbook.Save("RowCopySettingsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


