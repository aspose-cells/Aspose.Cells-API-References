---
title: "LoadOptions.Password"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LoadOptions-Eigenschaft. Liest und setzt das Passwort der Arbeitsmappe"
type: docs
url: /de/net/aspose.cells/loadoptions/password/
---
## LoadOptions.Password property

Liest und legt das Passwort der Arbeitsmappe fest.

```csharp
public string Password { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyPasswordDemo
    {
        public static void Run()
        {
            // Ladeoptionen erstellen und Passwort setzen
            LoadOptions options = new LoadOptions();
            options.Password = "test";

            // Passwortgeschützte Arbeitsmappe laden
            Workbook workbook = new Workbook("protected.xlsx", options);

            // Passwortschutz nach dem Laden entfernen
            workbook.Settings.Password = null;

            // Das ungeschützte Arbeitsbuch speichern
            workbook.Save("unprotected.xlsx");
        }
    }
}
```

### Siehe auch

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


