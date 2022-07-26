---
title: Validation
second_title: Aspose.Cells für .NET-API-Referenz
description: Repräsentiert Datenvalidierung.Einstellungen.
type: docs
weight: 6200
url: /de/net/aspose.cells/validation/
---
## Validation class

Repräsentiert Datenvalidierung.Einstellungen.

```csharp
public class Validation
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AlertStyle](../../aspose.cells/validation/alertstyle) { get; set; } | Stellt den Validierungswarnstil dar. |
| [Areas](../../aspose.cells/validation/areas) { get; } | bekommt alles[`CellArea`](../cellarea) die die Datenvalidierungseinstellungen enthalten. |
| [ErrorMessage](../../aspose.cells/validation/errormessage) { get; set; } | Stellt die Datenüberprüfungsfehlermeldung dar. |
| [ErrorTitle](../../aspose.cells/validation/errortitle) { get; set; } | Repräsentiert den Titel des Datenvalidierungsfehler-Dialogfelds. |
| [Formula1](../../aspose.cells/validation/formula1) { get; set; } | Stellt den Wert oder Ausdruck dar, der der Datenvalidierung zugeordnet ist. |
| [Formula2](../../aspose.cells/validation/formula2) { get; set; } | Stellt den Wert oder Ausdruck dar, der der Datenvalidierung zugeordnet ist. |
| [IgnoreBlank](../../aspose.cells/validation/ignoreblank) { get; set; } | Gibt an, ob Leerwerte von der Bereichsdatenvalidierung zugelassen sind. |
| [InCellDropDown](../../aspose.cells/validation/incelldropdown) { get; set; } | Gibt an, ob die Datenvalidierung eine Dropdown-Liste anzeigt, die akzeptable Werte enthält. |
| [InputMessage](../../aspose.cells/validation/inputmessage) { get; set; } | Stellt die Eingabenachricht zur Datenüberprüfung dar. |
| [InputTitle](../../aspose.cells/validation/inputtitle) { get; set; } | Repräsentiert den Titel des Eingabedialogfelds zur Datenvalidierung. |
| [Operator](../../aspose.cells/validation/operator) { get; set; } | Stellt den Operator für die Datenvalidierung dar. |
| [ShowError](../../aspose.cells/validation/showerror) { get; set; } | Gibt an, ob die Datenüberprüfungsfehlermeldung angezeigt wird, wenn der Benutzer ungültige Daten eingibt. |
| [ShowInput](../../aspose.cells/validation/showinput) { get; set; } | Gibt an, ob die Eingabemeldung zur Datenüberprüfung angezeigt wird, wenn der Benutzer eine Zelle im Datenüberprüfungsbereich auswählt. |
| [Type](../../aspose.cells/validation/type) { get; set; } | Repräsentiert den Datenvalidierungstyp. |
| [Value1](../../aspose.cells/validation/value1) { get; set; } | Stellt den ersten Wert dar, der der Datenvalidierung zugeordnet ist. |
| [Value2](../../aspose.cells/validation/value2) { get; set; } | Stellt den zweiten Wert dar, der der Datenvalidierung zugeordnet ist. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddArea](../../aspose.cells/validation/addarea#addarea)(CellArea) | Wendet die Validierung auf den Bereich an. |
| [AddArea](../../aspose.cells/validation/addarea#addarea_1)(CellArea, bool, bool) | Wendet die Validierung auf den Bereich an. |
| [AddAreas](../../aspose.cells/validation/addareas)(CellArea[], bool, bool) | Wendet die Validierung auf bestimmte Bereiche an. |
| [Copy](../../aspose.cells/validation/copy)(Validation, CopyOptions) | Kopiervalidierung. |
| [GetFormula1](../../aspose.cells/validation/getformula1#getformula1)(bool, bool) | Ruft den Wert oder Ausdruck ab, der dieser Validierung zugeordnet ist. |
| [GetFormula1](../../aspose.cells/validation/getformula1#getformula1_1)(bool, bool, int, int) | Ruft den Wert oder Ausdruck ab, der dieser Validierung für eine bestimmte Zelle zugeordnet ist. |
| [GetFormula2](../../aspose.cells/validation/getformula2#getformula2)(bool, bool) | Ruft den Wert oder Ausdruck ab, der dieser Validierung zugeordnet ist. |
| [GetFormula2](../../aspose.cells/validation/getformula2#getformula2_1)(bool, bool, int, int) | Ruft den Wert oder Ausdruck ab, der dieser Validierung für eine bestimmte Zelle zugeordnet ist. |
| [GetListValue](../../aspose.cells/validation/getlistvalue)(int, int) | Holen Sie sich den Wert für die Liste der Validierung für die angegebene Zelle. |
| [RemoveACell](../../aspose.cells/validation/removeacell)(int, int) | Entfernen Sie die Validierungseinstellungen in der Zelle. |
| [RemoveArea](../../aspose.cells/validation/removearea)(CellArea) | Entfernen Sie die Validierungseinstellungen im Bereich. |
| [RemoveAreas](../../aspose.cells/validation/removeareas)(CellArea[]) | Entfernt diese Validierung aus bestimmten Bereichen. |
| [SetFormula1](../../aspose.cells/validation/setformula1)(string, bool, bool) | Legt den Wert oder Ausdruck fest, der dieser Validierung zugeordnet ist. |
| [SetFormula2](../../aspose.cells/validation/setformula2)(string, bool, bool) | Legt den Wert oder Ausdruck fest, der dieser Validierung zugeordnet ist. |

### Beispiele

```csharp
[C#]
Workbook workbook = new Workbook();
ValidationCollection validations = workbook.Worksheets[0].Validations;
CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);
Validation validation = validations[validations.Add(area)];
validation.Type = Aspose.Cells.ValidationType.WholeNumber;
validation.Operator = OperatorType.Between;
validation.Formula1 = "3";
validation.Formula2 = "1234";

[Visual Basic]
Dim workbook as Workbook = new Workbook()
Dim validations as ValidationCollection  = workbook.Worksheets(0).Validations
Dim area as CellArea = CellArea.CreateCellArea(0, 0, 1, 1);
Dim validation as Validation = validations(validations.Add(area))
validation.Type = ValidationType.WholeNumber
validation.Operator = OperatorType.Between
validation.Formula1 = "3"
validation.Formula2 = "1234"
```

### Siehe auch

* namensraum [Aspose.Cells](../../aspose.cells)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
