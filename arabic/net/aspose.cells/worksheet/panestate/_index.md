---
title: "Worksheet.PaneState"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تشير إلى ما إذا كان الجزء يحتوي على تقسيمات أفقية أو عمودية وما إذا كانت تلك التقسيمات مجمدة"
type: docs
url: /ar/net/aspose.cells/worksheet/panestate/
---
## Worksheet.PaneState property

يشير إلى ما إذا كان اللوح يحتوي على تقسيمات أفقية أو عمودية، وما إذا كانت تلك التقسيمات مجمدة.

```csharp
public PaneStateType PaneState { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyPaneStateDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين بيانات عينة
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");

            // تجميد الأجزاء (الصف الأول)
            worksheet.FreezePanes(1, 0, 1, 0);

            // احصل على حالة اللوحة وعرضها
            PaneStateType paneState = worksheet.PaneState;
            Console.WriteLine("Pane State: " + paneState);

            // احفظ دفتر العمل
            workbook.Save("PaneStateDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PaneStateType](../../panestatetype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


