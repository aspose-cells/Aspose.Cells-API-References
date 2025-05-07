---
title: Spinner.CurrentValue
second_title: Aspose.Cells for .NET API Reference
description: Spinner property. Gets or sets the current value
type: docs
url: /net/aspose.cells.drawing/spinner/currentvalue/
---
## Spinner.CurrentValue property

Gets or sets the current value.

```csharp
public int CurrentValue { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(10, ((Spinner)objShape).CurrentValue);
[Test]
        public void Property_CurrentValue()
        {
            Workbook objWB = new Workbook(Constants.sourcePath + "CellsNet47600.xlsx");
            foreach (Shape objShape in objWB.Worksheets[0].Shapes)
            {
                if (!String.IsNullOrEmpty(objShape.MacroName))
                {
                    Assert.AreEqual("Button 15", objShape.Name);
                    if (!objShape.MacroName.EndsWith(@"Rafik\New AT.xls'!Button31_Click"))
                    {
                        Assert.Fail("'Button 15'.MacroName should end with \"Rafik\\New AT.xls'!Button31_Click\" but was: "
                            + objShape.MacroName);
                    }
                }
                if (objShape.MsoDrawingType == MsoDrawingType.Spinner)
                {
                    Assert.AreEqual(10, ((Spinner)objShape).CurrentValue);
                }
                if (objShape.MsoDrawingType == MsoDrawingType.ScrollBar)
                {
                    Assert.AreEqual("Scroll Bar 24", objShape.Name);
                    Assert.AreEqual(9, ((ScrollBar)objShape).CurrentValue);
                }
            }
            Util.ReSave(objWB, SaveFormat.Xlsx);
        }
```

### See Also

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


