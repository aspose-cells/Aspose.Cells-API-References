---
title: PivotField.GetFormula
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Gets formula of the calculated field 
type: docs
url: /net/aspose.cells.pivot/pivotfield/getformula/
---
## PivotField.GetFormula method

Gets formula of the calculated field .

```csharp
public string GetFormula()
```

### Examples

```csharp
// Called: string str = pt.BaseFields[pt.BaseFields.Count - 1].GetFormula();
[Test]
        public void Method_GetFormula()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "CELLSNET54009.xlsx");
            PivotTable pt = workbook.Worksheets[0].PivotTables[0];
            string str = pt.BaseFields[pt.BaseFields.Count - 1].GetFormula();
            Assert.AreEqual("='1月'+'2月'", str);
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


