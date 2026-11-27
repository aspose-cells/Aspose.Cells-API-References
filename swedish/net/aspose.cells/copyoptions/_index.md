---
title: "Klass CopyOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.CopyOptions-klass. Representerar kopieringsalternativen"
type: docs
url: /sv/net/aspose.cells/copyoptions/
---
## CopyOptions class

Representerar kopieringsalternativen.

```csharp
public class CopyOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [CopyOptions](copyoptions/)() | CopyOptions-konstruktor. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ColumnCharacterWidth](../../aspose.cells/copyoptions/columncharacterwidth/) { get; set; } | Anger om kolumnbredd ska kopieras i teckenenheter. |
| [CopyInvalidFormulasAsValues](../../aspose.cells/copyoptions/copyinvalidformulasasvalues/) { get; set; } | Om formeln inte är giltig för destinationsmålet, kopieras endast värden. |
| [CopyNames](../../aspose.cells/copyoptions/copynames/) { get; set; } | Anger om namnen ska kopieras. |
| [ExtendToAdjacentRange](../../aspose.cells/copyoptions/extendtoadjacentrange/) { get; set; } | Anger om områden ska utökas när området kopieras till ett intilliggande område. |
| [KeepMacros](../../aspose.cells/copyoptions/keepmacros/) { get; set; } | Anger om makron ska behållas; |
| [ReferToDestinationSheet](../../aspose.cells/copyoptions/refertodestinationsheet/) { get; set; } | När området kopieras i samma fil och diagrammet refererar till källbladet, betyder False att diagrammets datakälla inte ändras. True betyder att diagrammets datakälla refererar till destinationsbladet. |
| [ReferToSheetWithSameName](../../aspose.cells/copyoptions/refertosheetwithsamename/) { get; set; } | I MS Excel, när formler som refererar till andra kalkylblad kopieras samtidigt som ett kalkylblad kopieras till ett annat, bör de kopierade formlerna referera till källarboken. I vissa situationer kan användaren dock behöva att de kopierade formlerna refererar till kalkylblad med samma namn i samma arbetsbok, till exempel när dessa kalkylblad redan har kopierats innan denna kopieringsåtgärd, då bör denna egenskap vara sann. |
| [UpdateInvalidReferencesToTargetSheet](../../aspose.cells/copyoptions/updateinvalidreferencestotargetsheet/) { get; set; } | Anger om målarkbladet ska refereras till om det refererade kalkylbladet inte kopierats. |

### Exempel

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class CopyOptionsDemo
    {
        public static void CopyOptionsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till lite data i kalkylbladet
            sheet.Cells["A1"].PutValue("Hello");
            sheet.Cells["A2"].PutValue("World");

            // Skapa en ny arbetsbok att kopiera data till
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];

            // Skapa ett CopyOptions-objekt
            CopyOptions copyOptions = new CopyOptions
            {
                KeepMacros = true,
                ExtendToAdjacentRange = true,
                CopyNames = true,
                CopyInvalidFormulasAsValues = true,
                ColumnCharacterWidth = true,
                ReferToSheetWithSameName = true,
                ReferToDestinationSheet = true
            };

            // Kopiera data från källkalkylbladet till mål kalkylbladet
            destSheet.Cells.CopyRows(sheet.Cells, 0, 0, 2, copyOptions);

            // Spara målarbetsboken
            destWorkbook.Save("CopyOptionsExample.xlsx");
            destWorkbook.Save("CopyOptionsExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


