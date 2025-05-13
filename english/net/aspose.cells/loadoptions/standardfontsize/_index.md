---
title: LoadOptions.StandardFontSize
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Sets the default standard font size
type: docs
url: /net/aspose.cells/loadoptions/standardfontsize/
---
## LoadOptions.StandardFontSize property

Sets the default standard font size.

```csharp
[Obsolete("Use DefaultStyleSettings.FontSize property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double StandardFontSize { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This property will be removed 12 months later since March 2022. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: loadOptions.StandardFontSize = 11;
public void LoadOptions_Property_StandardFontSize()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"NET45057/";
    HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
    loadOptions.SupportDivTag = true;
    loadOptions.KeepPrecision = true;
    loadOptions.DeleteRedundantSpaces = true;
    loadOptions.AutoFitColsAndRows = true;
    loadOptions.StandardFont = "Calibri";
    loadOptions.StandardFontSize = 11;

    Workbook wb = new Workbook(filePath + "s1.htm", loadOptions);


    var worksheet = wb.Worksheets[0];
    Cells cells = worksheet.Cells;
    Assert.AreEqual(cells["A1"].GetStyle().Font.Name, "Calibri");
    Assert.AreEqual(cells["A1"].GetStyle().Font.Size, 11);

    Assert.AreEqual(cells["D11"].GetStyle().IsTextWrapped, true);
    Assert.AreEqual(cells["G11"].GetStyle().IsTextWrapped, true);

    Assert.AreEqual(cells["A28"].GetStyle().IsTextWrapped, true);
    Assert.AreEqual(cells["A28"].GetStyle().VerticalAlignment, TextAlignmentType.Center);
    Console.WriteLine(cells["A28"].GetStyle().Font.Color);
    if (cells["A28"].IsRichText())
    {
        Assert.AreEqual(cells["A28"].GetCharacters()[0].Font.Color, Color.FromArgb(255, 220, 20, 60));
    }
    else
    {
        Assert.AreEqual(cells["A28"].GetStyle().Font.Color, Color.FromArgb(255, 220, 20, 60));
    }

    Assert.AreEqual(cells["A292"].GetStyle().Borders[BorderType.TopBorder].LineStyle, CellBorderType.None);

    Assert.Greater(cells.Columns[0].Width, 35);
    Assert.Greater(cells.Columns[6].Width, 25);

    for (int i = 0; i < worksheet.Pictures.Count; i++)
    {
        Aspose.Cells.Drawing.Picture pic = worksheet.Pictures[i];
        pic.Height = 250;
        pic.Width = 300;
        worksheet.Cells.SetRowHeight(pic.UpperLeftRow, 200);

    }

    wb.Save(CreateFolder(filePath) + "out.xlsx");
}
```

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


