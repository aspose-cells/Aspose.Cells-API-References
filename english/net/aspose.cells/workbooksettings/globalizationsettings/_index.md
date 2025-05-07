---
title: WorkbookSettings.GlobalizationSettings
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets and sets the globalization settings
type: docs
url: /net/aspose.cells/workbooksettings/globalizationsettings/
---
## WorkbookSettings.GlobalizationSettings property

Gets and sets the globalization settings.

```csharp
public GlobalizationSettings GlobalizationSettings { get; set; }
```

### Examples

```csharp
// Called: wb.Settings.GlobalizationSettings = new RaGlobalization();
[Test]
        public void Property_GlobalizationSettings()
        { //CELLSNET-45437
            Workbook wb = new Workbook();
            string[] errs = new string[]{"#NAME?", "#DIV/0!", "#REF!", "#VALUE!", "#N/A", "#NUM!", "#NULL!"};
            Cells cells = wb.Worksheets[0].Cells;
            cells[0, 0].PutValue(true);
            cells[0, 1].PutValue(false);
            for (int i = 0; i < errs.Length; i++)
            {
                cells[0, i+2].PutValue(errs[i]);
            }
            wb.Settings.GlobalizationSettings = new RaGlobalization();
            string[] expected = new string[] { "ИСТИНА", "ЛОЖЬ", "#ИМЯ?", "#ДЕЛ/0!", "#ССЫЛКА!", "#ЗНАЧ!", "#Н/Д", "#ЧИСЛО!", "#ПУСТО!" };
            for (int i = 0; i < expected.Length; i++)
            {
                Assert.AreEqual(expected[i], cells[0, i].StringValue, cells[0, i].Value.ToString());
            }
        }
```

### See Also

* class [GlobalizationSettings](../../globalizationsettings/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


