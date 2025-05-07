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
// Called: int x =  vbaProject.Modules.AddUserForm("TestForm", source.VbaProject.Modules["TestForm"].Codes, source.VbaProject.Modules.GetDesignerStorage("TestForm"));
[Test]
        public void Property_Codes()
        {
            var source = new Workbook(Constants.sourcePath + "CELLSNET54310.xlsm");
            var wb = new Workbook(Constants.sourcePath + "CELLSNET54310.xlsm");
            VbaProject vbaProject = wb.VbaProject;
           int x =  vbaProject.Modules.AddUserForm("TestForm", source.VbaProject.Modules["TestForm"].Codes, source.VbaProject.Modules.GetDesignerStorage("TestForm"));
            Assert.IsNotNull(vbaProject.Modules.GetDesignerStorage("TestForm"));
            Assert.IsNotNull(vbaProject.Modules[x].Codes);
            wb.Save(Constants.destPath + "CELLSNET54310.xlsm");
        }
```

### See Also

* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


