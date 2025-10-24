##WebExtensionCollection.AddWebVideoPlayer
WebExtensionCollection method. Add a web video player into exel
## WebExtensionCollection.AddWebVideoPlayer method
Add a web video player into exel.
```csharp
public int AddWebVideoPlayer(string url, bool autoPlay, int startTime, int endTime)
```
| Parameter | Type | Description |
| --- | --- | --- |
| url | String |  |
| autoPlay | Boolean | Indicates whether auto playing the video. |
| startTime | Int32 | The start time in unit of seconds. |
| endTime | Int32 | The end time in unit of seconds. |
### Examples
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
### See Also
* class [WebExtensionCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)
