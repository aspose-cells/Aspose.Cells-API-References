---
title: "GridJsWorkbook.JsonToStream"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridJsWorkbook-metod. Genererar JSON från den minnesbaserade Workbook och skriver den till den angivna strömmen. Cachar valfritt det genererade JSON för snabbare efterföljande hämtning. Viktiga skillnader från JsonToStreamByUid  Denna metod använder det aktuella minnesbaserade Workbook-tillståndet wb-fältet  JsonToStreamByUid läser in Workbook från .cells-cachefiler på disk  Använd denna metod när du vill exportera det aktuella arbetsbokens tillstånd efter ändringar  Använd JsonToStreamByUid när du behöver återskapa JSON från ett tidigare cachat filtillstånd  Cachingbeteende när uid tillhandahålls  Kontrollerar JSON-cache innan generering L1 minne  L2 disk  Vid cachemiss genereras JSON från minnesbaserad workbook  Lagrar genererat JSON i cache för framtida förfrågningar"
type: docs
url: /sv/net/aspose.cells.gridjs/gridjsworkbook/jsontostream/
---
## GridJsWorkbook.JsonToStream method

Generera JSON från den minnesbaserade Workbook och skriv den till den angivna strömmen. Valfritt cachas den genererade JSON för snabbare efterföljande hämtning. Viktiga skillnader mot JsonToStreamByUid: - Denna metod använder det aktuella minnesbaserade Workbook‑tillståndet (wb‑fältet) - JsonToStreamByUid laddar om Workbook från .cells‑cache‑filer på disk - Använd denna metod när du vill exportera det aktuella arbetsbokens tillstånd efter ändringar - Använd JsonToStreamByUid när du behöver återskapa JSON från ett tidigare cachat filtillstånd. Caching‑beteende (när uid tillhandahålls): - Kontrollerar JSON‑cache innan generering (L1‑minne + L2‑disk) - Vid cache‑miss genereras JSON från minnes‑Workbook - Sparar genererad JSON i cache för framtida förfrågningar

```csharp
public void JsonToStream(Stream stream, string filename, string uid = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström | Utdatastreamen att skriva JSON-data till |
| filnamn | String | Anger filnamnet i JSON. Om det sätts till null, är standardfilnamnet: book1. |
| uid | String | Valfri unik identifierare för JSON-cachning. När den tillhandahålls möjliggör den cacheuppslagning och lagring. |

### Se även

* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


