---
title: "Protection.Password"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Protection-egenskap. Representerar lösenordet för att skydda kalkylbladet"
type: docs
url: /sv/net/aspose.cells/protection/password/
---
## Protection.Password property

Representerar lösenordet för att skydda kalkylbladet.

```csharp
public string Password { get; set; }
```

### Anmärkningar

Om lösenordet är satt till null eller en tom sträng kan du avskydda kalkylbladet eller arbetsboken utan att använda ett lösenord. Annars måste du ange lösenordet för att avskydda kalkylbladet eller arbetsboken.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyPasswordDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ställ in skyddsinställningar med lösenord
            Protection protection = worksheet.Protection;
            protection.AllowEditingContent = false;
            protection.AllowDeletingColumn = false;
            protection.Password = "test123";

            // Verifiera lösenordsskydd
            Console.WriteLine("Worksheet is protected: " + (protection.Password != null));
            Console.WriteLine("Protection password: " + protection.Password);

            // Skapa ett annat skyddsobjekt för jämförelse
            Protection protection2 = worksheet.Protection;
            protection2.Password = "test123";

            // Jämför lösenordsskydd
            Console.WriteLine("Passwords match: " + (protection.Password == protection2.Password));
        }
    }
}
```

### Se även

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


