---
title: WorkbookSettings.Password
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Represents Workbook file encryption password
type: docs
url: /net/aspose.cells/workbooksettings/password/
---
## WorkbookSettings.Password property

Represents Workbook file encryption password.

```csharp
public string Password { get; set; }
```

### Examples

```csharp
// Called: workbook.Settings.Password = "1";
[Test]
        public void Property_Password()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET-43921.xlsx");
            Util.SaveForViewer(workbook, "13", "CellsNet43921.xlsb");
            workbook = new Workbook(Constants.sourcePath + "CELLSNET-44218.xlsx");
            Util.SaveForViewer(workbook, "13", "CELLSNET-44218.xlsx");
            workbook = new Workbook(Constants.sourcePath + "CELLSNET-44222.xlsm");
            Util.SaveForViewer(workbook, "13", "CELLSNET-44222.xlsm");
            workbook = new Workbook(Constants.sourcePath + "CELLSNET-44220.xlsx");
            workbook.Settings.Password = "1"; 
            Util.SaveForViewer(workbook, "13", "CELLSNET-44220.xlsx");
            workbook = new Workbook(Constants.sourcePath + "CELLSNET-44231.xlsx");
            Util.SaveForViewer(workbook, "13", "CELLSNET-44231.xlsx");

        }
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


