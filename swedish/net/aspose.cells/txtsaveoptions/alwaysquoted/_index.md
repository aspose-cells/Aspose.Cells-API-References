---
title: "TxtSaveOptions.AlwaysQuoted"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TxtSaveOptions egenskap. Anger om alltid ska lägga till  för varje fält. Om true så kommer alla värden att omges av citationstecken. Om false så kommer värden endast att omges av citationstecken när det behövs, till exempel när värden innehåller specialtecken såsom   n eller separator-tecken. Standard är falskt."
type: docs
url: /sv/net/aspose.cells/txtsaveoptions/alwaysquoted/
---
## TxtSaveOptions.AlwaysQuoted property

Anger om alltid ska lägga till '"' för varje fält. Om true så kommer alla värden att omges av citationstecken; om false så kommer värden endast att omges av citationstecken när det behövs (till exempel när värden innehåller specialtecken såsom '"', '\n' eller separator-tecken). Standard är falskt.

```csharp
[Obsolete("Use QuoteType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool AlwaysQuoted { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället QuoteType-egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med augusti 2012. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyAlwaysQuotedDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200.50);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(899.99);

            // Skapa TxtSaveOptions med AlwaysQuoted satt till true
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Separator = ',',
                AlwaysQuoted = true,
                QuoteType = TxtValueQuoteType.Always
            };

            // Spara med citationstecken runt alla värden
            workbook.Save("AlwaysQuoted_True.txt", saveOptions);

            // Ändra till false och spara igen
            saveOptions.AlwaysQuoted = false;
            workbook.Save("AlwaysQuoted_False.txt", saveOptions);

            Console.WriteLine("Files saved with different AlwaysQuoted settings.");
        }
    }
}
```

### Se även

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


