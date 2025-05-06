---
title: VbaModuleCollection.GetDesignerStorage
second_title: Aspose.Cells for .NET API Reference
description: VbaModuleCollection method. Represents the data of Designer
type: docs
url: /net/aspose.cells.vba/vbamodulecollection/getdesignerstorage/
---
## VbaModuleCollection.GetDesignerStorage method

Represents the data of Designer.

```csharp
public byte[] GetDesignerStorage(string name)
```

### Remarks

We do not support to parse them. Just only for copying.

### Examples

```csharp
// Called: Assert.IsNull(vbaProject.Modules.GetDesignerStorage(&amp;quot;TestForm&amp;quot;));
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


