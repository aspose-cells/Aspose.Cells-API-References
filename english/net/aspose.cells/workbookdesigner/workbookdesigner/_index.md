---
title: WorkbookDesigner.WorkbookDesigner
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner constructor. Initializes a new instance of the WorkbookDesigner class
type: docs
url: /net/aspose.cells/workbookdesigner/workbookdesigner/
---
## WorkbookDesigner() {#constructor}

Initializes a new instance of the [`WorkbookDesigner`](../) class.

```csharp
public WorkbookDesigner()
```

### Examples

```csharp
// Called: WorkbookDesigner designer = new WorkbookDesigner();
[Test]
        public void WorkbookDesigner_Constructor()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;SmartMarker/CellsJava43172.xlsx&quot;);
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = (workbook);
            designer.SetDataSource(&quot;VariableArray1&quot;, new String[] { &quot;TEst&quot;, &quot;Test2&quot;, &quot;TEST3&quot;, &quot;TEST4&quot; });
            designer.SetDataSource(&quot;VariableArray2&quot;, new String[] { &quot;SecondTEst&quot;, &quot;SecondTtest2&quot;, &quot;SecondTEST3&quot;, &quot;SecondTEST4&quot; });
            designer.Process();
            Assert.AreEqual(&quot;Test2&quot;, workbook.Worksheets[0].Cells[&quot;A3&quot;].StringValue);
            Assert.AreEqual(&quot;SecondTtest2&quot;, workbook.Worksheets[0].Cells[&quot;D1&quot;].StringValue);
            workbook.Save(Constants.destPath + &quot;CellsJava43172.xlsx&quot;);
        }
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## WorkbookDesigner(Workbook) {#constructor_1}

Initializes a new instance of the [`WorkbookDesigner`](../) class.

```csharp
public WorkbookDesigner(Workbook workbook)
```

| Parameter | Type | Description |
| --- | --- | --- |
| workbook | Workbook | The template workbook file. |

### Examples

```csharp
// Called: WorkbookDesigner designer = new WorkbookDesigner(template);
public void WorkbookDesigner_Constructor()
        {
            string dir = Constants.sourcePath + @&quot;SmartMarker\&quot;;
            Workbook workbook = new Workbook(dir + &quot;repaccs1.csv&quot;);
            Cells cells = workbook.Worksheets[0].Cells;
            List&lt;Accident&gt; accidents = ExportList&lt;Accident&gt;(workbook.Worksheets[0].Cells, 0, 0, cells.MaxDataRow, cells.MaxDataColumn);

             workbook = new Workbook(dir + &quot;repvehs1.csv&quot;);
             cells = workbook.Worksheets[0].Cells;
            List&lt;Vehicle&gt; vehicles = ExportList&lt;Vehicle&gt;(workbook.Worksheets[0].Cells, 0, 0, cells.MaxDataRow, cells.MaxDataColumn);

             workbook = new Workbook(dir + &quot;repcas1.csv&quot;);
             cells = workbook.Worksheets[0].Cells;
            List&lt;Casualty&gt; casualties = ExportList&lt;Casualty&gt;(workbook.Worksheets[0].Cells, 0, 0, cells.MaxDataRow, cells.MaxDataColumn);
            Merge(vehicles, casualties);
            Merge(accidents, vehicles);
            Workbook template = new Workbook(dir + &quot;CELLSNET54674.xlsx&quot;);
            WorkbookDesigner designer = new WorkbookDesigner(template);
            designer.LineByLine = false;
            designer.SetDataSource(&quot;Accidents&quot;, accidents);
            designer.Process();
            template.CalculateFormula();
            AssertHelper.AreEqual(&quot;Wet/Damp&quot;, template.Worksheets[0].Cells[&quot;A38&quot;].StringValue,&quot;&quot;);
            template.Save(Constants.destPath + &quot;CELLSNET54674.xlsx&quot;);
        }
```

### See Also

* class [Workbook](../../workbook/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


