---
title: VbaModuleCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: VbaModuleCollection method. Adds module for a worksheet
type: docs
url: /net/aspose.cells.vba/vbamodulecollection/add/
---
## Add(Worksheet) {#add_1}

Adds module for a worksheet.

```csharp
public int Add(Worksheet sheet)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sheet | Worksheet | The worksheet |

### Examples

```csharp
// Called: var index = wb.VbaProject.Modules.Add(wb.Worksheets[0]);
[Test]
        public void Method_Worksheet_()
        {
            Workbook wb = new Workbook();

            var vbaCode = "Private Sub Worksheet_SelectionChange(ByVal Target As Range)\r\n";
            vbaCode += "    ActiveCell.Value = \"Hello\"\r\n";
            vbaCode += "End Sub\r\n";

            var index = wb.VbaProject.Modules.Add(wb.Worksheets[0]);
            var module = wb.VbaProject.Modules[index];
            module.Name = "Sheet1";
            module.Codes = vbaCode;

            wb.VbaProject.Sign(bcCertSign);

            // Save the workbook
            wb.Save(Constants.destPath + "CELLSNET-45266_BC.xlsb", SaveFormat.Xlsb);
        }
```

### See Also

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)

---

## Add(VbaModuleType, string) {#add}

Adds module.

```csharp
public int Add(VbaModuleType type, string name)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | VbaModuleType | The type of module. |
| name | String | The name of module. |

### Examples

```csharp
// Called: int index = vbaProject.Modules.Add(VbaModuleType.Class, "test");
public static void Method_String_()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            
            // Init VBA project
            VbaProject vbaProject = workbook.VbaProject;
            
            // Add a new class module
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "test");
            
            // Get the VBA module
            VbaModule vbaModule = vbaProject.Modules[index];
            
            // Set codes for the module
            vbaModule.Codes = "Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub";
            
            // Save the Excel file
            workbook.Save("VbaModuleTypeExample.xlsm");
        }
```

### See Also

* enum [VbaModuleType](../../vbamoduletype/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


