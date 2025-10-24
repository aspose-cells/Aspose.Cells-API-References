##RevisionFormat.Areas
RevisionFormat property. The range to which this formatting was applied
## RevisionFormat.Areas property
The range to which this formatting was applied.
```csharp
public CellArea[] Areas { get; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Revisions;
namespace AsposeCellsExamples
{
public class RevisionFormatPropertyAreasDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
workbook.Settings.Shared = true;
Worksheet worksheet = workbook.Worksheets[0];
Style style = workbook.CreateStyle();
style.BackgroundColor = System.Drawing.Color.Yellow;
Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2,C3:D4");
StyleFlag styleFlag = new StyleFlag();
styleFlag.All = true;
range.ApplyStyle(style, styleFlag);
using (MemoryStream ms = new MemoryStream())
{
workbook.Save(ms, SaveFormat.Xlsx);
ms.Position = 0;
Workbook reloadedWorkbook = new Workbook(ms);
foreach (RevisionLog log in reloadedWorkbook.Worksheets.RevisionLogs)
{
foreach (Revision rev in log.Revisions)
{
if (rev.Type == RevisionType.Format)
{
RevisionFormat rfmt = (RevisionFormat)rev;
Console.WriteLine("Worksheet: " + rfmt.Worksheet.Name);
Console.WriteLine("Number of areas: " + rfmt.Areas.Length);
for (int i = 0; i < rfmt.Areas.Length; i++)
{
CellArea area = rfmt.Areas[i];
Console.WriteLine($"Area {i}: StartRow={area.StartRow}, StartColumn={area.StartColumn}, EndRow={area.EndRow}, EndColumn={area.EndColumn}");
}
}
}
}
}
}
}
}
```
### See Also
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [RevisionFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
