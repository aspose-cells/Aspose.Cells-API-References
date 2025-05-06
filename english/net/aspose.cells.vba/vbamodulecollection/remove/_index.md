---
title: VbaModuleCollection.Remove
second_title: Aspose.Cells for .NET API Reference
description: VbaModuleCollection method. Removes module for a worksheet
type: docs
url: /net/aspose.cells.vba/vbamodulecollection/remove/
---
## Remove(Worksheet) {#remove}

Removes module for a worksheet.

```csharp
public void Remove(Worksheet sheet)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sheet | Worksheet | The worksheet |

### See Also

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)

---

## Remove(string) {#remove_1}

Remove the module by the name

```csharp
public void Remove(string name)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String |  |

### Examples

```csharp
// Called: vbaProject.Modules.Remove(&amp;quot;TestForm&amp;quot;);
[Test]
        public void Method_String_()
        {
            var source = new Workbook(Constants.sourcePath + &quot;CELLSNET54310.xlsm&quot;);
            var wb = new Workbook(Constants.sourcePath + &quot;CELLSNET54310.xlsm&quot;);
            VbaProject vbaProject = wb.VbaProject;
            vbaProject.Modules.Remove(&quot;TestForm&quot;);
            Assert.IsNull(vbaProject.Modules.GetDesignerStorage(&quot;TestForm&quot;));
            vbaProject.Modules.AddDesignerStorage(&quot;TestForm&quot;, source.VbaProject.Modules.GetDesignerStorage(&quot;TestForm&quot;));
            int index = vbaProject.Modules.Add(VbaModuleType.Designer, &quot;TestForm&quot;);
            vbaProject.Modules[index].Codes = source.VbaProject.Modules[&quot;TestForm&quot;].Codes;
            wb.Save(Constants.destPath + &quot;CELLSNET54310.xlsm&quot;);
        }
```

### See Also

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


