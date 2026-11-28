---
title: "Worksheet.TextBoxes"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. TextBox koleksiyonunu alır"
type: docs
url: /tr/net/aspose.cells/worksheet/textboxes/
---
## Worksheet.TextBoxes property

[`TextBox`](../../../aspose.cells.drawing/textbox/) koleksiyonunu alır.

```csharp
public TextBoxCollection TextBoxes { get; }
```

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTextBoxesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Çalışma sayfasına bir metin kutusu ekle
            int tID = ws.TextBoxes.Add(1, 1, 500, 1000);
            Aspose.Cells.Drawing.TextBox textBox = ws.TextBoxes[tID];

            // Metni ayarla ve parçalarını biçimlendir
            textBox.Text = "Red text 1. Plain text 1. Red text 2. Plain text 2.";
            textBox.Characters(0, 10).Font.Color = Color.Red;
            textBox.Characters(26, 10).Font.Color = Color.DarkRed;

            // Çalışma kitabını kaydedin
            wb.Save("TextBoxExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextBoxCollection](../../../aspose.cells.drawing/textboxcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


