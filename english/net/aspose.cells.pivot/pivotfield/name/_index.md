---
title: PivotField.Name
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Represents the name of PivotField
type: docs
url: /net/aspose.cells.pivot/pivotfield/name/
---
## PivotField.Name property

Represents the name of PivotField.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: string str = pt.RowFields[1].Name;
[Test]
        public void Property_Name()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;JAVA42604_&quot;;
            Workbook workbook = new Workbook(filePath + &quot;pivot.xlsx&quot;);
            PivotTable pt = workbook.Worksheets[0].PivotTables[0];
            pt.AddFieldToArea(PivotFieldType.Row, 1);
            pt.AddFieldToArea(PivotFieldType.Row, 2);
            pt.AddFieldToArea(PivotFieldType.Row, 3);
            string str = pt.RowFields[1].Name;
            pt.RowFields.Move(1, 2);
            Assert.AreEqual(str, pt.RowFields[2].Name);
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


