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
// Called: Assert.AreEqual(&amp;quot;=ABS(&amp;apos;ns1:TRN_AMOUNT&amp;apos;)&amp;quot;, fields[fields.Count - 1].GetFormula());
[Test]
        public void Method_GetFormula()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSNET52671.xlsx&quot;);
            PivotFieldCollection fields = workbook.Worksheets[1].PivotTables[0].BaseFields;
            Assert.AreEqual(&quot;=ABS(&apos;ns1:TRN_AMOUNT&apos;)&quot;, fields[fields.Count - 1].GetFormula());
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


