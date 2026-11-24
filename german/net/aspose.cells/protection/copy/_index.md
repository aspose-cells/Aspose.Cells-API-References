---
title: "Protection.Copy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Protection method. Kopiert Schutzinformationen"
type: docs
url: /de/net/aspose.cells/protection/copy/
---
## Protection.Copy method

Schutzinformationen kopieren.

```csharp
public void Copy(Protection source)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | Protection |  |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectionMethodCopyWithProtectionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie Quell-Schutz-Einstellungen – verwenden Sie den vorhandenen Schutz des Arbeitsblatts
            Protection sourceProtection = worksheet.Protection;
            sourceProtection.AllowDeletingColumn = true;
            sourceProtection.AllowInsertingRow = false;
            sourceProtection.Password = "test123";
            sourceProtection.AllowFormattingCell = true;

            // Ziel-Schutz-Einstellungen abrufen
            Protection targetProtection = worksheet.Protection;

            try
            {
                // Rufen Sie die Copy-Methode mit dem Protection-Parameter auf
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

            // Speichere die Arbeitsmappe
            workbook.Save("ProtectionCopyDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


