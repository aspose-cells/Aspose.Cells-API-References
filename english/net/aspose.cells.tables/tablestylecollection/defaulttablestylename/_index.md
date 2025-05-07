---
title: TableStyleCollection.DefaultTableStyleName
second_title: Aspose.Cells for .NET API Reference
description: TableStyleCollection property. Gets and sets the default style name of the table
type: docs
url: /net/aspose.cells.tables/tablestylecollection/defaulttablestylename/
---
## TableStyleCollection.DefaultTableStyleName property

Gets and sets the default style name of the table.

```csharp
public string DefaultTableStyleName { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("TableStyleDark3", tableStyles.DefaultTableStyleName);
[Test]
        public void Property_DefaultTableStyleName()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET53937.xlsx");
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            Assert.AreEqual("TableStyleDark3", tableStyles.DefaultTableStyleName);
            Assert.AreEqual("PivotStyleLight16", tableStyles.DefaultPivotStyleName);

            tableStyles.DefaultTableStyleName = "TableStyleMedium9";
            workbook.Save(Constants.destPath + "CELLSNET53937.xlsx");
            workbook = new Workbook(Constants.destPath + "CELLSNET53937.xlsx");
            tableStyles = workbook.Worksheets.TableStyles;
            Assert.AreEqual("TableStyleMedium9", tableStyles.DefaultTableStyleName);
        }
```

### See Also

* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


