---
title: Font.Name
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets or sets the name of the Font
type: docs
url: /net/aspose.cells/font/name/
---
## Font.Name property

Gets or sets the name of the [`Font`](../).

```csharp
public virtual string Name { get; set; }
```

### Examples

```csharp
// Called: font.Name = FontNameConstants.zh_SongTi;
public void Font_Property_Name()
{
    caseName = "testColumnWidth_001";
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    Style style = workbook.DefaultStyle;
    Font font = style.Font;
    font.Name = FontNameConstants.zh_SongTi;
    font.Size = 12;
    workbook.DefaultStyle = style;
    cells.SetColumnWidth(2, 20.8);            

    checkColumnWidth_001(workbook);
    workbook.Save(Constants.destPath + "testColumnWidth.xls");            
    workbook = new Workbook(Constants.destPath + "testColumnWidth.xls");
    checkColumnWidth_001(workbook);
    workbook.Save(Constants.destPath + "testColumnWidth.xlsx");            
    workbook = new Workbook(Constants.destPath + "testColumnWidth.xlsx");
    checkColumnWidth_001(workbook);
    workbook.Save(Constants.destPath + "testColumnWidth.xml", SaveFormat.SpreadsheetML);            
    workbook = new Workbook(Constants.destPath + "testColumnWidth.xml");
    checkColumnWidth_001(workbook);
    workbook.Save(Constants.destPath + "testColumnWidth.xls");
}
```

### See Also

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


