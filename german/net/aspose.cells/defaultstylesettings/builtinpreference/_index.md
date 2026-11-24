---
title: "DefaultStyleSettings.BuiltInPreference"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DefaultStyleSettings‑Eigenschaft. Gibt an, ob die Eigenschaft für das Zahlenformat vorzuziehen ist, wenn der Stil sowohl eingebaute Zahlen als auch ein benutzerdefiniertes Muster definiert. Der Standardwert ist false, was bedeutet, dass standardmäßig das benutzerdefinierte Muster verwendet wird, um Werte zu formatieren, solange es für einen Stil nicht leer ist."
type: docs
url: /de/net/aspose.cells/defaultstylesettings/builtinpreference/
---
## DefaultStyleSettings.BuiltInPreference property

Gibt an, ob die Eigenschaft für das Zahlenformat vorzuziehen ist, wenn der Stil sowohl integrierte Zahlen als auch ein benutzerdefiniertes Muster definiert. Der Standardwert ist false, das bedeutet, dass standardmäßig das benutzerdefinierte Muster verwendet wird, um Werte zu formatieren, solange es für einen Stil nicht leer ist.

```csharp
public bool BuiltInPreference { get; set; }
```

### Hinweise

Beim Laden einer Arbeitsmappe aus einer vorhandenen Vorlagendatei können für einen Stil sowohl eingebaute Zahlen als auch ein benutzerdefiniertes Muster definiert sein. Diese Eigenschaft bestimmt, ob beim Formatieren von Werten mit dem Stil die eingebaute Zahl oder das benutzerdefinierte Muster verwendet werden soll.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyBuiltInPreferenceDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Zugriff auf die Standard‑Stileinstellungen
            DefaultStyleSettings defaultStyleSettings = workbook.Settings.DefaultStyleSettings;

            // BuiltInPreference‑Eigenschaft demonstrieren
            defaultStyleSettings.BuiltInPreference = false;
            defaultStyleSettings.FontName = "Arial";
            defaultStyleSettings.FontSize = 12;

            // Auf das Arbeitsblatt anwenden
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Text");
            
            // Speichere die Arbeitsmappe
            workbook.Save("BuiltInPreferenceDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


