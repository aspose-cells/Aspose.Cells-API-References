---
title: "Enum GridLoadDataFilterOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridDesktop.Data.GridLoadDataFilterOptions enum. Representerar alternativen för att filtrera data när arbetsboken laddas från en mall"
type: docs
url: /sv/net/aspose.cells.griddesktop.data/gridloaddatafilteroptions/
---
## GridLoadDataFilterOptions enumeration

Representerar alternativen för att filtrera data när arbetsboken laddas från en mall.

```csharp
public enum GridLoadDataFilterOptions
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| All | `2147483647` | Läs in allt |
| CellBlank | `1` | Läs in celler vars värde är tomt |
| CellString | `2` | Läs in celler vars värde är en sträng |
| CellNumeric | `4` | Läs in celler vars värde är numeriskt(inklusive datum/tid) |
| CellError | `8` | Läs in celler vars värde är fel |
| CellBool | `16` | Läs in celler vars värde är boolesk |
| CellValue | `31` | Läs in cellvärden (alla värdetyper) endast |
| Formula | `32` | Läs in cellformler. |
| CellData | `67108927` | Läs in celldata inklusive värden, formler och formatering |
| Chart | `256` | Läs in diagram |
| Drawing | `402653952` | Ritobjekt(inklusive Diagram, Bild, OleObject och alla andra ritobjekt) |
| MergedArea | `1024` | Läs in sammanslagna celler |
| ConditionalFormatting | `2048` | Läs in villkorsstyrd formatering |
| DataValidation | `4096` | Läs in datavalideringar |
| PivotTable | `8192` | Läs in pivottabeller |
| Table | `16384` | Läs in tabeller |
| Hyperlinks | `32768` | Läs in hyperlänkar |
| SheetSettings | `65536` | Läs in inställningar för arbetsblad |
| SheetData | `403701759` | Läs in all data för arbetsblad, såsom celldata, inställningar, objekt, ...etc. |
| BookSettings | `1048576` | Läs in inställningar för arbetsbok |
| Settings | `1114112` | Läs in inställningar för arbetsbok och arbetsblad |
| XmlMap | `2097152` | Läs in XmlMap |
| Structure | `4194304` | Läs in strukturen för arbetsboken |
| DocumentProperties | `8388608` | Läs in dokumentegenskaper |
| DefinedNames | `16777216` | Läs in definierade Namn-objekt |
| VBA | `33554432` | Ladda VBA-projekt |
| Style | `67108864` | Ladda stilar för cellformatering |
| Picture | `134217728` | Ladda bilder |
| OleObject | `268435456` | Ladda OleObjects |
| Revision | `536870912` | Ladda revisionsloggar |

### Se även

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


