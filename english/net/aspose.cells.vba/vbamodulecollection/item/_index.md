---
title: VbaModuleCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: VbaModuleCollection property. Gets VbaModule in the list by the index
type: docs
url: /net/aspose.cells.vba/vbamodulecollection/item/
---
## VbaModuleCollection indexer (1 of 2)

Gets [`VbaModule`](../../vbamodule/) in the list by the index.

```csharp
public VbaModule this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Examples

```csharp
// Called: wb.VbaProject.Modules[i].Codes = txtModule;
[Test]
        public void Property_Int32_()
        {
            Workbook wb = new Workbook(Constants.sourcePath +&quot;CELLSNET-42716.xlsm&quot;);
            Util.SetHintMessage(wb.Worksheets[0].Cells[&quot;A1&quot;], &quot;On the menu bar there should be one tab named as \&quot;Testing\&quot; and click it you should see one picture of spider&quot;);
            Util.SaveManCheck(wb, &quot;ExcelUI&quot;, &quot;CellsNet42716.xlsx&quot;);
            wb = new Workbook(Constants.sourcePath + &quot;CELLSNET-42716_2.xlsm&quot;);
            Util.SetHintMessage(wb.Worksheets[0].Cells[&quot;A1&quot;], &quot;On the menu bar there should be one tab named as \&quot;Testing\&quot; and click it you should see several pictures&quot;);
            Util.SaveManCheck(wb, &quot;ExcelUI&quot;, &quot;CellsNet42716_2.xlsm&quot;);
            wb = new Workbook(Constants.sourcePath + &quot;CELLSNET-42766.xlsx&quot;);
            Util.SetHintMessage(wb.Worksheets[0].Cells[&quot;A1&quot;], &quot;Click views-&gt; custom views-&gt;show.&quot;);
            Util.SaveManCheck(wb, &quot;ExcelUI&quot;, &quot;CELLSNET-42766.xlsx&quot;);
            wb = new Workbook(Constants.sourcePath + &quot;CELLSNET-42849.xlsx&quot;);
            wb.Worksheets.ActiveSheetIndex = wb.Worksheets[&quot;DPH1&quot;].Index;
            Util.SetHintMessage(wb.Worksheets[&quot;DPH1&quot;].Cells[&quot;X21&quot;], &quot;Right Click Cell J21-&gt; Xml(x) -&gt;Xml source&quot;);
            Util.SaveManCheck(wb, &quot;ExcelUI&quot;, &quot;CELLSNET-42849.xlsx&quot;);

            wb = new Workbook(Constants.sourcePath + &quot;CELLSJAVA-40918.xls&quot;);
            wb.Save(Constants.destPath + &quot;CELLSJAVA-40918.xlsx&quot;);
            wb = new Workbook(Constants.destPath + &quot;CELLSJAVA-40918.xlsx&quot;);
            Util.SaveManCheck(wb, &quot;ExcelUI&quot;, &quot;CELLSJAVA-40918.xls&quot;);
            wb = new Workbook(Constants.sourcePath + &quot;CELLSJAVA41196.xlsb&quot;);
            wb.Worksheets.Add(&quot;Newsheet1&quot;);
            wb.Worksheets.Add(&quot;Newsheet2&quot;);
            wb.Worksheets.Add(&quot;Newsheet3&quot;);
            Util.SaveManCheck(wb, &quot;ExcelUI&quot;, &quot;CELLSJAVA41196.xlsb&quot;);
            wb = new Workbook(Constants.sourcePath + &quot;CELLSNET43401.xlsm&quot;);
            for (int i = 0; i &lt; wb.VbaProject.Modules.Count; i++)
            {
                // workbook.VbaProject.Modules[i].Name = workbook.VbaProject.Modules[i].Name + &quot;sdfsdf&quot;;
                string txtModule = wb.VbaProject.Modules[i].Codes;
                txtModule = txtModule.Replace(&quot;ASPOSE&quot;, &quot;Shakeel&quot;);
                wb.VbaProject.Modules[i].Codes = txtModule;
            } 

            Util.SaveManCheck(wb, &quot;ExcelUI&quot;, &quot;CELLSNET43401.xlsm&quot;);
        }
```

### See Also

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)

---

## VbaModuleCollection indexer (2 of 2)

Gets [`VbaModule`](../../vbamodule/) in the list by the name.

```csharp
public VbaModule this[string name] { get; }
```

| Parameter | Description |
| --- | --- |
| name | The name of module. |

### Examples

```csharp
// Called: int x =  vbaProject.Modules.AddUserForm(&amp;quot;TestForm&amp;quot;, source.VbaProject.Modules[&amp;quot;TestForm&amp;quot;].Codes, source.VbaProject.Modules.GetDesignerStorage(&amp;quot;TestForm&amp;quot;));
[Test]
        public void Property_String_()
        {
            var source = new Workbook(Constants.sourcePath + &quot;CELLSNET54310.xlsm&quot;);
            var wb = new Workbook(Constants.sourcePath + &quot;CELLSNET54310.xlsm&quot;);
            VbaProject vbaProject = wb.VbaProject;
           int x =  vbaProject.Modules.AddUserForm(&quot;TestForm&quot;, source.VbaProject.Modules[&quot;TestForm&quot;].Codes, source.VbaProject.Modules.GetDesignerStorage(&quot;TestForm&quot;));
            Assert.IsNotNull(vbaProject.Modules.GetDesignerStorage(&quot;TestForm&quot;));
            Assert.IsNotNull(vbaProject.Modules[x].Codes);
            wb.Save(Constants.destPath + &quot;CELLSNET54310.xlsm&quot;);
        }
```

### See Also

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


