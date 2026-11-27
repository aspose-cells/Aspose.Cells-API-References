---
title: "AbstractLowCodeProtectionProvider.GetWritePassword"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractLowCodeProtectionProvider-metod. Hämtar lösenordet för att ändra kalkylbladsfilen"
type: docs
url: /sv/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getwritepassword/
---
## AbstractLowCodeProtectionProvider.GetWritePassword method

Hämtar lösenordet för att ändra kalkylbladsfilen.

```csharp
public virtual string GetWritePassword()
```

### Returvärde

Lösenord för att ändra kalkylbladsfilen. Tom betyder att det inte finns något skydd för att ändra filen.

### Exempel

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
            
            // Skapa en instans av anpassad skyddsleverantör
            var protectionProvider = new CustomProtectionProvider();

            try
            {
                // Anropa explicit GetWritePassword och visa resultatet
                string writePassword = protectionProvider.GetWritePassword();
                Console.WriteLine($"Retrieved write password: {writePassword}");

                // Spara arbetsboken – tillämpa skrivskydd direkt
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

    // Anpassad skyddsleverantörsimplementation
    public class CustomProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public override string GetWritePassword()
        {
            return "AsposeTestPassword123!";
        }

        // Implementera övriga obligatoriska metoder med standardvärden
        public override string GetOpenPassword() => null;
        public override string GetWorkbookPassword() => null;
        public override ProtectionType GetWorkbookProtectionType() => ProtectionType.None;
        public override string GetWorksheetPassword(string sheetName) => null;
        public override ProtectionType GetWorksheetProtectionType(string sheetName) => ProtectionType.None;
    }
}
```

### Se även

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


