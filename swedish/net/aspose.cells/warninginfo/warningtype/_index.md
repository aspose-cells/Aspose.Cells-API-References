---
title: "WarningInfo.WarningType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WarningInfo-egenskap. Hämta varningstyp"
type: docs
url: /sv/net/aspose.cells/warninginfo/warningtype/
---
## WarningInfo.WarningType property

Hämta varningstyp.

```csharp
[Obsolete("Use WarningInfo.Type property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public WarningType WarningType { get; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd i stället WarningInfo.Type-egenskapen. Denna egenskap kommer att tas bort 12 månader senare, från och med december 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WarningInfoPropertyWarningTypeDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok och utlösa en varning
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Detta kommer att utlösa en varning vid sparande med ej stödda funktioner
            workbook.Settings.WarningCallback = new WarningCallback();
            
            // Spara med ett format som kan orsaka varningar
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }

    internal class WarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            // Demonstrera användning av egenskapen WarningType
            Console.WriteLine("Warning: " + warningInfo.WarningType + " - " + warningInfo.Description);
            
            // Hantera specifika varningstyper
            if (warningInfo.WarningType == WarningType.UnsupportedFileFormat)
            {
                Console.WriteLine("Unsupported format warning detected!");
            }
        }
    }
}
```

### Se även

* enum [WarningType](../../warningtype/)
* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


