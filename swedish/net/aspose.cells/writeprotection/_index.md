---
title: "Klassen WriteProtection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.WriteProtection-klass. Anger skrivskyddsinställningar för en arbetsbok"
type: docs
url: /sv/net/aspose.cells/writeprotection/
---
## WriteProtection class

Anger skrivskyddsinställningar för en arbetsbok.

```csharp
public class WriteProtection
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Author](../../aspose.cells/writeprotection/author/) { get; set; } | Hämtar och anger författaren. |
| [IsWriteProtected](../../aspose.cells/writeprotection/iswriteprotected/) { get; } | Anger om den här arbetsboken är skrivskyddad. |
| [Password](../../aspose.cells/writeprotection/password/) { get; set; } | Anger det skyddade lösenordet för att ändra filen. |
| [RecommendReadOnly](../../aspose.cells/writeprotection/recommendreadonly/) { get; set; } | Anger om alternativet Läs endast rekommenderat är valt. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [ValidatePassword](../../aspose.cells/writeprotection/validatepassword/)(string) | Returnerar true om det angivna lösenordet är samma som skrivskyddslösenordet som filen skyddades med. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WriteProtectionDemo
    {
        public static void WriteProtectionExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till arbetsbokens inställningar
            WorkbookSettings settings = workbook.Settings;

            // Åtkomst till skrivskyddsinställningarna
            WriteProtection writeProtection = settings.WriteProtection;

            // Ange författaren för skrivskyddet
            writeProtection.Author = "John Doe";

            // Ange lösenordet för skrivskyddet
            writeProtection.Password = "password123";

            // Ange det rekommenderade skrivskyddsalternativet
            writeProtection.RecommendReadOnly = true;

            // Kontrollera om arbetsboken är skrivskyddad
            bool isWriteProtected = writeProtection.IsWriteProtected;
            Console.WriteLine("Is Write Protected: " + isWriteProtected);

            // Validera lösenordet
            bool isValidPassword = writeProtection.ValidatePassword("password123");
            Console.WriteLine("Is Valid Password: " + isValidPassword);

            // Spara arbetsboken
            workbook.Save("WriteProtectionExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


