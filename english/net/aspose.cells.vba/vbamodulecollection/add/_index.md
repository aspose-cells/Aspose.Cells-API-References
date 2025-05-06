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
// Called: idx = workbook.VbaProject.Modules.Add(worksheet);
[Test]
        public void Method_Worksheet_()
        {
           

            Workbook workbook = new Workbook(Constants.sourcePath +&quot;CellsNet43614.xlsm&quot;);


            int idx;

            Worksheet worksheet = null;

            VbaModule mod = null;


            //Set One

            idx = workbook.Worksheets.AddCopy(1);


            worksheet = workbook.Worksheets[idx];


            idx = workbook.VbaProject.Modules.Add(worksheet);


            mod = workbook.VbaProject.Modules[idx];

            mod.Name = &quot;newNameString&quot;;


            //Set Two

            idx = workbook.Worksheets.AddCopy(1);


            worksheet = workbook.Worksheets[idx];


            idx = workbook.VbaProject.Modules.Add(worksheet);


            mod = workbook.VbaProject.Modules[idx];

            mod.Name = &quot;newNameString2&quot;;


            //This will throw exception

            workbook.Save(Constants.destPath + &quot;CellsNet43614.xlsm&quot;);
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
// Called: int index = vbaProject.Modules.Add(VbaModuleType.Class, &amp;quot;test&amp;quot;);
public static void Method_String_()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();

            // Initialize VBA project
            VbaProject vbaProject = workbook.VbaProject;

            // Add a new module
            int index = vbaProject.Modules.Add(VbaModuleType.Class, &quot;test&quot;);

            // Get the VBA module
            VbaModule vbaModule = vbaProject.Modules[index];

            // Set the codes for the module
            vbaModule.Codes = &quot;Sub ShowMessage()\r\nMsgBox \&quot;Welcome to Aspose!\&quot;\r\nEnd Sub&quot;;

            // Saving the Excel file
            workbook.Save(&quot;VbaModuleExample.xlsm&quot;);
        }
```

### See Also

* enum [VbaModuleType](../../vbamoduletype/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


