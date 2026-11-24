---
title: "SettableGlobalizationSettings.ListSeparator"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableGlobalizationSettings-Eigenschaft. Gibt das Trennzeichen für Listenparameter von Funktionen ...usw zurück"
type: docs
url: /de/net/aspose.cells/settableglobalizationsettings/listseparator/
---
## SettableGlobalizationSettings.ListSeparator property

Liest das Trennzeichen für Listen, Funktionsparameter, ...usw.

```csharp
public override char ListSeparator { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsPropertyListSeparatorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle eine Instanz von SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Zeigen Sie den aktuellen ListSeparator-Wert an (Standard ist Komma in den meisten Gebietsschemas)
            Console.WriteLine("Current ListSeparator value: " + settings.ListSeparator);
            
            // Legen Sie einen neuen ListSeparator-Wert fest (z. B. Semikolon)
            settings.SetListSeparator(';');
            
            // Wenden Sie die Einstellungen auf die Arbeitsmappe an
            workbook.Settings.GlobalizationSettings = settings;
            
            // Demonstrieren Sie die Wirkung von ListSeparator beim Parsen von Formeln
            worksheet.Cells["A1"].PutValue("Test");
            worksheet.Cells["A2"].PutValue("Data");
            
            // Erstellen Sie eine Formel, die das ListSeparator verwendet
            worksheet.Cells["A3"].Formula = "=CONCATENATE(A1,A2)";
            
            // Die Formel verwendet das benutzerdefinierte ListSeparator beim Parsen
            Console.WriteLine("Formula with custom separator: " + worksheet.Cells["A3"].Formula);
            
            // Speichere die Arbeitsmappe
            workbook.Save("PropertyListSeparatorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


