---
title: Workbook.VbaProject
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets the VbaProject in a spreadsheet
type: docs
url: /net/aspose.cells/workbook/vbaproject/
---
## Workbook.VbaProject property

Gets the `VbaProject` in a spreadsheet.

```csharp
public VbaProject VbaProject { get; }
```

### Examples

```csharp
// Called: var index = workbook.VbaProject.Modules.Add(VbaModuleType.Class, Path.GetFileNameWithoutExtension(resourceName));
private static void Workbook_Property_VbaProject(Workbook workbook, string resourceName)
        {
            //File.WriteAllText(@"D:\Filetemp\d.txt", workbook.VbaProject.Modules[0].Codes);
            //  var moduleType = GetModuleType(resourceName);
            var index = workbook.VbaProject.Modules.Add(VbaModuleType.Class, Path.GetFileNameWithoutExtension(resourceName));
            var module = workbook.VbaProject.Modules[index];
            module.Codes = File.ReadAllText(Constants.sourcePath + resourceName);
        }
```

### See Also

* class [VbaProject](../../../aspose.cells.vba/vbaproject/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


