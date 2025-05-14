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
// Called: int lc_Index = lc_NewWorkBook.VbaProject.Modules.Add(lc_NewWorkBook.Worksheets["Sheet1"]);
public void VbaModuleCollection_Method_Add()
{
    Workbook lc_WorkBook = new Workbook(Constants.sourcePath + "example.xlsm");
    Workbook lc_NewWorkBook = new Workbook();
    lc_NewWorkBook.Worksheets["Sheet1"].Copy(lc_WorkBook.Worksheets["Controls"]);


    //'VBAをコピーする
    int lc_Index = lc_NewWorkBook.VbaProject.Modules.Add(lc_NewWorkBook.Worksheets["Sheet1"]);
    lc_NewWorkBook.VbaProject.Modules[lc_Index].Codes = lc_WorkBook.VbaProject.Modules[lc_WorkBook.Worksheets["Controls"].CodeName].Codes;
   Assert.AreEqual("CommandButton1",lc_NewWorkBook.Worksheets[0].Shapes[0].Name);
    // 'ファイル名「Result.xlsm」で保存
    lc_NewWorkBook.Save(Constants.destPath + "example.xlsm", Aspose.Cells.SaveFormat.Xlsm);
    Assert.IsTrue(ManualFileUtil.ManualCheckStringInZip(Constants.destPath + "example.xlsm", "xl/worksheets/sheet1.xml", new string[] { "name=\"CommandButton1\"" }, true));
    Assert.IsTrue(ManualFileUtil.ManualCheckStringInZip(Constants.destPath + "example.xlsm", "xl/drawings/drawing1.xml", new string[] { "<xdr:cNvPr id=\"1027\"" }, true));
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
public static void VbaModuleCollection_Method_Add()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();

            // Initialize VBA project
            VbaProject vbaProject = workbook.VbaProject;

            // Add a new module
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "test");

            // Get the VBA module
            VbaModule vbaModule = vbaProject.Modules[index];

            // Set the codes for the module
            vbaModule.Codes = "Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub";

            // Saving the Excel file
            workbook.Save("VbaModuleExample.xlsm");
        }
```

### See Also

* enum [VbaModuleType](../../vbamoduletype/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


