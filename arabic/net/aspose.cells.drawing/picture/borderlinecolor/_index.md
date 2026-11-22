---
title: "Picture.BorderLineColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Picture. تمثل لون خط حدود الصورة"
type: docs
url: /ar/net/aspose.cells.drawing/picture/borderlinecolor/
---
## Picture.BorderLineColor property

يمثل لون خط الحدود للصورة.

```csharp
public Color BorderLineColor { get; set; }
```

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyBorderLineColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Picture pic = worksheet.Pictures[imgIndex];
            
            pic.BorderLineColor = Color.Red;
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


