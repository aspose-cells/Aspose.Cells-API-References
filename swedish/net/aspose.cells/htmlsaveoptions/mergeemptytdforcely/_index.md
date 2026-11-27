---
title: "HtmlSaveOptions.MergeEmptyTdForcely"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions‑egenskap. Anger om tomma TD‑element ska slås samman tvångsmässigt vid export av fil till html. Storleken på html‑filen kommer att minskas avsevärt efter att värdet satts till true. Standardvärdet är false. Om du vill importera html‑filen till Excel eller exportera perfekta rutnätslinjer när du sparar fil till html, behåll standardvärdet."
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/mergeemptytdforcely/
---
## HtmlSaveOptions.MergeEmptyTdForcely property

Anger om tomma TD‑element ska slås samman tvångsmässigt vid export av fil till html. Storleken på html‑filen kommer att minskas avsevärt efter att värdet satts till true. Standardvärdet är false. Om du vill importera html‑filen till Excel eller exportera perfekta rutnätslinjer när du sparar fil till html, behåll standardvärdet.

```csharp
[Obsolete("Use HtmlSaveOptions.MergeEmptyTdType instead.")]
public bool MergeEmptyTdForcely { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyMergeEmptyTdForcelyDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok med tomma celler
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa några tomma celler i kalkylbladet
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            // B2 är avsiktligt lämnat tomt
            
            // Spara med MergeEmptyTdForcely aktiverat
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.MergeEmptyTdForcely = true;
            workbook.Save("output_with_merge.html", options);
            
            // Spara utan MergeEmptyTdForcely för jämförelse
            options.MergeEmptyTdForcely = false;
            workbook.Save("output_without_merge.html", options);
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


