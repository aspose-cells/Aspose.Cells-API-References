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
// Called: vbaProject.Modules.Remove("TestForm");
public void VbaModuleCollection_Method_Remove()
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


