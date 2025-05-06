---
title: WorkbookDesigner.RepeatFormulasWithSubtotal
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner property. Indicates whether repeating formulas with subtotal row
type: docs
url: /net/aspose.cells/workbookdesigner/repeatformulaswithsubtotal/
---
## WorkbookDesigner.RepeatFormulasWithSubtotal property

Indicates whether repeating formulas with subtotal row.

```csharp
public bool RepeatFormulasWithSubtotal { get; set; }
```

### Examples

```csharp
// Called: designer.RepeatFormulasWithSubtotal = (true);
[Test]
        public void Property_RepeatFormulasWithSubtotal()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;SmartMarker/CellsJava43435.xlsx&quot;);
            //Workbook workbook = new Workbook(dataDir + &quot;TestSmartMarkers.xlsx&quot;);

            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = (workbook);

            List&lt;Level&gt; list = new List&lt;Level&gt;();
            list.Add(new Level(&quot;A&quot;, &quot;A1&quot;));
            list.Add(new Level(&quot;B&quot;, &quot;B1&quot;));
            //list.add(new Level(&quot;B&quot;, &quot;B2&quot;));
            //list.add(new Level(&quot;C&quot;, &quot;C1&quot;));
            //list.add(new Level(&quot;C&quot;, &quot;C2&quot;));
            //list.add(new Level(&quot;C&quot;, &quot;C3&quot;));

            List&lt;NumberData&gt; list2 = new List&lt;NumberData&gt;();
            list2.Add(new NumberData(1, 2));
            list2.Add(new NumberData(3, 4));
            list2.Add(new NumberData(5, 6));
            list2.Add(new NumberData(7, 8));
            list2.Add(new NumberData(9, 10));
            list2.Add(new NumberData(11, 12));

            designer.SetDataSource(&quot;Level&quot;, list);
            designer.SetDataSource(&quot;NumData&quot;, list2);
            // designer.setCalculateFormula(true);
            designer.RepeatFormulasWithSubtotal = (true);
            designer.Process();
            Assert.AreEqual(&quot;=A7+B7&quot;, designer.Workbook.Worksheets[0].Cells[&quot;D7&quot;].Formula);
            workbook.Save(Constants.destPath + &quot;CellsJava43435.xlsx&quot;);
        }
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


