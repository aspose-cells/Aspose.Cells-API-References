---
title: VbaModule.Name
second_title: Aspose.Cells for .NET API Reference
description: VbaModule property. Gets and sets the name of Module
type: docs
url: /net/aspose.cells.vba/vbamodule/name/
---
## VbaModule.Name property

Gets and sets the name of Module.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: module.Name = "Sheet1";
public void VbaModule_Property_Name()
{
    Workbook wb = new Workbook();

    var vbaCode = "Private Sub Worksheet_SelectionChange(ByVal Target As Range)\r\n";
    vbaCode += "    ActiveCell.Value = \"Hello\"\r\n";
    vbaCode += "End Sub\r\n";

    var index = wb.VbaProject.Modules.Add(wb.Worksheets[0]);
    var module = wb.VbaProject.Modules[index];
    module.Name = "Sheet1";
    module.Codes = vbaCode;

    wb.VbaProject.Sign(certSign);

    // Save the workbook
    wb.Save(new MemoryStream(), SaveFormat.Xlsb);
}
```

### See Also

* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


