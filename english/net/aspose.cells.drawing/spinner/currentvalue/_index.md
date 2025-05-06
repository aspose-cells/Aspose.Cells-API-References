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
            Workbook objWB = new Workbook(Constants.sourcePath + &quot;CellsNet47600.xlsx&quot;);
            foreach (Shape objShape in objWB.Worksheets[0].Shapes)
            {
                if (!String.IsNullOrEmpty(objShape.MacroName))
                {
                    Assert.AreEqual(&quot;Button 15&quot;, objShape.Name);
                    if (!objShape.MacroName.EndsWith(@&quot;Rafik\New AT.xls&apos;!Button31_Click&quot;))
                    {
                        Assert.Fail(&quot;&apos;Button 15&apos;.MacroName should end with \&quot;Rafik\\New AT.xls&apos;!Button31_Click\&quot; but was: &quot;
                            + objShape.MacroName);
                    }
                }
                if (objShape.MsoDrawingType == MsoDrawingType.Spinner)
                {
                    Assert.AreEqual(10, ((Spinner)objShape).CurrentValue);
                }
                if (objShape.MsoDrawingType == MsoDrawingType.ScrollBar)
                {
                    Assert.AreEqual(&quot;Scroll Bar 24&quot;, objShape.Name);
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


