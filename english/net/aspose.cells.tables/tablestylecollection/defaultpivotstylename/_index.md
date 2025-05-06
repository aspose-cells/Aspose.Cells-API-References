---
title: TableStyleCollection.DefaultPivotStyleName
second_title: Aspose.Cells for .NET API Reference
description: TableStyleCollection property. Gets and sets the default style name of pivot table 
type: docs
url: /net/aspose.cells.tables/tablestylecollection/defaultpivotstylename/
---
## TableStyleCollection.DefaultPivotStyleName property

Gets and sets the default style name of pivot table .

```csharp
public string DefaultPivotStyleName { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;PivotStyleLight16&amp;quot;, tableStyles.DefaultPivotStyleName);
[Test]
        public void Property_DefaultPivotStyleName()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET53937.xlsx&quot;);
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            Assert.AreEqual(&quot;TableStyleDark3&quot;, tableStyles.DefaultTableStyleName);
            Assert.AreEqual(&quot;PivotStyleLight16&quot;, tableStyles.DefaultPivotStyleName);

            tableStyles.DefaultTableStyleName = &quot;TableStyleMedium9&quot;;
            workbook.Save(Constants.destPath + &quot;CELLSNET53937.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET53937.xlsx&quot;);
            tableStyles = workbook.Worksheets.TableStyles;
            Assert.AreEqual(&quot;TableStyleMedium9&quot;, tableStyles.DefaultTableStyleName);
        }
```

### See Also

* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


