---
title: "ProtectedRange.Password"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ProtectedRange-egenskap. Representerar lösenordet för att skydda området"
type: docs
url: /sv/net/aspose.cells/protectedrange/password/
---
## ProtectedRange.Password property

Representerar lösenordet för att skydda området.

```csharp
public string Password { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangePropertyPasswordDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa samling av skyddade områden
            ProtectedRangeCollection allowRanges = worksheet.AllowEditRanges;

            // Lägg till ett skyddat område
            int index = allowRanges.Add("MyProtectedRange", 0, 0, 2, 2);
            ProtectedRange protectedRange = allowRanges[index];

            // Ange lösenord för det skyddade området
            protectedRange.Password = "12345";

            // Spara arbetsboken
            workbook.Save("ProtectedRangeWithPassword.xlsx");
        }
    }
}
```

### Se även

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


