---
title: MultiThreadReading
second_title: Aspose.Cells för .NET API-referens
description: Hämtar eller ställer in om celldatamodellen ska stödja multitrådsläsning. Standardvärdet för den här egenskapen är false.
type: docs
weight: 200
url: /sv/net/aspose.cells/cells/multithreadreading/
---
## Cells.MultiThreadReading property

Hämtar eller ställer in om celldatamodellen ska stödja multitrådsläsning. Standardvärdet för den här egenskapen är false.

```csharp
public bool MultiThreadReading { get; set; }
```

### Anmärkningar

Om det finns flera trådar för att läsa rad-/cellobjekt i den här samlingen samtidigt, ska denna egenskap ställas in som sant, annars kan oväntade resultat uppstå. Stöd för multitrådsläsning kan försämra prestandan för åtkomst av rad-/cellobjekt från den här samlingen. Observera att vissa funktioner inte stöder multitrådsläsning, såsom formateringsvärden (av[`StringValue`](../../cell/stringvalue) ,[`DisplayStringValue`](../../cell/displaystringvalue) .etc.). Så även om den här egenskapen är inställd som true, kan dessa API:er fortfarande ge oväntade resultat för flertrådsläsning.

### Se även

* class [Cells](../../cells)
* namnutrymme [Aspose.Cells](../../cells)
* hopsättning [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
