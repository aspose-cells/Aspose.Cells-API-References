---
title: Protection
second_title: Aspose.Cells für .NET-API-Referenz
description: Stellt die verschiedenen Arten von Schutzoptionen dar die für ein Arbeitsblatt verfügbar sind.
type: docs
weight: 4910
url: /de/net/aspose.cells/protection/
---
## Protection class

Stellt die verschiedenen Arten von Schutzoptionen dar, die für ein Arbeitsblatt verfügbar sind.

```csharp
public class Protection
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AllowDeletingColumn](../../aspose.cells/protection/allowdeletingcolumn) { get; set; } | Stellt dar, ob das Löschen von Spalten auf einem geschützten Arbeitsblatt zulässig ist. |
| [AllowDeletingRow](../../aspose.cells/protection/allowdeletingrow) { get; set; } | Stellt dar, ob das Löschen von Zeilen auf einem geschützten Arbeitsblatt zulässig ist. |
| [AllowEditingContent](../../aspose.cells/protection/alloweditingcontent) { get; set; } | Stellt dar, ob der Benutzer den Inhalt gesperrter Zellen auf einem geschützten Arbeitsblatt bearbeiten darf. |
| [AllowEditingObject](../../aspose.cells/protection/alloweditingobject) { get; set; } | Stellt dar, ob der Benutzer Zeichnungsobjekte auf einem geschützten Arbeitsblatt bearbeiten darf. |
| [AllowEditingScenario](../../aspose.cells/protection/alloweditingscenario) { get; set; } | Stellt dar, ob der Benutzer berechtigt ist, Szenarien auf einem geschützten Arbeitsblatt zu bearbeiten. |
| [AllowFiltering](../../aspose.cells/protection/allowfiltering) { get; set; } | Stellt dar, ob der Benutzer einen AutoFilter verwenden darf, der erstellt wurde, bevor das Blatt geschützt wurde. |
| [AllowFormattingCell](../../aspose.cells/protection/allowformattingcell) { get; set; } | Gibt an, ob die Formatierung von Zellen auf einem geschützten Arbeitsblatt zulässig ist. |
| [AllowFormattingColumn](../../aspose.cells/protection/allowformattingcolumn) { get; set; } | Stellt dar, ob die Formatierung von Spalten auf einem geschützten Arbeitsblatt zulässig ist |
| [AllowFormattingRow](../../aspose.cells/protection/allowformattingrow) { get; set; } | Stellt dar, ob die Formatierung von Zeilen auf einem geschützten Arbeitsblatt zulässig ist |
| [AllowInsertingColumn](../../aspose.cells/protection/allowinsertingcolumn) { get; set; } | Stellt dar, ob das Einfügen von Spalten auf einem geschützten Arbeitsblatt erlaubt ist |
| [AllowInsertingHyperlink](../../aspose.cells/protection/allowinsertinghyperlink) { get; set; } | Stellt dar, ob das Einfügen von Hyperlinks auf einem geschützten Arbeitsblatt erlaubt ist |
| [AllowInsertingRow](../../aspose.cells/protection/allowinsertingrow) { get; set; } | Stellt dar, ob das Einfügen von Zeilen auf einem geschützten Arbeitsblatt erlaubt ist |
| [AllowSelectingLockedCell](../../aspose.cells/protection/allowselectinglockedcell) { get; set; } | Stellt dar, ob der Benutzer gesperrte Zellen auf einem geschützten Arbeitsblatt auswählen darf. |
| [AllowSelectingUnlockedCell](../../aspose.cells/protection/allowselectingunlockedcell) { get; set; } | Stellt dar, ob der Benutzer entsperrte Zellen auf einem geschützten Arbeitsblatt auswählen darf. |
| [AllowSorting](../../aspose.cells/protection/allowsorting) { get; set; } | Gibt an, ob die Sortieroption auf einem geschützten Arbeitsblatt zulässig ist. |
| [AllowUsingPivotTable](../../aspose.cells/protection/allowusingpivottable) { get; set; } | Stellt dar, ob der Benutzer Pivot-Tabellen auf einem geschützten Arbeitsblatt bearbeiten darf. |
| [IsProtectedWithPassword](../../aspose.cells/protection/isprotectedwithpassword) { get; } | Gibt an, ob die Arbeitsblätter passwortgeschützt sind. |
| [Password](../../aspose.cells/protection/password) { get; set; } | Stellt das Passwort dar, um das Arbeitsblatt zu schützen. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Copy](../../aspose.cells/protection/copy)(Protection) | Kopierschutzinfo. |
| [GetPasswordHash](../../aspose.cells/protection/getpasswordhash)() | Ruft den Hash des aktuellen Passworts ab. |
| [VerifyPassword](../../aspose.cells/protection/verifypassword)(string) | Verifiziert das Passwort. |

### Beispiele

```csharp

[C#]
//Instanziieren eines Workbook-Objekts
Workbook workbook = new Workbook();

Worksheet worksheet = workbook.Worksheets[0];
// Benutzern erlauben, gesperrte Zellen des Arbeitsblatts auszuwählen
worksheet.Protection.AllowSelectingLockedCell = true;
// Benutzern erlauben, entsperrte Zellen des Arbeitsblatts auszuwählen
worksheet.Protection.AllowSelectingUnlockedCell = true;  

[Visual Basic]

'Instanziieren eines Workbook-Objekts
Dim workbook As Workbook = New Workbook()
Dim worksheet As Worksheet = workbook.Worksheets(0)
'Ermöglicht Benutzern, gesperrte Zellen des Arbeitsblatts auszuwählen
worksheet.Protection.AllowSelectingLockedCell = True
'Ermöglicht Benutzern, nicht gesperrte Zellen des Arbeitsblatts auszuwählen
worksheet.Protection.AllowSelectingUnlockedCell = True
```

### Siehe auch

* namensraum [Aspose.Cells](../../aspose.cells)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
