---
title: Validation.Operator
second_title: Aspose.Cells for .NET API Reference
description: Validation property. Represents the operator for the data validation
type: docs
url: /net/aspose.cells/validation/operator/
---
## Validation.Operator property

Represents the operator for the data validation.

```csharp
public OperatorType Operator { get; set; }
```

### Examples

```csharp
// Called: vldt.Operator = OperatorType.GreaterThan;
[Test]
        public void Property_Operator()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Validation vldt = sheet.Validations[sheet.Validations.Add(CellArea.CreateCellArea(5, 3, 6, 3))];
            vldt.Operator = OperatorType.GreaterThan;
            vldt.Formula1 = &quot;F3&quot;;

            vldt.AddArea(CellArea.CreateCellArea(3, 3, 3, 4), false, true);
            Assert.AreEqual(2, vldt.Areas.Length, &quot;Area count after changing base&quot;);
            Assert.AreEqual(&quot;=F3&quot;, vldt.Formula1, &quot;Formula1 after changing base, now total 2 areas&quot;);
            vldt.RemoveArea(CellArea.CreateCellArea(3, 3, 3, 4));
            Assert.AreEqual(1, vldt.Areas.Length, &quot;Area count after removing base&quot;);
            Assert.AreEqual(&quot;=F3&quot;, vldt.Formula1, &quot;Formula1 after removing base&quot;);

            CellArea[] areas = new CellArea[8000];
            for (int i = 0; i &lt; areas.Length; i++)
            {
                areas[i] = CellArea.CreateCellArea(6 + (i&lt;&lt;1), 3, 6 + (i&lt;&lt;1), 4);
            }
            TimePerformance monitor = new TimePerformance(5);
            monitor.StartPerfTest();
            foreach (CellArea item in areas)
            {
                vldt.AddArea(item);
            }
            Console.WriteLine(&quot;PerfBase of adding one by one: &quot; + monitor.GenPerfBase());
            //monitor.FinishPerfTest(&quot;Validation.AddArea&quot;);
            Assert.AreEqual(&quot;=F3&quot;, vldt.Formula1, &quot;Formula1 after adding one by one without changing base&quot;);
            vldt.AddArea(CellArea.CreateCellArea(3, 3, 3, 4), false, true);
            Assert.AreEqual(areas.Length + 2, vldt.Areas.Length, &quot;Area count before removing base&quot;);
            Assert.AreEqual(&quot;=F3&quot;, vldt.Formula1,
                &quot;Formula1 after changing base, now total 802 areas&quot;);
            vldt.RemoveArea(CellArea.CreateCellArea(3, 3, 3, 4));
            Assert.AreEqual(areas.Length + 1, vldt.Areas.Length, &quot;Area count after removing base&quot;);
            Assert.AreEqual(&quot;=F3&quot;, vldt.Formula1,
                &quot;Formula1 after removing base, now total 801 areas&quot;);

            monitor.StartPerfTest();
            foreach (CellArea item in areas)
            {
                vldt.RemoveArea(item);
            }
            Console.WriteLine(&quot;PerfBase of removing one by one: &quot; + monitor.GenPerfBase());
            Assert.AreEqual(1, vldt.Areas.Length, &quot;Area count after removing one by one&quot;);
            Assert.AreEqual(&quot;=F3&quot;, vldt.Formula1, &quot;Formula1 after removing one by one without changing base&quot;);

            monitor.StartPerfTest();
            areas[areas.Length/2] = CellArea.CreateCellArea(3, 3, 3, 4);
            vldt.AddAreas(areas, true, true);
            Console.WriteLine(&quot;PerfBase of bulk adding: &quot; + monitor.GenPerfBase());
            Assert.AreEqual(areas.Length + 1, vldt.Areas.Length, &quot;Area count after bulk adding&quot;);
            Assert.AreEqual(&quot;=F3&quot;, vldt.Formula1,
                &quot;Formula1 after changing base by bulk adding, now total 801 areas&quot;);

            monitor.StartPerfTest();
            vldt.RemoveAreas(areas);
            Console.WriteLine(&quot;PerfBase of bulk removing: &quot; + monitor.GenPerfBase());
            Assert.AreEqual(1, vldt.Areas.Length, &quot;Area count after bulk removing&quot;);
            Assert.AreEqual(&quot;=F3&quot;, vldt.Formula1, &quot;Formula1 after changing base, now total 1 area&quot;);
        }
```

### See Also

* enum [OperatorType](../../operatortype/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


