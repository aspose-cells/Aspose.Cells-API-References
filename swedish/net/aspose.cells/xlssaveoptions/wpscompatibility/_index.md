---
title: "XlsSaveOptions.WpsCompatibility"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XlsSaveOptions-egenskap. Anger om xls ska göras mer kompatibel med WPS"
type: docs
url: /sv/net/aspose.cells/xlssaveoptions/wpscompatibility/
---
## XlsSaveOptions.WpsCompatibility property

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
    public class XlsSaveOptionsPropertyWpsCompatibilityDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Test WPS Compatibility");
            worksheet.Cells["B1"].PutValue(123.45);
            
            // Ställ in sparalternativ med WPS-kompatibilitet
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.WpsCompatibility = true;
            
            // Spara arbetsboken
            workbook.Save("output_with_wps_compatibility.xls", saveOptions);
            
            Console.WriteLine("File saved with WPS compatibility enabled.");
        }
    }
}
```

### Se även

* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


