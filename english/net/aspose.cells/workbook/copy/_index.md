---
title: Workbook.Copy
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Copies another Workbook object
type: docs
url: /net/aspose.cells/workbook/copy/
---
## Copy(Workbook, CopyOptions) {#copy_1}

Copies another Workbook object.

```csharp
public void Copy(Workbook source, CopyOptions copyOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| source | Workbook | Source Workbook object. |
| copyOptions | CopyOptions | The options of copying other workbook. |

### Remarks

It's very simple to clone an Excel file.

### Examples

```csharp
// Called: workbook1.Copy(workbook2, options);
[Test]
        public void Method_CopyOptions_()
        {
            var workbook1 = new Workbook(Constants.sourcePath + @&quot;CellsNet47570.xlsm&quot;);
           
            var workbook2 = new Workbook(Constants.sourcePath + @&quot;CellsNet47570.xlsx&quot;);
            CopyOptions options = new CopyOptions();
            options.KeepMacros = true;
            workbook1.Copy(workbook2, options);
            Assert.AreEqual(1,workbook1.VbaProject.Modules.Count);
            workbook1.Save(Constants.destPath + &quot;CellsNet47570.xlsm&quot;);
        }
```

### See Also

* class [CopyOptions](../../copyoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Copy(Workbook) {#copy}

Copies data from a source Workbook object.

```csharp
public void Copy(Workbook source)
```

| Parameter | Type | Description |
| --- | --- | --- |
| source | Workbook | Source Workbook object. |

### Examples

```csharp
// Called: n.Copy(wb);
private void Method_Workbook_(bool copy)
        {
            Console.WriteLine(&quot;TestUsingChain: Init....&quot;);
            Workbook wb = new Workbook();
            wb.Worksheets.Add(&quot;Data&quot;);
            long tt = DateTime.Now.ToFileTimeUtc();
            Cells cellsF = wb.Worksheets[0].Cells;
            Cells cellsD = wb.Worksheets[1].Cells;
            for (int i = 0; i &lt; 30; i++)
            {
                SetFormulas(cellsF, i);
            }
            CalculationOptions copts = new CalculationOptions();
            CheckUsingChain cMonitor = new CheckUsingChain();
            copts.CalculationMonitor = cMonitor;
            long time1 = DateTime.Now.ToFileTimeUtc();
            wb.CalculateFormula(copts);
            time1 = DateTime.Now.ToFileTimeUtc() - time1;
            cMonitor.CheckWithoutChain();
            Thread.Sleep(100);
            wb.Settings.FormulaSettings.EnableCalculationChain = true;
            cMonitor.ResetForCalculation();
            long time2 = DateTime.Now.ToFileTimeUtc();
            wb.CalculateFormula(copts); //chain is created here
            time2 = DateTime.Now.ToFileTimeUtc() - time2;
            if (time1 &gt; time2)
            {
                time1 = time2;
            }
            cMonitor.CheckWithoutChain();
            if (copy)
            {
                Console.WriteLine(&quot;Copying workbook with chain...&quot;);
                Workbook n = new Workbook();
                n.Copy(wb);
                wb = n;
                cellsF = wb.Worksheets[0].Cells;
                cellsD = wb.Worksheets[1].Cells;
            }
            for (int i = 0; i &lt; 30; i++)
            {
                Thread.Sleep(100);
                cellsF[i, 16].PutValue(1);
                cMonitor.ResetForCalculation();
                Console.WriteLine(&quot;TestUsingChain: Calculating....&quot; + i);
                //time2 = DateTime.Now.ToFileTimeUtc();
                wb.CalculateFormula(copts);
                //time2 = DateTime.Now.ToFileTimeUtc() - time2;
                //if ((time2 &lt;&lt; 1) &gt; time1)
                //{
                //    Console.WriteLine(&quot;Time performance: with chain is &quot; + time2 + &quot;, without chain is &quot; + time1);
                //}
                cMonitor.CheckWithChain(i, false);
                Thread.Sleep(100);
                cellsD[i, 16].PutValue(1);
                cMonitor.ResetForCalculation();
                //time2 = DateTime.Now.ToFileTimeUtc();
                wb.CalculateFormula(copts);
                //time2 = DateTime.Now.ToFileTimeUtc() - time2;
                //if ((time2 &lt;&lt; 1) &gt; time1)
                //{
                //    Console.WriteLine(&quot;Time performance: with chain is &quot; + time2 + &quot;, without chain is &quot; + time1);
                //}
                cMonitor.CheckWithChain(i, true);
            }
            Console.WriteLine(&quot;Test time cost: &quot;
                + ((DateTime.Now.ToFileTimeUtc() - tt) / 10000000.0).ToString(&quot;#,##0.###&quot;));
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


