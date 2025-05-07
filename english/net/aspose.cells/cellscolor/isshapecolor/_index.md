---
title: CellsColor.IsShapeColor
second_title: Aspose.Cells for .NET API Reference
description: CellsColor property. Gets and set the color which should apply to cell or shape
type: docs
url: /net/aspose.cells/cellscolor/isshapecolor/
---
## CellsColor.IsShapeColor property

Gets and set the color which should apply to cell or shape.

```csharp
public bool IsShapeColor { get; set; }
```

### Remarks

The expression of the color of the cell and the shape is different. For example: the theme color with same tint value will be not same in the cell and the shape.

### Examples

```csharp
// Called: clr.IsShapeColor = true;
[Test]
        public void Property_IsShapeColor()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsJava40851.xlsx");

            Workbook b = new Workbook();
            b.Copy(workbook);
            Util.SaveManCheck(b, "Shape", "CellsJava40851.xlsx");
             workbook = new Workbook();

            //Access the first worksheet 
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Shape should be transparent.");
            //Add your picture inside the worksheet 
            int pid = worksheet.Pictures.Add(5, 5, Constants.sourcePath + "TAMSA_11919191.gif");
            Picture pic = worksheet.Pictures[pid];

            //Create cells color 
            CellsColor clr = workbook.CreateCellsColor();
            clr.Color = Color.FromArgb(255, 255, 255);
            clr.IsShapeColor = true;

            //Make this color transparent for this picture 
            pic.FormatPicture.TransparentColor = clr;

            Util.SaveManCheck(b, "Shape", "CELLSNET-43131.xls");

            workbook = new Workbook(Constants.sourcePath + "CELLSNET-43290.xlsx");


            Util.SaveManCheck(workbook, "Shape", "CELLSNET-43290.xlsx");
            workbook = new Workbook(Constants.sourcePath + "CELLSNET-43325.xltx");


            Util.SaveManCheck(workbook, "Shape", "CELLSNET-43325.xlsx");
            workbook = new Workbook(Constants.sourcePath + "CELLSNET-43456.xls");
            Util.SaveManCheck(workbook, "Shape", "CELLSNET-43456.xls");
            workbook = new Workbook(Constants.sourcePath + "CELLSNET-43767.xls");
            Util.SaveManCheck(workbook, "Shape", "CELLSNET-43767.xls");
            //workbook = new Workbook(Constants.sourcePath + "CELLSJAVA-41258.xlsx");
            //Util.SaveManCheck(workbook, "Shape", "CELLSJAVA-41258.xlsx");
            //workbook = new Workbook(Constants.sourcePath + "CELLSJAVA-41258.xlsx");
            //Util.SaveManCheck(workbook, "Shape", "CELLSJAVA-41258.xlsx");
        }
```

### See Also

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


