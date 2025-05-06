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
        public void Property_CheckCustomNumberFormat()
        {
            Workbook workbook = new Workbook();
            Style style = workbook.CreateStyle();
            style.Custom = &quot;fff @ ggg&quot;;
            workbook.Settings.CheckCustomNumberFormat = true;
            style.Custom = &quot;fff @ ggg&quot;;
        }
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


