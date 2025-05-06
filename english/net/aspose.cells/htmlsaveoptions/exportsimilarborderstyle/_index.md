---
title: HtmlSaveOptions.ExportSimilarBorderStyle
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to import the html or mht file to excel please keep the default value. The default value is false
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportsimilarborderstyle/
---
## HtmlSaveOptions.ExportSimilarBorderStyle property

Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to import the html or mht file to excel, please keep the default value. The default value is false.

```csharp
public bool ExportSimilarBorderStyle { get; set; }
```

### Examples

```csharp
// Called: options.ExportSimilarBorderStyle = true;
[Test]
        public void Property_ExportSimilarBorderStyle()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Java43579.xlsx&quot;);
            WorksheetCollection sheetCollection = workbook.Worksheets;
            int sheetCont = sheetCollection.Count;
            for (int i = 0; i &lt; sheetCont; i++)
            {
                AutoFitterOptions fitterOptions = new AutoFitterOptions();
                // fitterOptions.AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine;
                sheetCollection[i].AutoFitColumns(fitterOptions);
            }
            //workbook.Save(dir + &quot;dest.xlsx&quot;);
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportDocumentProperties = false;
            options.ExportWorkbookProperties = false;
            options.ExportWorkbookProperties = false;
            options.ExportSimilarBorderStyle = true;
            options.ExportImagesAsBase64 = false;
            options.ExcludeUnusedStyles = true;
            options.ExportHiddenWorksheet = false;
            options.WidthScalable = false;
            options.PresentationPreference = true;
            options.HtmlCrossStringType = HtmlCrossType.CrossHideRight;

            options.ExportActiveWorksheetOnly = true;
            workbook.Worksheets.ActiveSheetIndex = 0;
            workbook.Save(_destFilesPath + &quot;Java43579.html&quot;, options);
            string text = File.ReadAllText(_destFilesPath + &quot;Java43579.html&quot;);
            Assert.IsTrue(text.IndexOf(&quot;&lt;td colspan=&apos;2&apos; class=&apos;x149&apos; style=&apos;visibility:hidden;border-right:1px solid windowtext;border-bottom:1px solid windowtext;&apos;&gt;浙商银行广州开发区支行&lt;/td&gt;&quot;) != -1);

            Regex reg = new Regex(@&quot;&lt;td.*?(&amp;nbsp;)+.*?\-&lt;span.*?&gt;(&amp;nbsp;){3}&lt;/span&gt;&lt;/td&gt;&quot;);
            Assert.IsTrue(reg.IsMatch(text));
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


