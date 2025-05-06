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
// Called: wb.Settings.Password = &amp;quot;123456&amp;quot;;
private void Property_Password(Workbook wb, string fnTail)
        {
            wb.Settings.Password = &quot;123456&quot;;
            wb.Settings.WriteProtection.Password = &quot;234567&quot;;
            Util.SaveManCheck(wb, &quot;License&quot;, &quot;PluginLock&quot; + fnTail);
        }
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


