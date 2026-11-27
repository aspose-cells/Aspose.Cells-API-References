---
title: "Klass Validation"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridWeb.Validation-klass."
type: docs
url: /sv/net/aspose.cells.gridweb/validation/
---
## Validation class

```csharp
[Obsolete("This class is obsolete; use  GridValidation instead")]
public class Validation : CellAttachObject
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [Validation](validation/#constructor)() | Standardkonstruktorn. |
| [Validation](validation/#constructor_1)(GridValidation) |  |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Cell](../../aspose.cells.gridweb.data/cellattachobject/cell/) { get; } | Hämtar den relativa cellen för objektet.(Ärvd från [`CellAttachObject`](../../aspose.cells.gridweb.data/cellattachobject/).) |
| [ClientValidationFunction](../../aspose.cells.gridweb/validation/clientvalidationfunction/) { get; set; } | Hämtar eller anger klientvalideringens JavaScript-funktionsnamn. |
| [ClientValidationOpType](../../aspose.cells.gridweb/validation/clientvalidationoptype/) { get; set; } | Hämtar eller anger validerings‑operationstyp, Between/NotBetween/Equal/NotEqual/Greater/GreaterOrEqual/Less/LessOrEqual. |
| [ClientValidationValue1](../../aspose.cells.gridweb/validation/clientvalidationvalue1/) { get; set; } | Hämtar eller anger operatörens målvärde 1 |
| [ClientValidationValue2](../../aspose.cells.gridweb/validation/clientvalidationvalue2/) { get; set; } | Hämtar eller anger operatörens målvärde 2 |
| [IsRequired](../../aspose.cells.gridweb/validation/isrequired/) { get; set; } | Hämtar eller anger om cellvärdet är obligatoriskt. |
| [RegEx](../../aspose.cells.gridweb/validation/regex/) { get; set; } | Hämtar eller anger reguljära uttryckets sträng. |
| [ValueArray](../../aspose.cells.gridweb/validation/valuearray/) { get; set; } |  |
| [ValueList](../../aspose.cells.gridweb/validation/valuelist/) { get; } | Hämtar värdelistobjektet. |
| [ValueText](../../aspose.cells.gridweb/validation/valuetext/) { get; set; } | Endast för designtid. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [LoadValueList](../../aspose.cells.gridweb/validation/loadvaluelist/)(DataView, string, string, bool) | Laddar värdelista från ett DataView-objekt. Du kan ange värdefältet och textfältet i DataView. Varje värde‑ och textpar kombineras till en sträng, med ett kommatecken mellan dem. |

### Anmärkningar

OBS: Den här klassen är nu föråldrad. vänligen använd GridValidation istället. Den här klassen kommer att tas bort efter 6 månader sedan augusti 2014. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Se även

* class [CellAttachObject](../../aspose.cells.gridweb.data/cellattachobject/)
* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


