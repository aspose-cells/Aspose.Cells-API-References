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
// Called: vbaProject.Modules.AddDesignerStorage("TestForm", source.VbaProject.Modules.GetDesignerStorage("TestForm"));
[Test]
        public void Method_String_()
        {
            var source = new Workbook(Constants.sourcePath + "CELLSNET54310.xlsm");
            var wb = new Workbook(Constants.sourcePath + "CELLSNET54310.xlsm");
            VbaProject vbaProject = wb.VbaProject;
            vbaProject.Modules.Remove("TestForm");
            Assert.IsNull(vbaProject.Modules.GetDesignerStorage("TestForm"));
            vbaProject.Modules.AddDesignerStorage("TestForm", source.VbaProject.Modules.GetDesignerStorage("TestForm"));
            int index = vbaProject.Modules.Add(VbaModuleType.Designer, "TestForm");
            vbaProject.Modules[index].Codes = source.VbaProject.Modules["TestForm"].Codes;
            wb.Save(Constants.destPath + "CELLSNET54310.xlsm");
        }
```

### See Also

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


