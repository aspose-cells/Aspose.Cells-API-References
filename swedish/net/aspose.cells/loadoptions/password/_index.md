---
title: "LoadOptions.Password"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LoadOptions-egenskap. Hämtar och sätter lösenordet för arbetsboken"
type: docs
url: /sv/net/aspose.cells/loadoptions/password/
---
## LoadOptions.Password property

Hämtar och anger lösenordet för Workbook.

```csharp
public string Password { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyPasswordDemo
    {
        public static void Run()
        {
            // Skapa inläsningsalternativ och ange lösenordet
            LoadOptions options = new LoadOptions();
            options.Password = "test";

            // Läs in lösenordsskyddad arbetsbok
            Workbook workbook = new Workbook("protected.xlsx", options);

            // Ta bort lösenordsskyddet efter inläsning
            workbook.Settings.Password = null;

            // Spara den oskyddade arbetsboken
            workbook.Save("unprotected.xlsx");
        }
    }
}
```

### Se även

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


