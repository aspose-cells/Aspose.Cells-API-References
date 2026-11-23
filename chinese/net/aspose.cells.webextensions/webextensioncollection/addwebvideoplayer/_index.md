---
title: "WebExtensionCollection.AddWebVideoPlayer"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "WebExtensionCollection 方法。向 exel 中添加网络视频播放器"
type: docs
url: /zh/net/aspose.cells.webextensions/webextensioncollection/addwebvideoplayer/
---
## WebExtensionCollection.AddWebVideoPlayer method

向 exel 中添加网络视频播放器。

```csharp
public int AddWebVideoPlayer(string url, bool autoPlay, int startTime, int endTime)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| url | String |  |
| autoPlay | 布尔 | 指示视频是否自动播放。 |
| startTime | Int32 | 开始时间，单位为秒。 |
| endTime | Int32 | 结束时间，单位为秒。 |

### 示例

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

### 另请参见

* class [WebExtensionCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


