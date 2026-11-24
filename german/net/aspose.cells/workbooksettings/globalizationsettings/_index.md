---
title: "WorkbookSettings.GlobalizationSettings"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Ruft die Globalisierungseinstellungen ab und legt sie fest"
type: docs
url: /de/net/aspose.cells/workbooksettings/globalizationsettings/
---
## WorkbookSettings.GlobalizationSettings property

Liest und setzt die Globalisierungseinstellungen.

```csharp
public GlobalizationSettings GlobalizationSettings { get; set; }
```

### Beispiele

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

            // Benutzerdefinierte Globalisierungseinstellungen festlegen
            wb.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            // Ergebnisse anzeigen
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

### Siehe auch

* class [GlobalizationSettings](../../globalizationsettings/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


