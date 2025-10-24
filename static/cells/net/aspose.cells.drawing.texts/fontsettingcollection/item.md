##FontSettingCollection.Item
FontSettingCollection property. Gets the FontSetting by the index
## FontSettingCollection indexer
Gets the [`FontSetting`](../../../aspose.cells/fontsetting/) by the index.
```csharp
public FontSetting this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The index. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class FontSettingCollectionPropertyItemDemo
{
public static void Run()
{
Workbook w = new Workbook();
Worksheet s = w.Worksheets[0];
Shape tb = s.Shapes.AddTextBox(3, 0, 7, 0, 70, 300);
tb.Text = "Sample Text";
// Set font properties for specific characters
Aspose.Cells.Font fo = tb.Characters(3, 5).Font;
fo.IsSuperscript = true;
fo.Color = Color.Red;
// Access font through TextBody.Item property
Aspose.Cells.Font fo1 = tb.TextBody[3].Font;
Console.WriteLine("IsSuperscript: " + fo1.IsSuperscript);
Console.WriteLine("Color: " + fo1.Color);
w.Save("output.xlsx");
}
}
}
```
### See Also
* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
