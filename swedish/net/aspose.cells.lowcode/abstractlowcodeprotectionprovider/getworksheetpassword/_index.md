---
title: "AbstractLowCodeProtectionProvider.GetWorksheetPassword"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractLowCodeProtectionProvider-metod. Hämtar lösenordet för att skydda det angivna kalkylbladet"
type: docs
url: /sv/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworksheetpassword/
---
## AbstractLowCodeProtectionProvider.GetWorksheetPassword method

Hämtar lösenordet för att skydda det angivna kalkylbladet.

```csharp
public virtual string GetWorksheetPassword(string sheetName)
```

### Returvärde

Lösenord för att skydda det angivna kalkylbladet.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetWorksheetPasswordWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            string sheetName = worksheet.Name;

            // Skapa en instans av anpassad skyddsleverantör
            var provider = new CustomProtectionProvider();

            try
            {
                // Anropa GetWorksheetPassword med kalkylbladets namn
                string password = provider.GetWorksheetPassword(sheetName);

                // Tillämpa skydd på kalkylbladet med det hämtade lösenordet
                worksheet.Protect(ProtectionType.All, password, null);

                Console.WriteLine($"Protected worksheet '{sheetName}' with password: {password}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetWorksheetPassword: {ex.Message}");
            }

            // Spara den skyddade arbetsboken
            workbook.Save("WorksheetPasswordDemo.xlsx");

        }
    }

    // Anpassad implementation som returnerar lösenord baserat på bladnamn
    public class CustomProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public new string GetWorksheetPassword(string sheetName)
        {
            // Enkel lösenordsgenereringslogik för demonstration
            return $"pw_{sheetName}";
        }
    }
}
```

### Se även

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


