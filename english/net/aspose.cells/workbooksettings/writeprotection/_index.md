---
title: WorkbookSettings.WriteProtection
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Provides access to the workbook write protection options
type: docs
url: /net/aspose.cells/workbooksettings/writeprotection/
---
## WorkbookSettings.WriteProtection property

Provides access to the workbook write protection options.

```csharp
public WriteProtection WriteProtection { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;abc&amp;quot;, workbook.Settings.WriteProtection.Author);
[Test]
        public void Property_WriteProtection()
        {

            Workbook workbook = new Workbook();

            workbook.Settings.WriteProtection.Password = &quot;test&quot;;
            workbook.Settings.WriteProtection.Author = &quot;abc&quot;;
            workbook.Save(Constants.destPath + &quot;WriteProtection1.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;WriteProtection1.xlsx&quot;);
            Assert.AreEqual(&quot;abc&quot;, workbook.Settings.WriteProtection.Author);

        }
```

### See Also

* class [WriteProtection](../../writeprotection/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


