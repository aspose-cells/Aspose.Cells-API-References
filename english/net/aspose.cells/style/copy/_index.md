---
title: Style.Copy
second_title: Aspose.Cells for .NET API Reference
description: Style method. Copies data from another style object
type: docs
url: /net/aspose.cells/style/copy/
---
## Style.Copy method

Copies data from another style object

```csharp
public void Copy(Style style)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | Source Style object |

### Remarks

This method does not copy the name of the style. If you want to copy the name, please call the following codes after copying style: destStyle.Name = style.Name.

### Examples

```csharp
// Called: styleDest.Copy(styleSrc);
[Test]
        public void Method_Style_()
        {
            caseName = "testCopy_001";
            Workbook workbook = new Workbook();            
            workbook = new Workbook(Constants.sourcePath + @"Style/Style_001.xls");
            Cells cells = workbook.Worksheets[0].Cells;
            Style styleSrc = cells[1, 1].GetStyle();
            Style styleDest = cells[3, 1].GetStyle();
            styleDest.Copy(styleSrc);
            cells[3, 1].SetStyle(styleDest);

            checkCopy_001(workbook);
            workbook.Save(Constants.destPath + "testCopy.xls");
            workbook = new Workbook(Constants.destPath + "testCopy.xls");
            checkCopy_001(workbook);
            workbook.Save(Constants.destPath + "testCopy.xlsx");
            workbook = new Workbook(Constants.destPath + "testCopy.xlsx");
            checkCopy_001(workbook);
            workbook.Save(Constants.destPath + "testCopy.xml", SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + "testCopy.xml");
            checkCopy_001(workbook);
            workbook.Save(Constants.destPath + "testCopy.xls");
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


