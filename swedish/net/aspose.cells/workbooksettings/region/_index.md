---
title: Region
second_title: Aspose.Cells för .NET API-referens
description: Hämtar eller ställer in de regionala inställningarna för arbetsboken.
type: docs
weight: 370
url: /sv/net/aspose.cells/workbooksettings/region/
---
## WorkbookSettings.Region property

Hämtar eller ställer in de regionala inställningarna för arbetsboken.

```csharp
public CountryCode Region { get; set; }
```

### Anmärkningar

1. Regionala inställningar som används av Aspose.Cells-komponenten för en arbetsbok som laddas från mallfilen: i). För en XLS-fil finns det fält definierade för regionala inställningar och MS Excel sparar regionala inställningar i filen när XLS-filen sparas. Så vi använder den sparade regionen i mallfilen för arbetsboken. Om du inte gör det om du vill använda regionen som sparats i XLS-filen, återställ den till den förväntade (som CountryCode.Default) efter att ha laddat mallfilen. Och vi sparar det användarspecificerade värdet (med den här metoden) i filen också när du sparar en XLS-fil. ii). För andra filformat, såsom XLSX, XLSB...etc., finns det inget fält definierat för regionala inställningar i filformatspecifikationen. Så vi använder de regionala inställningarna för programmets miljö för arbetsboken. Och, användarspecificerat värde (med den här metoden) kan inte behållas för de genererade filerna med dessa filformat. 2. För vyeffekten i MS Excel: De tillämpade regionala inställningarna här kan endast träda i kraft under körning med Aspose.Cells-komponenten och inte när du tittar på den genererade filen med MS Excel. Även för den genererade XLS-filen där de angivna regionala inställningsdata har sparats, när du visar/redigerar den med MS Excel, är den region som används för att utföra formatering med MS Excel alltid standard regionala inställningar för miljön där MS Excel körs, inte den som sparats i filen. Det är MS Excels beteende och kan inte ändras med kod.

### Se även

* enum [CountryCode](../../countrycode)
* class [WorkbookSettings](../../workbooksettings)
* namnutrymme [Aspose.Cells](../../workbooksettings)
* hopsättning [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->