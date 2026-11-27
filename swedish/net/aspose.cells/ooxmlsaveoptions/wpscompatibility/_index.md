---
title: "OoxmlSaveOptions.WpsCompatibility"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OoxmlSaveOptions-egenskap. Anger om xls ska göras mer kompatibel med WPS"
type: docs
url: /sv/net/aspose.cells/ooxmlsaveoptions/wpscompatibility/
---
## OoxmlSaveOptions.WpsCompatibility property

Anger om xls ska göras mer kompatibel med WPS.

```csharp
[Obsolete("Use WorkbookSetting.WpsCompatibility property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool WpsCompatibility { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället WorkbookSetting.WpsCompatibility-egenskapen. Denna metod kommer att tas bort 12 månader senare från december 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyWpsCompatibilityDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första kalkylbladet och lägg till exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test WPS Compatibility");
            
            // Skapa OOXML-sparalternativ och aktivera WPS-kompatibilitet
            OoxmlSaveOptions options = new OoxmlSaveOptions();
            options.WpsCompatibility = true;
            
            // Spara arbetsboken med WPS-kompatibilitet
            workbook.Save("output_with_wps_compatibility.xlsx", options);
            
            Console.WriteLine("Workbook saved with WPS compatibility enabled.");
        }
    }
}
```

### Se även

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


