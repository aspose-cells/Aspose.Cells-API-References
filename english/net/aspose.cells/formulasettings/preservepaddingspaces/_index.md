---
title: FormulaSettings.PreservePaddingSpaces
second_title: Aspose.Cells for .NET API Reference
description: FormulaSettings property. Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false
type: docs
url: /net/aspose.cells/formulasettings/preservepaddingspaces/
---
## FormulaSettings.PreservePaddingSpaces property

Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false.

```csharp
public bool PreservePaddingSpaces { get; set; }
```

### Remarks

Generally those spaces and line breaks are jsut for visual purpose, Preserving them or not does not affect the calculated result. For performance consideration, if there is no special requirement, it is better not to preserve them while processing formulas.

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Settings.FormulaSettings.PreservePaddingSpaces ? fml : fml.Replace(&amp;quot; &amp;quot;, &amp;quot;&amp;quot;),
[Test]
        public void Property_PreservePaddingSpaces()
        {
            Aspose.Cells.WorkbookDesigner designer = new Aspose.Cells.WorkbookDesigner();
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;SmartMarker/41984.xlsx&quot;);
            designer.Workbook = workbook;
            designer.SetDataSource(&quot;AAA&quot;, &quot;ABCDEF&quot;);
            designer.Process();
            string fml = &quot;=SUM(A2:A1 )&quot;;
            Assert.AreEqual(workbook.Settings.FormulaSettings.PreservePaddingSpaces ? fml : fml.Replace(&quot; &quot;, &quot;&quot;),
                workbook.Worksheets[0].Cells[&quot;B2&quot;].Formula);
        }
```

### See Also

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


