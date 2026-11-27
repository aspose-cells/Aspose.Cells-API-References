---
title: "Protection.Copy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Skyddmetod. Kopiera skyddsinformation"
type: docs
url: /sv/net/aspose.cells/protection/copy/
---
## Protection.Copy method

Kopiera skyddsinformation.

```csharp
public void Copy(Protection source)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| källa | Skydd |  |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectionMethodCopyWithProtectionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa källskyddsinställningar - använd befintligt skydd från arbetsbladet
            Protection sourceProtection = worksheet.Protection;
            sourceProtection.AllowDeletingColumn = true;
            sourceProtection.AllowInsertingRow = false;
            sourceProtection.Password = "test123";
            sourceProtection.AllowFormattingCell = true;

            // Hämta målskyddsinställningar
            Protection targetProtection = worksheet.Protection;

            try
            {
                // Anropa Copy-metoden med Protection-parameter
                targetProtection.Copy(sourceProtection);

                Console.WriteLine("Protection settings copied successfully.");
                Console.WriteLine($"Target protection - AllowDeletingColumn: {targetProtection.AllowDeletingColumn}");
                Console.WriteLine($"Target protection - AllowInsertingRow: {targetProtection.AllowInsertingRow}");
                Console.WriteLine($"Target protection - Password set: {!string.IsNullOrEmpty(targetProtection.Password)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error copying protection settings: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("ProtectionCopyDemo.xlsx");
        }
    }
}
```

### Se även

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


