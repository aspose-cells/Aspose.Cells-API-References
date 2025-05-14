---
title: WorkbookSettings.CheckCustomNumberFormat
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Indicates whether checking custom number format when setting Style.Custom
type: docs
url: /net/aspose.cells/workbooksettings/checkcustomnumberformat/
---
## WorkbookSettings.CheckCustomNumberFormat property

Indicates whether checking custom number format when setting Style.Custom.

```csharp
public bool CheckCustomNumberFormat { get; set; }
```

### Examples

```csharp
// Called: workbook.Settings.CheckCustomNumberFormat = true;
[Test, ExpectedException(typeof(CellsException))]
#endif
        public void WorkbookSettings_Property_CheckCustomNumberFormat()
        {
            Workbook workbook = new Workbook();
            Style style = workbook.CreateStyle();
            style.Custom = "fff @ ggg";
            workbook.Settings.CheckCustomNumberFormat = true;
            style.Custom = "fff @ ggg";
        }
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


