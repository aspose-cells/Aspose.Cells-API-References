---
title: "Klasse Validation"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Validation class. Stellt data validation.settings dar"
type: docs
url: /de/net/aspose.cells/validation/
---
## Validation class

Stellt data validation.settings dar.

```csharp
public class Validation
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AlertStyle](../../aspose.cells/validation/alertstyle/) { get; set; } | Stellt den Validierungswarnungsstil dar. |
| [Areas](../../aspose.cells/validation/areas/) { get; } | Ruft alle [`CellArea`](../cellarea/) ab, die die Datenvalidierungseinstellungen enthalten. |
| [ErrorMessage](../../aspose.cells/validation/errormessage/) { get; set; } | Stellt die Fehlermeldung der Datenvalidierung dar. |
| [ErrorTitle](../../aspose.cells/validation/errortitle/) { get; set; } | Stellt den Titel des Fehlermeldungsdialogs der Datenvalidierung dar. |
| [Formula1](../../aspose.cells/validation/formula1/) { get; set; } | Stellt den Wert oder Ausdruck dar, der mit der Datenvalidierung verknüpft ist. |
| [Formula2](../../aspose.cells/validation/formula2/) { get; set; } | Stellt den Wert oder Ausdruck dar, der mit der Datenvalidierung verknüpft ist. |
| [IgnoreBlank](../../aspose.cells/validation/ignoreblank/) { get; set; } | Gibt an, ob leere Werte von der Bereichs-Datenvalidierung erlaubt sind. |
| [InCellDropDown](../../aspose.cells/validation/incelldropdown/) { get; set; } | Gibt an, ob die Datenvalidierung eine Dropdown-Liste anzeigt, die akzeptable Werte enthält. |
| [InputMessage](../../aspose.cells/validation/inputmessage/) { get; set; } | Stellt die Eingabenachricht der Datenvalidierung dar. |
| [InputTitle](../../aspose.cells/validation/inputtitle/) { get; set; } | Stellt den Titel des Eingabedialogs der Datenvalidierung dar. |
| [Operator](../../aspose.cells/validation/operator/) { get; set; } | Stellt den Operator für die Datenvalidierung dar. |
| [ShowError](../../aspose.cells/validation/showerror/) { get; set; } | Gibt an, ob die Fehlermeldung der Datenvalidierung angezeigt wird, sobald der Benutzer ungültige Daten eingibt. |
| [ShowInput](../../aspose.cells/validation/showinput/) { get; set; } | Gibt an, ob die Eingabenachricht der Datenvalidierung angezeigt wird, sobald der Benutzer eine Zelle im Datenvalidierungsbereich auswählt. |
| [Type](../../aspose.cells/validation/type/) { get; set; } | Stellt den Typ der Datenvalidierung dar. |
| [Value1](../../aspose.cells/validation/value1/) { get; set; } | Stellt den ersten Wert dar, der mit der Datenvalidierung verknüpft ist. |
| [Value2](../../aspose.cells/validation/value2/) { get; set; } | Stellt den zweiten Wert dar, der mit der Datenvalidierung verknüpft ist. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddArea](../../aspose.cells/validation/addarea/#addarea)(CellArea) | Wendet die Validierung auf den Bereich an. |
| [AddArea](../../aspose.cells/validation/addarea/#addarea_1)(CellArea, bool, bool) | Wendet die Validierung auf den Bereich an. |
| [AddAreas](../../aspose.cells/validation/addareas/)(CellArea[], bool, bool) | Wendet die Validierung auf die angegebenen Bereiche an. |
| [Copy](../../aspose.cells/validation/copy/)(Validation, CopyOptions) | Validierung kopieren. |
| [GetFormula1](../../aspose.cells/validation/getformula1/#getformula1)(bool, bool) | Liest den Wert oder Ausdruck, der mit dieser Validierung verknüpft ist. |
| [GetFormula1](../../aspose.cells/validation/getformula1/#getformula1_1)(bool, bool, int, int) | Liest den Wert oder Ausdruck, der mit dieser Validierung für eine bestimmte Zelle verknüpft ist. |
| [GetFormula2](../../aspose.cells/validation/getformula2/#getformula2)(bool, bool) | Liest den Wert oder Ausdruck, der mit dieser Validierung verknüpft ist. |
| [GetFormula2](../../aspose.cells/validation/getformula2/#getformula2_1)(bool, bool, int, int) | Liest den Wert oder Ausdruck, der mit dieser Validierung für eine bestimmte Zelle verknüpft ist. |
| [GetListValue](../../aspose.cells/validation/getlistvalue/)(int, int) | Liest den Wert für die Liste der Validierung für die angegebene Zelle. |
| [GetValue](../../aspose.cells/validation/getvalue/)(int, int, bool) | Liest den Wert der Validierung für die spezifische Zelle. |
| [RemoveACell](../../aspose.cells/validation/removeacell/)(int, int) | Entfernt die Validierungseinstellungen in der Zelle. |
| [RemoveArea](../../aspose.cells/validation/removearea/)(CellArea) | Entfernt die Validierungseinstellungen im Bereich. |
| [RemoveAreas](../../aspose.cells/validation/removeareas/)(CellArea[]) | Entfernt diese Validierung aus den angegebenen Bereichen. |
| [SetFormula1](../../aspose.cells/validation/setformula1/)(string, bool, bool) | Setzt den Wert oder Ausdruck, der mit dieser Validierung verknüpft ist. |
| [SetFormula2](../../aspose.cells/validation/setformula2/)(string, bool, bool) | Setzt den Wert oder Ausdruck, der mit dieser Validierung verknüpft ist. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationDemo
    {
        public static void ValidationExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Definiert einen Zellenbereich für die Validierung
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);

            // Greift auf die Validierungssammlung zu
            ValidationCollection validations = worksheet.Validations;

            // Fügt der Sammlung eine neue Validierung hinzu
            int validationIndex = validations.Add(area);
            Validation validation = validations[validationIndex];

            // Setzt Validierungseigenschaften
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "3";
            validation.Formula2 = "1234";
            validation.InputMessage = "Please enter a whole number between 3 and 1234.";
            validation.InputTitle = "Whole Number Validation";
            validation.ErrorMessage = "The value must be a whole number between 3 and 1234.";
            validation.ErrorTitle = "Invalid Input";
            validation.ShowInput = true;
            validation.ShowError = true;
            validation.IgnoreBlank = true;
            validation.InCellDropDown = true;

            // Speichere die Arbeitsmappe
            workbook.Save("ValidationExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


