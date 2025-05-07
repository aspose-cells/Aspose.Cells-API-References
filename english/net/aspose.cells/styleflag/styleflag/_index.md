---
title: StyleFlag.StyleFlag
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag constructor. Constructs an object with all flags as false
type: docs
url: /net/aspose.cells/styleflag/styleflag/
---
## StyleFlag constructor

Constructs an object with all flags as false.

```csharp
public StyleFlag()
```

### Examples

```csharp
// Called: StyleFlag sflag = new StyleFlag();
[Test]
        public void StyleFlag_Constructor()
        {
            caseName = "testApplyColumnStyle_002";
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Style style = getStyle(workbook);
            StyleFlag sflag = new StyleFlag();
            sflag.Borders = true;
            cells.ApplyColumnStyle(255, style, sflag);

            checkApplyColumnStyle_002(workbook);
            workbook.Save(Constants.destPath + "testApplyColumnStyle.xls");            
            workbook = new Workbook(Constants.destPath + "testApplyColumnStyle.xls");
            checkApplyColumnStyle_002(workbook);
            workbook.Save(Constants.destPath + "testApplyColumnStyle.xlsx");            
            workbook = new Workbook(Constants.destPath + "testApplyColumnStyle.xlsx");
            checkApplyColumnStyle_002(workbook);
            workbook.Save(Constants.destPath + "testApplyColumnStyle.xml", SaveFormat.SpreadsheetML);            
            workbook = new Workbook(Constants.destPath + "testApplyColumnStyle.xml");
            checkApplyColumnStyle_002(workbook);
            workbook.Save(Constants.destPath + "testApplyColumnStyle.xls");   
        }
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


