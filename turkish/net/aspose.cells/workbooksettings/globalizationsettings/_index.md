---
title: "WorkbookSettings.GlobalizationSettings"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Küreselleştirme ayarlarını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/workbooksettings/globalizationsettings/
---
## WorkbookSettings.GlobalizationSettings property

Küreselleştirme ayarlarını alır ve ayarlar.

```csharp
public GlobalizationSettings GlobalizationSettings { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyGlobalizationSettingsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            string[] errs = new string[] { "#NAME?", "#DIV/0!", "#REF!", "#VALUE!", "#N/A", "#NUM!", "#NULL!" };
            Cells cells = wb.Worksheets[0].Cells;
            
            cells[0, 0].PutValue(true);
            cells[0, 1].PutValue(false);
            
            for (int i = 0; i < errs.Length; i++)
            {
                cells[0, i + 2].PutValue(errs[i]);
            }

            // Özel küreselleştirme ayarlarını ayarla
            wb.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            // Sonuçları göster
            for (int i = 0; i < 9; i++)
            {
                Console.WriteLine($"Cell[0,{i}]: {cells[0, i].StringValue}");
            }
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetBooleanValueString(bool bv)
        {
            return bv ? "ИСТИНА" : "ЛОЖЬ";
        }

        public override string GetErrorValueString(string err)
        {
            switch (err)
            {
                case "#NAME?": return "#ИМЯ?";
                case "#DIV/0!": return "#ДЕЛ/0!";
                case "#REF!": return "#ССЫЛКА!";
                case "#VALUE!": return "#ЗНАЧ!";
                case "#N/A": return "#Н/Д";
                case "#NUM!": return "#ЧИСЛО!";
                case "#NULL!": return "#ПУСТО!";
                default: return base.GetErrorValueString(err);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [GlobalizationSettings](../../globalizationsettings/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


