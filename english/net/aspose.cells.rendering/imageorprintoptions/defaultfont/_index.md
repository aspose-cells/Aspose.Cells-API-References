---
title: ImageOrPrintOptions.DefaultFont
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. When characters in the Excel are Unicode and not be set with correct font in cell style They may appear as block in pdfimage. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set Aspose.Cells will use system default font to show these unicode characters
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/defaultfont/
---
## ImageOrPrintOptions.DefaultFont property

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters.

```csharp
public string DefaultFont { get; set; }
```

### Examples

```csharp
// Called: imgOption.DefaultFont = &amp;quot;SimSun&amp;quot;;
[Test]
        public void Property_DefaultFont()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;JAVA42953/&quot;;
            //string fileName = &quot;窗边堵缝清单.xls&quot;;
            string fileName = &quot;附件6.重庆雍景湾项目一期外墙石材及铝板安装工程--计量文件【审核稿】.xls&quot;;

            LoadOptions loadOptions = new LoadOptions();
            loadOptions.StandardFont = &quot;SimSun&quot;;
            loadOptions.Region = CountryCode.USA;
            loadOptions.MemorySetting = MemorySetting.MemoryPreference;
            Workbook excel = new Workbook(filePath + fileName, loadOptions);
            excel.AcceptAllRevisions();

            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportActiveWorksheetOnly = true;
            saveOptions.ExportHiddenWorksheet = false;
            saveOptions.ExportImagesAsBase64 = true;
            saveOptions.HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden;
            saveOptions.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden;
            saveOptions.LinkTargetType = HtmlLinkTargetType.Blank;

            int sheetCount = excel.Worksheets.Count;
            int originActiveIndex = excel.Worksheets.ActiveSheetIndex;
            Worksheet worksheet = null;

            Workbook checkExcel = getCheckExcel42953(new FileStream(filePath + fileName, FileMode.Open, FileAccess.ReadWrite));
            bool canApplyStyle = canApplyStyle42953(filePath, checkExcel, saveOptions);
            for (int i = 1; i &lt;= sheetCount; i++)
            {
                worksheet = checkExcel.Worksheets[i - 1];
                Cells cells1 = worksheet.Cells;
                Cell cell1 = cells1[&quot;A6&quot;];
                Style style1 = cell1.GetStyle();
                if (worksheet != null &amp;&amp; worksheet.IsVisible)
                {
                    excel.Worksheets.ActiveSheetIndex = i - 1;
                    if (canApplyStyle)
                    {
                        Style newStyle = checkExcel.CreateStyle();
                        newStyle.IsTextWrapped = true;
                        StyleFlag flag = new StyleFlag();
                        flag.WrapText = true;
                        newStyle.IsTextWrapped = true;
                        Cells cells = worksheet.Cells;
                        cells.ApplyStyle(newStyle, flag);
                    }
                    Cells cells2 = worksheet.Cells;
                    Cell cell2 = cells2[&quot;A6&quot;];
                    Style style2 = cell2.GetStyle();
                    if (originActiveIndex == i - 1)
                    {
                        worksheet.PageSetup.PrintArea = &quot;A1:I4&quot;;
                        ImageOrPrintOptions imgOption = new ImageOrPrintOptions();
                        imgOption.HorizontalResolution = 96;
                        imgOption.VerticalResolution = 96;
                        imgOption.DefaultFont = &quot;SimSun&quot;;
                        imgOption.Quality = 100;
                        imgOption.OutputBlankPageWhenNothingToPrint = true;
                        imgOption.ImageType = ImageType.Png;
                        SheetRender sheetRender = new SheetRender(worksheet, imgOption);
                        sheetRender.ToImage(0, CreateFolder(filePath) + &quot;thumbnail.png&quot;);
                    }
                    excel.Save(CreateFolder(filePath) + &quot;pageResult&quot; + i + &quot;.html&quot;, saveOptions);
                }
            }
        }
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


