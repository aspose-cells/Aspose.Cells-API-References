---
title: "Style.IndentLevel"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Hücre veya aralık için girinti seviyesini temsil eder. Yalnızca 0 ile 250 arasında bir tam sayı olabilir."
type: docs
url: /tr/net/aspose.cells/style/indentlevel/
---
## Style.IndentLevel property

Hücre veya aralık için girinti seviyesini temsil eder. Yalnızca 0 ile 250 arasında bir tam sayı olabilir.

```csharp
public int IndentLevel { get; set; }
```

### Açıklamalar

Metin yatay hizalama türü sola veya sağa dışında bir değere ayarlanırsa, girinti seviyesi sıfıra sıfırlanır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIndentLevelDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Hücreler için farklı girinti seviyeleri ayarlayın
            for (int i = 0; i < 16; i++)
            {
                Cell cell = cells[i, 0];
                Style style = cell.GetStyle();
                style.IndentLevel = i;
                style.HorizontalAlignment = TextAlignmentType.Left;
                cell.SetStyle(style);
                cell.PutValue($"Indent Level {i}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("IndentLevelDemo.xlsx");
            Console.WriteLine("Workbook saved with different indent levels.");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


