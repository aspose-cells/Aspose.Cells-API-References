---
title: "WorkbookSettings.DefaultStyleSettings"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Ruft die Einstellungen für Standardwerte der stilbezogenen Eigenschaften dieser Arbeitsmappe ab"
type: docs
url: /de/net/aspose.cells/workbooksettings/defaultstylesettings/
---
## WorkbookSettings.DefaultStyleSettings property

Liest die Einstellungen für Standardwerte von stilbezogenen Eigenschaften für dieses Workbook.

```csharp
public DefaultStyleSettings DefaultStyleSettings { get; }
```

### Beispiele

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDefaultStyleSettingsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greifen Sie auf die Standard-Stileinstellungen zu
            DefaultStyleSettings styleSettings = workbook.Settings.DefaultStyleSettings;

            // Legen Sie die integrierte Zahlenformatpräferenz fest
            styleSettings.BuiltInPreference = true;

            // Legen Sie die Kultur für die Zahlenformatierung fest
            workbook.Settings.CultureInfo = new CultureInfo("en-US");

            // Greifen Sie auf Zellen zu und wenden Sie Formatierungen an
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Werte und Formatierungen festlegen
            cells["A1"].PutValue(1234.56);
            cells["A1"].GetStyle().Number = 4; // Currency format

            cells["B1"].PutValue(0.456);
            cells["B1"].GetStyle().Number = 2; // Percentage format

            cells["C1"].PutValue(DateTime.Now);
            cells["C1"].GetStyle().Number = 22; // Short date format

            // Speichere die Arbeitsmappe
            workbook.Save("DefaultStyleSettingsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DefaultStyleSettings](../../defaultstylesettings/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


