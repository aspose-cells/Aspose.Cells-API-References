---
title: VbaModule.Codes
second_title: Aspose.Cells for .NET API Reference
description: VbaModule property. Gets and sets the codes of module
type: docs
url: /net/aspose.cells.vba/vbamodule/codes/
---
## VbaModule.Codes property

Gets and sets the codes of module.

```csharp
public string Codes { get; set; }
```

### Examples

```csharp
// Called: module.Codes = (code + "\n" +
public void VbaModule_Property_Codes()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    VbaModuleCollection modules = workbook.VbaProject.Modules;
    bool hasFinalMacros = false;
    for (int i = 0; i < modules.Count; i++)
    {
        VbaModule module = modules[i];
        String code = module.Codes;
        if (code.ToLower().Contains("finalmacros"))
        {
            module.Codes = (code + "\n" +
                    "Private Sub Auto_open()\n" +
                    " Call FinalMacros\n" +
                    "End Sub");
            break;
        }
    }
    Util.SaveManCheck(workbook, "Shape", "example.xls");


}
```

### See Also

* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


