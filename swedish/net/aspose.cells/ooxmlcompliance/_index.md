---
title: "Enum OoxmlCompliance"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.OoxmlCompliance enum. Tillåter att ange vilken OOXML-specifikation som ska användas vid sparande i Xlsx-formatet"
type: docs
url: /sv/net/aspose.cells/ooxmlcompliance/
---
## OoxmlCompliance enumeration

Tillåter att ange vilken OOXML-specifikation som ska användas vid sparande i Xlsx-formatet.

```csharp
public enum OoxmlCompliance
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Ecma376_2006 | `0` | ECMA-376 1:a upplagan, 2006. |
| Iso29500_2008_Strict | `1` | ISO/IEC 29500:2008 Strikt efterlevnadsnivå. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlComplianceDemo
    {
        public static void OoxmlComplianceExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till arbetsboksinställningar
            WorkbookSettings settings = workbook.Settings;

            // Ställ in OOXML-efterlevnadsnivån till ISO/IEC 29500:2008 Strict
            settings.Compliance = OoxmlCompliance.Iso29500_2008_Strict;

            // Lägg till lite data i kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello, World!");

            // Spara arbetsboken med den angivna OOXML-efterlevnadsnivån
            workbook.Save("OoxmlComplianceExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


