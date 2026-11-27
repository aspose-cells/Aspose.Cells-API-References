---
title: "Klass Style"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridDesktop.Style klass. Representerar visningsstil för Excel‑dokument såsom teckenfärg, justering, kant osv."
type: docs
url: /sv/net/aspose.cells.griddesktop/style/
---
## Style class

Representerar visningsstil för ett Excel‑dokument, såsom teckensnitt, färg, justering, kantlinje osv.

```csharp
public class Style
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [Style](style/)(GridDesktop) | skapa en ny Style för kontrollen |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BackgroundColor](../../aspose.cells.griddesktop/style/backgroundcolor/) { get; set; } | Hämtar eller anger cellens bakgrundsfärg; om stilmönstret inte är satt till solid, kommer det att ha effekt. |
| [CellLocked](../../aspose.cells.griddesktop/style/celllocked/) { get; set; } | Hämtar eller anger ett värde som indikerar om en cell kan ändras eller inte. |
| [Color](../../aspose.cells.griddesktop/style/color/) { get; set; } | Hämtar eller anger cellens skuggfärg. När mönstret är none, returneras Color.Empty; när mönstret är BackgroundType.Solid, returneras ForegroundColor; annars returneras BackgroundColor. |
| [Custom](../../aspose.cells.griddesktop/style/custom/) { get; set; } | Representerar den anpassade talformatsträngen för detta stilobjekt. Om det anpassade talformatet inte är angivet (till exempel om talformatet är inbyggt) returneras "". |
| [Font](../../aspose.cells.griddesktop/style/font/) { get; set; } | Hämtar ett [`GridFont`](../../aspose.cells.griddesktop.data/gridfont/)‑objekt. |
| [ForegroundColor](../../aspose.cells.griddesktop/style/foregroundcolor/) { get; set; } | Hämtar eller anger en stils förgrundsfärg. |
| [HAlignment](../../aspose.cells.griddesktop/style/halignment/) { get; set; } | Hämtar eller anger horisontellt justeringsattribut. |
| [Indent](../../aspose.cells.griddesktop/style/indent/) { get; set; } | Representerar m_IndentLevel‑nivån för cellen eller området. Kan endast vara ett heltal mellan 0 och 15. |
| [NumberType](../../aspose.cells.griddesktop/style/numbertype/) { get; set; } | Hämtar eller anger visningsformatet för tal och datum. Formateringsmönstren skiljer sig åt mellan olika regioner. |
| [Pattern](../../aspose.cells.griddesktop/style/pattern/) { get; set; } | Hämtar eller anger cellens bakgrundsmönstertyp. |
| [Rotation](../../aspose.cells.griddesktop/style/rotation/) { get; set; } | Representerar textrotationsvinkeln. |
| [Shrink](../../aspose.cells.griddesktop/style/shrink/) { get; set; } | Representerar om text automatiskt krymper för att passa i den tillgängliga kolumnbredden. |
| [TextDirection](../../aspose.cells.griddesktop/style/textdirection/) { get; set; } | Hämtar eller anger textdirektionsattribut. |
| [TextWrapped](../../aspose.cells.griddesktop/style/textwrapped/) { get; set; } | Hämtar eller anger ett värde som indikerar om texten i en cell är radbruten. |
| [VAlignment](../../aspose.cells.griddesktop/style/valignment/) { get; set; } | Hämtar eller anger vertikalt justeringsattribut. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Clone](../../aspose.cells.griddesktop/style/clone/)() | Skapar och returnerar en kopia av detta objekt. **NOTE:**Om du klonar en namngiven stil, klonas inte namnet eftersom stilnamnet måste vara unikt. Därför kommer den klonade stilen inte att \"equals to\" den ursprungliga stilen. |
| [SetBorderColor](../../aspose.cells.griddesktop/style/setbordercolor/)(BorderType, Color) | Anger färgen på den angivna kanten. |
| [SetBorderLine](../../aspose.cells.griddesktop/style/setborderline/)(BorderType, BorderLineType) | Ställer in kantlinjetypen för den angivna kanten. |

### Se även

* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


