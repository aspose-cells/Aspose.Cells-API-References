---
title: "Klasse Validation"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridWeb.Validation Klasse."
type: docs
url: /de/net/aspose.cells.gridweb/validation/
---
## Validation class

```csharp
[Obsolete("This class is obsolete; use  GridValidation instead")]
public class Validation : CellAttachObject
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [Validation](validation/#constructor)() | Der Standardkonstruktor. |
| [Validation](validation/#constructor_1)(GridValidation) |  |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Cell](../../aspose.cells.gridweb.data/cellattachobject/cell/) { get; } | Liefert die relative Zelle des Objekts. (Vererbt von [`CellAttachObject`](../../aspose.cells.gridweb.data/cellattachobject/).) |
| [ClientValidationFunction](../../aspose.cells.gridweb/validation/clientvalidationfunction/) { get; set; } | Liest oder setzt den Namen der clientseitigen Validierungs-JavaScript-Funktion. |
| [ClientValidationOpType](../../aspose.cells.gridweb/validation/clientvalidationoptype/) { get; set; } | Liest oder setzt den Validierungs‑Operationstyp, Between/NotBetween/Equal/NotEqual/Greater/GreaterOrEqual/Less/LessOrEqual. |
| [ClientValidationValue1](../../aspose.cells.gridweb/validation/clientvalidationvalue1/) { get; set; } | Liest oder setzt den Zielwert des Operators 1 |
| [ClientValidationValue2](../../aspose.cells.gridweb/validation/clientvalidationvalue2/) { get; set; } | Liest oder setzt den Zielwert des Operators 2 |
| [IsRequired](../../aspose.cells.gridweb/validation/isrequired/) { get; set; } | Liest oder schreibt, ob der Zellenwert erforderlich ist. |
| [RegEx](../../aspose.cells.gridweb/validation/regex/) { get; set; } | Liest oder setzt die reguläre Ausdruckszeichenkette. |
| [ValueArray](../../aspose.cells.gridweb/validation/valuearray/) { get; set; } |  |
| [ValueList](../../aspose.cells.gridweb/validation/valuelist/) { get; } | Liest das Wertlistenobjekt. |
| [ValueText](../../aspose.cells.gridweb/validation/valuetext/) { get; set; } | Nur zur Entwurfszeit verwendet. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [LoadValueList](../../aspose.cells.gridweb/validation/loadvaluelist/)(DataView, string, string, bool) | Lädt die Wertliste aus einem DataView‑Objekt. Sie können das Werte‑ und Textfeld des DataView angeben. Jeder Werte‑ und Text‑Paar wird zu einem String kombiniert, getrennt durch ein Komma. |

### Hinweise

HINWEIS: Diese Klasse ist jetzt veraltet. Bitte verwenden Sie stattdessen GridValidation. Diese Klasse wird nach 6 Monaten ab August 2014 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Siehe auch

* class [CellAttachObject](../../aspose.cells.gridweb.data/cellattachobject/)
* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


