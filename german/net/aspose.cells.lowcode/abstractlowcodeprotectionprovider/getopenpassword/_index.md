---
title: "AbstractLowCodeProtectionProvider.GetOpenPassword"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AbstractLowCodeProtectionProvider-Methode. Gibt das Passwort zum Öffnen der Tabellendatei zurück"
type: docs
url: /de/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getopenpassword/
---
## AbstractLowCodeProtectionProvider.GetOpenPassword method

Liefert das Passwort zum Öffnen der Tabellendatei.

```csharp
public virtual string GetOpenPassword()
```

### Rückgabewert

Passwort zum Öffnen der Tabellendatei. Empty bedeutet, dass keine Schutz für das Öffnen der Datei besteht.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetOpenPasswordDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle eine Instanz des Schutzanbieters
                var protectionProvider = new DemoProtectionProvider();

                // Rufe die Methode GetOpenPassword auf, um das Passwort abzurufen
                string password = protectionProvider.GetOpenPassword();

                // Erstelle ein neues Arbeitsbuch und wende das Passwort an
                Workbook workbook = new Workbook("sample.xlsx");
                workbook.Settings.Password = password;

                // Speichere das passwortgeschützte Arbeitsbuch
                workbook.Save("MethodGetOpenPasswordDemo.xlsx");

                Console.WriteLine($"Workbook protected with open password: {password}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing demo: {ex.Message}");
            }
        }
    }

    public class DemoProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public override string GetOpenPassword()
        {
            return "AsposeDemo123!";
        }
    }
}
```

### Siehe auch

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


