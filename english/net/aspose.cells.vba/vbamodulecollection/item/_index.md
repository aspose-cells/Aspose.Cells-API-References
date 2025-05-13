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
// Called: Assert.AreEqual("Sheet6", workbook.VbaProject.Modules[6].Name);
public void VbaModuleCollection_Property_Item()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Assert.AreEqual("Sheet6", workbook.VbaProject.Modules[6].Name);
    workbook.Save(Constants.destPath + "example.xlsx");
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
// Called: int x =  vbaProject.Modules.AddUserForm("TestForm", source.VbaProject.Modules["TestForm"].Codes, source.VbaProject.Modules.GetDesignerStorage("TestForm"));
public void VbaModuleCollection_Property_Item()
{
    var source = new Workbook(Constants.sourcePath + "example.xlsm");
    var wb = new Workbook(Constants.sourcePath + "example.xlsm");
    VbaProject vbaProject = wb.VbaProject;
   int x =  vbaProject.Modules.AddUserForm("TestForm", source.VbaProject.Modules["TestForm"].Codes, source.VbaProject.Modules.GetDesignerStorage("TestForm"));
    Assert.IsNotNull(vbaProject.Modules.GetDesignerStorage("TestForm"));
    Assert.IsNotNull(vbaProject.Modules[x].Codes);
    wb.Save(Constants.destPath + "example.xlsm");
}
```

### See Also

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


