---
title: "Schutzklasse"
linktitle: "Schutz"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "Schutzklasse. Kapselt das Objekt, das den Schutz in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/protection/
---

## Protection class

Stellt die verschiedenen Arten von Schutzoptionen dar, die für ein Arbeitsblatt verfügbar sind.

```go

type Protection struct  {
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
| [Copy](./copy/) | Kopiere Schutzinformationen. |
| [GetAllowDeletingColumn](./getallowdeletingcolumn/) | Gibt an, ob das Löschen von Spalten in einem geschützten Arbeitsblatt erlaubt ist. |
| [SetAllowDeletingColumn](./setallowdeletingcolumn/) | Gibt an, ob das Löschen von Spalten in einem geschützten Arbeitsblatt erlaubt ist. |
| [GetAllowDeletingRow](./getallowdeletingrow/) | Gibt an, ob das Löschen von Zeilen in einem geschützten Arbeitsblatt erlaubt ist. |
| [SetAllowDeletingRow](./setallowdeletingrow/) | Gibt an, ob das Löschen von Zeilen in einem geschützten Arbeitsblatt erlaubt ist. |
| [GetAllowFiltering](./getallowfiltering/) | Gibt an, ob der Benutzer einen AutoFilter verwenden darf, der erstellt wurde, bevor das Blatt geschützt wurde. |
| [SetAllowFiltering](./setallowfiltering/) | Gibt an, ob der Benutzer einen AutoFilter verwenden darf, der erstellt wurde, bevor das Blatt geschützt wurde. |
| [GetAllowFormattingCell](./getallowformattingcell/) | Gibt an, ob das Formatieren von Zellen in einem geschützten Arbeitsblatt erlaubt ist. |
| [SetAllowFormattingCell](./setallowformattingcell/) | Gibt an, ob das Formatieren von Zellen in einem geschützten Arbeitsblatt erlaubt ist. |
| [GetAllowFormattingColumn](./getallowformattingcolumn/) | Gibt an, ob das Formatieren von Spalten in einem geschützten Arbeitsblatt erlaubt ist |
| [SetAllowFormattingColumn](./setallowformattingcolumn/) | Gibt an, ob das Formatieren von Spalten in einem geschützten Arbeitsblatt erlaubt ist |
| [GetAllowFormattingRow](./getallowformattingrow/) | Gibt an, ob das Formatieren von Zeilen in einem geschützten Arbeitsblatt erlaubt ist |
| [SetAllowFormattingRow](./setallowformattingrow/) | Gibt an, ob das Formatieren von Zeilen in einem geschützten Arbeitsblatt erlaubt ist |
| [GetAllowInsertingColumn](./getallowinsertingcolumn/) | Gibt an, ob das Einfügen von Spalten in einem geschützten Arbeitsblatt erlaubt ist |
| [SetAllowInsertingColumn](./setallowinsertingcolumn/) | Gibt an, ob das Einfügen von Spalten in einem geschützten Arbeitsblatt erlaubt ist |
| [GetAllowInsertingHyperlink](./getallowinsertinghyperlink/) | Gibt an, ob das Einfügen von Hyperlinks in einem geschützten Arbeitsblatt erlaubt ist |
| [SetAllowInsertingHyperlink](./setallowinsertinghyperlink/) | Gibt an, ob das Einfügen von Hyperlinks in einem geschützten Arbeitsblatt erlaubt ist |
| [GetAllowInsertingRow](./getallowinsertingrow/) | Gibt an, ob das Einfügen von Zeilen in einem geschützten Arbeitsblatt erlaubt ist |
| [SetAllowInsertingRow](./setallowinsertingrow/) | Gibt an, ob das Einfügen von Zeilen in einem geschützten Arbeitsblatt erlaubt ist |
| [GetAllowSorting](./getallowsorting/) | Gibt an, ob die Sortieroption in einem geschützten Arbeitsblatt erlaubt ist. |
| [SetAllowSorting](./setallowsorting/) | Gibt an, ob die Sortieroption in einem geschützten Arbeitsblatt erlaubt ist. |
| [GetAllowUsingPivotTable](./getallowusingpivottable/) | Gibt an, ob der Benutzer Pivot-Tabellen in einem geschützten Arbeitsblatt manipulieren darf. |
| [SetAllowUsingPivotTable](./setallowusingpivottable/) | Gibt an, ob der Benutzer Pivot-Tabellen in einem geschützten Arbeitsblatt manipulieren darf. |
| [GetAllowEditingContent](./getalloweditingcontent/) | Gibt an, ob der Benutzer Inhalte gesperrter Zellen in einem geschützten Arbeitsblatt bearbeiten darf. |
| [SetAllowEditingContent](./setalloweditingcontent/) | Gibt an, ob der Benutzer Inhalte gesperrter Zellen in einem geschützten Arbeitsblatt bearbeiten darf. |
| [GetAllowEditingObject](./getalloweditingobject/) | Gibt an, ob der Benutzer Zeichenobjekte in einem geschützten Arbeitsblatt manipulieren darf. |
| [SetAllowEditingObject](./setalloweditingobject/) | Gibt an, ob der Benutzer Zeichenobjekte in einem geschützten Arbeitsblatt manipulieren darf. |
| [GetAllowEditingScenario](./getalloweditingscenario/) | Gibt an, ob der Benutzer Szenarien in einem geschützten Arbeitsblatt bearbeiten darf. |
| [SetAllowEditingScenario](./setalloweditingscenario/) | Gibt an, ob der Benutzer Szenarien in einem geschützten Arbeitsblatt bearbeiten darf. |
| [GetAllowSelectingLockedCell](./getallowselectinglockedcell/) | Gibt an, ob der Benutzer gesperrte Zellen in einem geschützten Arbeitsblatt auswählen darf. |
| [SetAllowSelectingLockedCell](./setallowselectinglockedcell/) | Gibt an, ob der Benutzer gesperrte Zellen in einem geschützten Arbeitsblatt auswählen darf. |
| [GetAllowSelectingUnlockedCell](./getallowselectingunlockedcell/) | Gibt an, ob der Benutzer entsperrte Zellen in einem geschützten Arbeitsblatt auswählen darf. |
| [SetAllowSelectingUnlockedCell](./setallowselectingunlockedcell/) | Gibt an, ob der Benutzer entsperrte Zellen in einem geschützten Arbeitsblatt auswählen darf. |
| [GetPassword](./getpassword/) | Gibt das Passwort zum Schutz des Arbeitsblatts an. |
| [SetPassword](./setpassword/) | Gibt das Passwort zum Schutz des Arbeitsblatts an. |
| [IsProtectedWithPassword](./isprotectedwithpassword/) | Gibt an, ob das Arbeitsblatt mit einem Passwort geschützt ist. |
| [VerifyPassword](./verifypassword/) | Überprüft das Passwort. |
| [GetPasswordHash](./getpasswordhash/) | Ermittelt den Hash des aktuellen Passworts. |
