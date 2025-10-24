##PdfBookmarkEntry.IsCollapse
PdfBookmarkEntry property. When this property is true the bookmarkentry will collapse otherwise it will expand
## PdfBookmarkEntry.IsCollapse property
When this property is true, the bookmarkentry will collapse, otherwise it will expand.
```csharp
public bool IsCollapse { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class PdfBookmarkEntryPropertyIsCollapseDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
PdfSaveOptions saveOptions = new PdfSaveOptions();
// Create root bookmark entry
PdfBookmarkEntry rootEntry = new PdfBookmarkEntry();
rootEntry.Text = "Annual Report";
// Create collapsed financial section
PdfBookmarkEntry financialSection = new PdfBookmarkEntry();
financialSection.Text = "Financial Data";
Console.WriteLine("Financial section IsCollapse initial value: " + financialSection.IsCollapse); // Default: False
financialSection.IsCollapse = true; // Collapse this section by default
Console.WriteLine("Financial section IsCollapse after modification: " + financialSection.IsCollapse); // Now: True
// Add quarterly subsections to financial section
financialSection.SubEntry = new System.Collections.ArrayList();
for (int i = 1; i <= 4; i++)
{
PdfBookmarkEntry quarter = new PdfBookmarkEntry();
quarter.Text = $"Q{i} 2023";
financialSection.SubEntry.Add(quarter);
}
// Create expanded operational section
PdfBookmarkEntry opsSection = new PdfBookmarkEntry();
opsSection.Text = "Operations";
opsSection.IsCollapse = false; // Explicitly expanded
// Build bookmark hierarchy
rootEntry.SubEntry = new System.Collections.ArrayList();
rootEntry.SubEntry.Add(financialSection);
rootEntry.SubEntry.Add(opsSection);
// Assign bookmarks to save options
saveOptions.Bookmark = rootEntry;
// Save with configured bookmarks
workbook.Save("CollapsibleBookmarks.pdf", saveOptions);
}
}
}
```
### See Also
* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
