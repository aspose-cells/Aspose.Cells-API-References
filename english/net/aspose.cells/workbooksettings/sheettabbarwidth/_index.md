---
title: WorkbookSettings.SheetTabBarWidth
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Width of worksheet tab bar in 1/1000 of window width
type: docs
url: /net/aspose.cells/workbooksettings/sheettabbarwidth/
---
## WorkbookSettings.SheetTabBarWidth property

Width of worksheet tab bar (in 1/1000 of window width).

```csharp
public int SheetTabBarWidth { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Settings.SheetTabBarWidth, 1000);
[Test]
        public void Property_SheetTabBarWidth()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET43086.ods&quot;);

            Assert.AreEqual(workbook.Settings.SheetTabBarWidth, 1000);
            workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET43087.ods&quot;);

            Assert.AreEqual(workbook.Settings.SheetTabBarWidth, 1000);
        }
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


