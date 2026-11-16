---
title: "Validierungsklasse"
linktitle: "Validierung"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "Validierungsklasse. Kapselt das Objekt, das die Validierung in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/validation/
---

## Validation class

Stellt Datenvalidierungseinstellungen dar.

```go

type Validation struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetOperator](./getoperator/) | Stellt den Operator für die Datenvalidierung dar. |
| [SetOperator](./setoperator/) | Stellt den Operator für die Datenvalidierung dar. |
| [GetAlertStyle](./getalertstyle/) | Stellt den Validierungs-Alarmstil dar. |
| [SetAlertStyle](./setalertstyle/) | Stellt den Validierungs-Alarmstil dar. |
| [GetType](./gettype/) | Stellt den Typ der Datenvalidierung dar. |
| [SetType](./settype/) | Stellt den Typ der Datenvalidierung dar. |
| [GetInputMessage](./getinputmessage/) | Stellt die Eingabemeldung der Datenvalidierung dar. |
| [SetInputMessage](./setinputmessage/) | Stellt die Eingabemeldung der Datenvalidierung dar. |
| [GetInputTitle](./getinputtitle/) | Stellt den Titel des Eingabedialogfelds der Datenvalidierung dar. |
| [SetInputTitle](./setinputtitle/) | Stellt den Titel des Eingabedialogfelds der Datenvalidierung dar. |
| [GetErrorMessage](./geterrormessage/) | Stellt die Fehlermeldung der Datenvalidierung dar. |
| [SetErrorMessage](./seterrormessage/) | Stellt die Fehlermeldung der Datenvalidierung dar. |
| [GetErrorTitle](./geterrortitle/) | Stellt den Titel des Fehlerdialogfelds der Datenvalidierung dar. |
| [SetErrorTitle](./seterrortitle/) | Stellt den Titel des Fehlerdialogfelds der Datenvalidierung dar. |
| [GetShowInput](./getshowinput/) | Gibt an, ob die Eingabemeldung der Datenvalidierung angezeigt wird, wenn der Benutzer eine Zelle im Datenvalidierungsbereich auswählt. |
| [SetShowInput](./setshowinput/) | Gibt an, ob die Eingabemeldung der Datenvalidierung angezeigt wird, wenn der Benutzer eine Zelle im Datenvalidierungsbereich auswählt. |
| [GetShowError](./getshowerror/) | Gibt an, ob die Fehlermeldung der Datenvalidierung angezeigt wird, wenn der Benutzer ungültige Daten eingibt. |
| [SetShowError](./setshowerror/) | Gibt an, ob die Fehlermeldung der Datenvalidierung angezeigt wird, wenn der Benutzer ungültige Daten eingibt. |
| [GetIgnoreBlank](./getignoreblank/) | Gibt an, ob leere Werte durch die Bereichs-Datenvalidierung erlaubt sind. |
| [SetIgnoreBlank](./setignoreblank/) | Gibt an, ob leere Werte durch die Bereichs-Datenvalidierung erlaubt sind. |
| [GetFormula1_Bool_Bool](./getformula1_bool_bool/) | Ermittelt den Wert oder Ausdruck, der mit dieser Validierung verknüpft ist. |
| [GetFormula2_Bool_Bool](./getformula2_bool_bool/) | Ermittelt den Wert oder Ausdruck, der mit dieser Validierung verknüpft ist. |
| [GetFormula1_Bool_Bool_Int_Int](./getformula1_bool_bool_int_int/) | Ermittelt den Wert oder Ausdruck, der mit dieser Validierung für eine bestimmte Zelle verknüpft ist. |
| [GetFormula2_Bool_Bool_Int_Int](./getformula2_bool_bool_int_int/) | Ermittelt den Wert oder Ausdruck, der mit dieser Validierung für eine bestimmte Zelle verknüpft ist. |
| [SetFormula1_String_Bool_Bool](./setformula1_string_bool_bool/) | Setzt den Wert oder Ausdruck, der mit dieser Validierung verknüpft ist. |
| [SetFormula2_String_Bool_Bool](./setformula2_string_bool_bool/) | Setzt den Wert oder Ausdruck, der mit dieser Validierung verknüpft ist. |
| [GetFormula1](./getformula1/) | Stellt den Wert oder Ausdruck dar, der mit der Datenvalidierung verknüpft ist. |
| [SetFormula1_String](./setformula1_string/) | Stellt den Wert oder Ausdruck dar, der mit der Datenvalidierung verknüpft ist. |
| [GetFormula2](./getformula2/) | Stellt den Wert oder Ausdruck dar, der mit der Datenvalidierung verknüpft ist. |
| [SetFormula2_String](./setformula2_string/) | Stellt den Wert oder Ausdruck dar, der mit der Datenvalidierung verknüpft ist. |
| [GetListValue](./getlistvalue/) | Ermittelt den Wert für die Liste der Validierung für die angegebene Zelle. |
| [GetValue1](./getvalue1/) | Stellt den ersten Wert dar, der mit der Datenvalidierung verknüpft ist. |
| [SetValue1](./setvalue1/) | Stellt den ersten Wert dar, der mit der Datenvalidierung verknüpft ist. |
| [GetValue2](./getvalue2/) | Stellt den zweiten Wert dar, der mit der Datenvalidierung verknüpft ist. |
| [SetValue2](./setvalue2/) | Stellt den zweiten Wert dar, der mit der Datenvalidierung verknüpft ist. |
| [GetValue](./getvalue/) | Ermittelt den Wert der Validierung für die spezifische Zelle. |
| [GetInCellDropDown](./getincelldropdown/) | Gibt an, ob die Datenvalidierung eine Dropdown-Liste anzeigt, die akzeptable Werte enthält. |
| [SetInCellDropDown](./setincelldropdown/) | Gibt an, ob die Datenvalidierung eine Dropdown-Liste anzeigt, die akzeptable Werte enthält. |
| [GetAreas](./getareas/) | Ruft alle CellArea ab, die die Datenvalidierungseinstellungen enthalten. |
| [AddArea_CellArea](./addarea_cellarea/) | Wendet die Validierung auf den Bereich an. |
| [AddArea_CellArea_Bool_Bool](./addarea_cellarea_bool_bool/) | Wendet die Validierung auf den Bereich an. |
| [AddAreas](./addareas/) | Wendet die Validierung auf die angegebenen Bereiche an. |
| [RemoveArea](./removearea/) | Entfernt die Validierungseinstellungen im Bereich. |
| [RemoveAreas](./removeareas/) | Entfernt diese Validierung aus den angegebenen Bereichen. |
| [RemoveACell](./removeacell/) | Entfernt die Validierungseinstellungen in der Zelle. |
| [Copy](./copy/) | Validierung kopieren. |
