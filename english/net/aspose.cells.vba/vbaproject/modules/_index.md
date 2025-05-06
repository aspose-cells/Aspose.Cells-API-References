---
title: VbaProject.Modules
second_title: Aspose.Cells for .NET API Reference
description: VbaProject property. Gets all VbaModule objects
type: docs
url: /net/aspose.cells.vba/vbaproject/modules/
---
## VbaProject.Modules property

Gets all [`VbaModule`](../../vbamodule/) objects.

```csharp
public VbaModuleCollection Modules { get; }
```

### Examples

```csharp
// Called: workbook.VbaProject.Modules[i].Codes += &amp;quot; &amp;apos;&amp;quot; + i.ToString() + &amp;quot; &amp;quot;;
[Test]
        public void Property_Modules()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET43891.xlsm&quot;);
            Console.WriteLine(&quot;Before Deleting Sheet &amp; Module: &quot; + &quot;workbook.Worksheets.Count: &quot; + workbook.Worksheets.Count.ToString() + &quot;workbook.VbaProject.Modules.Count: &quot; + workbook.VbaProject.Modules.Count.ToString());
            workbook.Worksheets.RemoveAt(workbook.Worksheets.Count - 1);
            workbook.VbaProject.Modules.RemoveAt(workbook.VbaProject.Modules.Count - 1);
            Console.WriteLine(&quot;After Deleting Sheet &amp; Module: &quot; + &quot;workbook.Worksheets.Count: &quot; + workbook.Worksheets.Count.ToString() + &quot;workbook.VbaProject.Modules.Count: &quot; + workbook.VbaProject.Modules.Count.ToString());

            Console.WriteLine(&quot;Before Adding Sheet &amp; Module: &quot; + &quot;workbook.Worksheets.Count: &quot; + workbook.Worksheets.Count.ToString() + &quot;workbook.VbaProject.Modules.Count: &quot; + workbook.VbaProject.Modules.Count.ToString());
            workbook.VbaProject.Modules.Add(workbook.Worksheets.Add(&quot;TestSheet&quot;));
            Console.WriteLine(&quot;After Adding Sheet &amp; Module: &quot; + &quot;workbook.Worksheets.Count: &quot; + workbook.Worksheets.Count.ToString() + &quot;workbook.VbaProject.Modules.Count: &quot; + workbook.VbaProject.Modules.Count.ToString());
            for (int i = 0; i &lt;= workbook.VbaProject.Modules.Count - 1; i++)
            {
                workbook.VbaProject.Modules[i].Codes += &quot; &apos;&quot; + i.ToString() + &quot; &quot;;
            }
            workbook.Save(Constants.destPath + &quot;CELLSNET43891.xlsm&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET43891.xlsm&quot;);
            Assert.AreEqual(&quot;Sheet1&quot;, workbook.Worksheets[0].CodeName);
        }
```

### See Also

* class [VbaModuleCollection](../../vbamodulecollection/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


