---
title: "GridJsWorkbook.InsertImage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridJsWorkbook metod. Infogar bild i kalkylbladet från filström eller URL; antingen filström eller URL måste tillhandahållas, eller infogar form när p.type är en av AutoShapeType."
type: docs
url: /sv/net/aspose.cells.gridjs/gridjsworkbook/insertimage/
---
## GridJsWorkbook.InsertImage method

Infogar bild i kalkylbladet från filström eller URL (antingen filström eller URL måste tillhandahållas) eller infogar form när p.type är en av AutoShapeType.

```csharp
public string InsertImage(string uid, string p, Stream s, string imageUrl)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | String | Det unika id:t för filcachen |
| p | String | JSON-formatsträngen för operationen som specificerar cellens plats, kalkylbladets namn, övre vänstra raden, övre vänstra kolumnen för bilden osv {name:'sheet1',ri:1,ci:1} |
| s | Ström | Filströmmen för bildfilen |
| imageUrl | String | URL:en för bildfilen |

### Returvärde

JSON-formatsträngen för den infogade bilden

### Se även

* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


