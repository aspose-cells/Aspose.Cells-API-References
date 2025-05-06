---
title: PivotFieldCollection.Move
second_title: Aspose.Cells for .NET API Reference
description: PivotFieldCollection method. Moves the PivotField from current position to destination position
type: docs
url: /net/aspose.cells.pivot/pivotfieldcollection/move/
---
## PivotFieldCollection.Move method

Moves the PivotField from current position to destination position

```csharp
public void Move(int currPos, int destPos)
```

| Parameter | Type | Description |
| --- | --- | --- |
| currPos | Int32 | Current position of PivotField based on zero |
| destPos | Int32 | Destination position of PivotField based on zero |

### Examples

```csharp
// Called: pt.RowFields.Move(1, 2);
[Test]
        public void Method_Int32_()
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

* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


