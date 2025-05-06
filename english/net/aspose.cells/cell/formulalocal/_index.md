---
title: Cell.FormulaLocal
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Get the locale formatted formula of the cell
type: docs
url: /net/aspose.cells/cell/formulalocal/
---
## Cell.FormulaLocal property

Get the locale formatted formula of the cell.

```csharp
public string FormulaLocal { get; set; }
```

### Examples

```csharp
// Called: cell.FormulaLocal = fmlLoc;
[Test]
	    public void Property_FormulaLocal()
        { //CELLSNET-45697
	        Workbook wb = new Workbook();
            wb.Worksheets[0].PageSetup.PrintArea = &quot;B2:D3&quot;;
            wb.Worksheets[0].Cells[&quot;C2&quot;].PutValue(10000);
            wb.Worksheets.Add(&quot;Sheet2&quot;).PageSetup.PrintArea = &quot;C3:D5&quot;;
            wb.Worksheets[1].Cells[&quot;C4&quot;].PutValue(20000);
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            string fmlStd = &quot;=SUM(1.23,Print_Area,{3.45,6.78,9.01;8.76,5.43,2.1},Sheet2!Print_Area,TRUE,FALSE,&quot;
                + &quot;ERROR.TYPE(#NAME?),ERROR.TYPE(#DIV/0!),ERROR.TYPE(#REF!),ERROR.TYPE(#VALUE!),&quot;
                + &quot;ERROR.TYPE(#N/A),ERROR.TYPE(#NUM!),ERROR.TYPE(#NULL!))&quot;;
            string fmlLoc = &quot;=SUMME(1,23;XXX_XX;{3,45\\6,78\\9,01;8,76\\5,43\\2,1};Sheet2!XXX_XX;GLT;GLF;&quot;
                + &quot;GLET(#ИМЯ?);GLET(#ДЕЛ/0!);GLET(#ССЫЛКА!);GLET(#ЗНАЧ!);&quot;
                + &quot;GLET(#Н/Д);GLET(#ЧИСЛО!);GLET(#ПУСТО!))&quot;;

            cell.Formula = fmlStd;
            wb.CalculateFormula(false);
            double v = cell.DoubleValue;
            wb.Settings.GlobalizationSettings = new GlobalizationForFormula();
            wb.Settings.Region = CountryCode.Germany;

            CheckSetFormulaLocal(&quot;After Cell.Formula&quot;, cell, fmlStd, fmlLoc);

            cell.FormulaLocal = fmlLoc;
            CheckSetFormulaLocal(&quot;After Cell.FormulaLocal&quot;, cell, fmlStd, fmlLoc);
            wb.CalculateFormula(false);
            Assert.AreEqual(v, cell.DoubleValue, &quot;Calculated value after setting FormulaLocal&quot;);

            cell.SetFormula(fmlStd, new FormulaParseOptions(), null);
            CheckSetFormulaLocal(&quot;After Cell.SetFormula(local as false)&quot;, cell, fmlStd, fmlLoc);
            wb.CalculateFormula(false);
            Assert.AreEqual(v, cell.DoubleValue, &quot;Calculated value after Cell.SetFormula(local as false)&quot;);

            cell.SetFormula(fmlLoc, new FormulaParseOptions() { LocaleDependent = true }, null);
            CheckSetFormulaLocal(&quot;After Cell.SetFormula(local as true)&quot;, cell, fmlStd, fmlLoc);
            wb.CalculateFormula(false);
            Assert.AreEqual(v, cell.DoubleValue, &quot;Calculated value after Cell.SetFormula(local as true)&quot;);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


