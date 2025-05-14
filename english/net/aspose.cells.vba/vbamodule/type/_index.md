---
title: VbaModule.Type
second_title: Aspose.Cells for .NET API Reference
description: VbaModule property. Gets the type of module
type: docs
url: /net/aspose.cells.vba/vbamodule/type/
---
## VbaModule.Type property

Gets the type of module.

```csharp
public VbaModuleType Type { get; }
```

### Examples

```csharp
// Called: Console.WriteLine(lModules[i].Type);
public void VbaModule_Property_Type()
 {

     Workbook wb = new Workbook(Constants.sourcePath + "example.xlsm");
     VbaProject lVbaProject = wb.VbaProject;
     VbaModuleCollection lModules = lVbaProject.Modules;
     for (int i = 0; i < lModules.Count; i++)
     {
        string name = lModules[i].Name;
         Console.WriteLine(lModules[i].Type);
         string codes = lModules[i].Codes;
     }
     wb.Save(Constants.destPath + "example.xlsm");
 }
```

### See Also

* enum [VbaModuleType](../../vbamoduletype/)
* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


