---
title: HtmlSaveOptions.ExportSingleTab
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates whether exporting the single tab when the file only has one worksheet. The default value is false
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportsingletab/
---
## HtmlSaveOptions.ExportSingleTab property

Indicates whether exporting the single tab when the file only has one worksheet. The default value is false.

```csharp
public bool ExportSingleTab { get; set; }
```

### Examples

```csharp
// Called: ExportSingleTab = true,
[Test]
        public void Property_ExportSingleTab()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;NET47493/&quot;;

            ArrayList files = new ArrayList();
            files.Add(&quot;pivot_ConsolidationExternal.xlsx&quot;);
            files.Add(&quot;pivot_TimelineConnectedToPivotTable.xlsx&quot;);
            files.Add(&quot;pivot_WithSpecialChars.xlsx&quot;);
            files.Add(&quot;PivotTables.xlsx&quot;);
            files.Add(&quot;simple-pivot-table.xlsx&quot;);

            Workbook wb = null;
            HtmlSaveOptions options = new HtmlSaveOptions
            {
                ExportImagesAsBase64 = true,
                ExportSingleTab = true,
                ExportHiddenWorksheet = false,
                HiddenRowDisplayType = HtmlHiddenRowDisplayType.Remove,
                HiddenColDisplayType = HtmlHiddenColDisplayType.Remove,
                ExportGridLines = true
            };

            string savePath = CreateFolder(filePath);
            for (int i = 0; i &lt; files.Count; i++)
            {
                string f = (string)files[i];
                wb = new Workbook(filePath + f);
                wb.Save(savePath + Path.GetFileName(f) + &quot;_out.html&quot;, options);
            }
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


