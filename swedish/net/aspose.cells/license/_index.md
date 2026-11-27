---
title: "Klass Licens"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.License-klass. Tillhandahåller metoder för att licensiera komponenten"
type: docs
url: /sv/net/aspose.cells/license/
---
## License class

Tillhandahåller metoder för att licensiera komponenten.

```csharp
public class License
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [License](license/)() | Initierar en ny instans av denna klass. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [SetLicense](../../aspose.cells/license/setlicense/#setlicense)(Stream) | Licensierar komponenten. |
| [SetLicense](../../aspose.cells/license/setlicense/#setlicense_1)(string) | Licensierar komponenten. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LicenseDemo
    {
        public static void LicenseExample()
        {
            // Skapa en instans av Licens-klassen
            License license = new License();

            // Ange licensen med ett licensfilnamn
            license.SetLicense("Aspose.Cells.NET.lic");

            // Alternativt, ange licensen med en ström
            using (FileStream licenseStream = new FileStream("Aspose.Cells.NET.lic", FileMode.Open))
            {
                license.SetLicense(licenseStream);
            }

            // Ytterligare kod för att demonstrera användningen av licensierad Aspose.Cells-funktionalitet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello, Aspose.Cells!");

            // Spara arbetsboken för att verifiera att licensen har tillämpats korrekt
            workbook.Save("LicensedWorkbook.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


