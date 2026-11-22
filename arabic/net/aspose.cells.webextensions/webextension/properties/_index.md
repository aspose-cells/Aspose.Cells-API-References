---
title: "WebExtension.Properties"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebExtension. تحصل على جميع خصائص امتداد الويب"
type: docs
url: /ar/net/aspose.cells.webextensions/webextension/properties/
---
## WebExtension.Properties property

يحصل على جميع خصائص الامتداد الويب.

```csharp
public WebExtensionPropertyCollection Properties { get; }
```

### أمثلة

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionPropertyPropertiesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            int extIndex = workbook.Worksheets.WebExtensions.Add();
            WebExtension webExt = workbook.Worksheets.WebExtensions[extIndex];

            webExt.Reference.Id = "wa104104476";
            webExt.Reference.Version = "1.3.0.0";
            webExt.Reference.StoreName = "en-US";
            webExt.Reference.StoreType = WebExtensionStoreType.OMEX;

            webExt.Properties.Add("theme", "\"giant-redwhiteblack\"");
            webExt.Properties.Add("sku", "\"peoplebar-giant\"");

            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 0, 0, 500, 500);
            WebExtensionShape webShape = (WebExtensionShape)shapes[0];
            webShape.WebExtension = webExt;

            workbook.Save("WebExtensionPropertyPropertiesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WebExtensionPropertyCollection](../../webextensionpropertycollection/)
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


