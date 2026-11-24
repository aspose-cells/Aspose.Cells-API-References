---
title: "AbstractLowCodeProtectionProvider.GetWritePassword"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AbstractLowCodeProtectionProvider-Methode. Gibt das Passwort zurück, um die Tabellendatei zu ändern"
type: docs
url: /de/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getwritepassword/
---
## AbstractLowCodeProtectionProvider.GetWritePassword method

Liefert das Passwort zum Ändern der Tabellendatei.

```csharp
public virtual string GetWritePassword()
```

### Rückgabewert

Passwort zum Ändern der Tabellendatei. Leer bedeutet, dass keine Schutz für das Ändern der Datei besteht.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetWritePasswordDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Erstelle eine benutzerdefinierte Instanz des Schutz-Providers
            var protectionProvider = new CustomProtectionProvider();

            try
            {
                // Rufe GetWritePassword explizit auf und zeige das Ergebnis an
                string writePassword = protectionProvider.GetWritePassword();
                Console.WriteLine($"Retrieved write password: {writePassword}");

                // Speichere das Arbeitsbuch – wende den Schreibschutz direkt an
                workbook.Settings.WriteProtection.Password = writePassword;
                workbook.Save("MethodGetWritePasswordDemo.xlsx");
                Console.WriteLine("Workbook saved with write protection password.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetWritePassword method: {ex.Message}");
            }
        }

    }

    // Benutzerdefinierte Implementierung des Schutzanbieters
    public class CustomProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public override string GetWritePassword()
        {
            return "AsposeTestPassword123!";
        }

        // Implementiere weitere erforderliche Methoden mit Standardrückgaben
        public override string GetOpenPassword() => null;
        public override string GetWorkbookPassword() => null;
        public override ProtectionType GetWorkbookProtectionType() => ProtectionType.None;
        public override string GetWorksheetPassword(string sheetName) => null;
        public override ProtectionType GetWorksheetProtectionType(string sheetName) => ProtectionType.None;
    }
}
```

### Siehe auch

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


