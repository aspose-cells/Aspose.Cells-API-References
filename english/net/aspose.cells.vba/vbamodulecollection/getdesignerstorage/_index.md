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
// Called: Assert.IsNull(vbaProject.Modules.GetDesignerStorage("TestForm"));
public void VbaModuleCollection_Method_GetDesignerStorage()
{
    var source = new Workbook(Constants.sourcePath + "example.xlsm");
    var wb = new Workbook(Constants.sourcePath + "example.xlsm");
    VbaProject vbaProject = wb.VbaProject;
    vbaProject.Modules.Remove("TestForm");
    Assert.IsNull(vbaProject.Modules.GetDesignerStorage("TestForm"));
    vbaProject.Modules.AddDesignerStorage("TestForm", source.VbaProject.Modules.GetDesignerStorage("TestForm"));
    int index = vbaProject.Modules.Add(VbaModuleType.Designer, "TestForm");
    vbaProject.Modules[index].Codes = source.VbaProject.Modules["TestForm"].Codes;
    wb.Save(Constants.destPath + "example.xlsm");
}
```

### See Also

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


