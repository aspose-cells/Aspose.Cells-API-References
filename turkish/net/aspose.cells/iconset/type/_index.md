---
title: "IconSet.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "IconSet özelliği. Görüntülenecek simge seti türünü Alın veya Ayarlayın. Tür ayarlandığında, mevcut Cfvoss sayısının yeni türle uyumlu olup olmadığı otomatik olarak kontrol edilir. Uyumsuzsa eski Cfvos temizlenir ve varsayılan Cfvos eklenir."
type: docs
url: /tr/net/aspose.cells/iconset/type/
---
## IconSet.Type property

Görüntülenecek ikon seti türünü alın veya ayarlayın. Tür ayarlandığında, mevcut Cfvos sayısının yeni türle uyumlu olup olmadığı otomatik olarak kontrol edilir. Uyumsuzsa, eski Cfvos temizlenir ve varsayılan Cfvos eklenir.

```csharp
public IconSetType Type { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            int idx = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = fcs[idx];
            IconSet iconSet = cond.IconSet;

            // Type özelliğinin kullanımını gösterin.
            iconSet.Type = IconSetType.Arrows3;

            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            workbook.Save("IconSetExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [IconSetType](../../iconsettype/)
* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


