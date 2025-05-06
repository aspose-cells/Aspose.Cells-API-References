---
title: Cell.Type
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Represents cell value type
type: docs
url: /net/aspose.cells/cell/type/
---
## Cell.Type property

Represents cell value type.

```csharp
public CellValueType Type { get; }
```

### Examples

```csharp
// Called: if (cell.Type == CellValueType.IsNumeric)
[Test]
        public void Property_Type()
        {
            bool failed = false;
            Workbook wbData = new Workbook(Constants.sourcePath + &quot;Formula\\ExternalLinkSource.xlsx&quot;);
            Workbook wbCalc = new Workbook(Constants.sourcePath + &quot;Formula\\ExternalFormula.xlsx&quot;);
            wbCalc.CalculateFormula(false);
            if (!FormulaCaseUtil.VerifyCalc(wbCalc,
                new Workbook(Constants.sourcePath + &quot;Formula\\ExternalFormula_NoLink.xlsx&quot;)))
            {
                failed = true;
                Console.WriteLine(&quot;Recalculate with embedded data source failed.&quot;);
            }
            else
            {
                Console.WriteLine(&quot;Recalculate with embedded data source succeeded.&quot;);
            }
            wbCalc.UpdateLinkedDataSource(new Workbook[] { wbData });
            wbCalc.CalculateFormula(false);
            Workbook wbBase = new Workbook(Constants.sourcePath + &quot;Formula\\ExternalFormula.xlsx&quot;);
            if (!FormulaCaseUtil.VerifyCalc(wbCalc, wbBase))
            {
                failed = true;
                Console.WriteLine(&quot;Recalculate with original data source failed.&quot;);
            }
            else
            {
                Console.WriteLine(&quot;Recalculate with original data source succeeded.&quot;);
            }
            //wbCalc.Save(Constants.sourcePath + &quot;Formula\\ExternalFormula_res.xlsx&quot;);
            wbCalc = Util.ReSave(wbCalc, SaveFormat.Xlsx);
            wbCalc.CalculateFormula(false);
            if (!FormulaCaseUtil.VerifyCalc(wbCalc,
                new Workbook(Constants.sourcePath + &quot;Formula\\ExternalFormula_NoLink.xlsx&quot;)))
            {
                failed = true;
                Console.WriteLine(&quot;Calculate resaved workbook with embedded data source failed.&quot;);
            }
            else
            {
                Console.WriteLine(&quot;Calculate resaved workbook with embedded data source succeeded.&quot;);
            }
            IEnumerator en;
            foreach (Worksheet sheet in wbData.Worksheets)
            {
                en = sheet.Cells.GetEnumerator();
                while (en.MoveNext())
                {
                    Cell cell = (Cell)en.Current;
                    if (cell.Type == CellValueType.IsNumeric)
                    {
                        double dv = cell.DoubleValue;
                        if (dv &gt; 0.0)
                        {
                            cell.PutValue(dv + 1.0);
                        }
                        else if (dv &lt; 0.0)
                        {
                            cell.PutValue(dv - 1.0);
                        }
                    }
                }
            }
            //wbData.Save(Constants.sourcePath + &quot;Formula\\ExternalLinkSource_New.xlsx&quot;);
            Cells cells = wbBase.Worksheets[0].Cells;
            cells[&quot;A2&quot;].PutValue(2);
            cells[&quot;A6&quot;].PutValue(520);
            cells[&quot;A7&quot;].PutValue(262161);
            cells[&quot;A9&quot;].PutValue(-520);
            cells[&quot;A10&quot;].PutValue(-65);
            cells[&quot;A12&quot;].PutValue(-65);
            cells[&quot;A13&quot;].PutValue(2);
            wbData.FileName = &quot;ExternalLinkSource.xlsx&quot;;
            wbCalc.UpdateLinkedDataSource(new Workbook[] { wbData });
            wbCalc.CalculateFormula(false);
            if (!FormulaCaseUtil.VerifyCalc(wbCalc, wbBase))
            {
                failed = true;
                Console.WriteLine(&quot;Recalculate with updated data source failed.&quot;);
            }
            else
            {
                Console.WriteLine(&quot;Recalculate with updated data source succeeded.&quot;);
            }
            if (failed)
            {
                Assert.Fail(&quot;Test failed. Please see the error messages shown in the process.&quot;);
            }
        }
```

### See Also

* enum [CellValueType](../../cellvaluetype/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


