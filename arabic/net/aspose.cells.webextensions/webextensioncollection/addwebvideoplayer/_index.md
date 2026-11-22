---
title: "WebExtensionCollection.AddWebVideoPlayer"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة WebExtensionCollection. أضف مشغل فيديو ويب إلى إكسل"
type: docs
url: /ar/net/aspose.cells.webextensions/webextensioncollection/addwebvideoplayer/
---
## WebExtensionCollection.AddWebVideoPlayer method

إضافة مشغل فيديو ويب إلى إكسل.

```csharp
public int AddWebVideoPlayer(string url, bool autoPlay, int startTime, int endTime)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| url | String |  |
| autoPlay | منطقي | يشير إلى ما إذا كان الفيديو يُشغل تلقائيًا. |
| startTime | Int32 | وقت البدء بوحدة الثواني. |
| endTime | Int32 | وقت النهاية بوحدة الثواني. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionCollectionMethodAddWebVideoPlayerWithStringBooleanInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            
            int index = webExtensions.AddWebVideoPlayer(
                "https://www.youtube.com/watch?v=z0hFbzPPfm8", 
                true, 
                0, 
                0);
                
            WebExtension webExt = webExtensions[index];
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 410, 730, 0, 0);
            
            WebExtensionShape wShape = (WebExtensionShape)shapes[0];
            wShape.WebExtension = webExt;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WebExtensionCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


