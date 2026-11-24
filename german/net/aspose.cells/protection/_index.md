---
title: "Klasse Protection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Protection Klasse. Stellt die verschiedenen Arten von Schutzoptionen für ein Arbeitsblatt dar"
type: docs
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
| [AllowDeletingColumn](../../aspose.cells/protection/allowdeletingcolumn/) { get; set; } | Stellt dar, ob das Löschen von Spalten in einem geschützten Arbeitsblatt erlaubt ist. |
| [AllowDeletingRow](../../aspose.cells/protection/allowdeletingrow/) { get; set; } | Stellt dar, ob das Löschen von Zeilen in einem geschützten Arbeitsblatt erlaubt ist. |
| [AllowEditingContent](../../aspose.cells/protection/alloweditingcontent/) { get; set; } | Stellt dar, ob der Benutzer den Inhalt gesperrter Zellen in einem geschützten Arbeitsblatt bearbeiten darf. |
| [AllowEditingObject](../../aspose.cells/protection/alloweditingobject/) { get; set; } | Stellt dar, ob der Benutzer Zeichenobjekte in einem geschützten Arbeitsblatt manipulieren darf. |
| [AllowEditingScenario](../../aspose.cells/protection/alloweditingscenario/) { get; set; } | Stellt dar, ob der Benutzer Szenarien in einem geschützten Arbeitsblatt bearbeiten darf. |
| [AllowFiltering](../../aspose.cells/protection/allowfiltering/) { get; set; } | Stellt dar, ob der Benutzer einen AutoFilter, der vor dem Schutz des Blatts erstellt wurde, verwenden darf. |
| [AllowFormattingCell](../../aspose.cells/protection/allowformattingcell/) { get; set; } | Stellt dar, ob das Formatieren von Zellen in einem geschützten Arbeitsblatt erlaubt ist. |
| [AllowFormattingColumn](../../aspose.cells/protection/allowformattingcolumn/) { get; set; } | Stellt dar, ob das Formatieren von Spalten in einem geschützten Arbeitsblatt erlaubt ist |
| [AllowFormattingRow](../../aspose.cells/protection/allowformattingrow/) { get; set; } | Stellt dar, ob das Formatieren von Zeilen in einem geschützten Arbeitsblatt erlaubt ist |
| [AllowInsertingColumn](../../aspose.cells/protection/allowinsertingcolumn/) { get; set; } | Stellt dar, ob das Einfügen von Spalten in einem geschützten Arbeitsblatt erlaubt ist |
| [AllowInsertingHyperlink](../../aspose.cells/protection/allowinsertinghyperlink/) { get; set; } | Stellt dar, ob das Einfügen von Hyperlinks in einem geschützten Arbeitsblatt erlaubt ist |
| [AllowInsertingRow](../../aspose.cells/protection/allowinsertingrow/) { get; set; } | Stellt dar, ob das Einfügen von Zeilen in einem geschützten Arbeitsblatt erlaubt ist |
| [AllowSelectingLockedCell](../../aspose.cells/protection/allowselectinglockedcell/) { get; set; } | Stellt dar, ob der Benutzer gesperrte Zellen in einem geschützten Arbeitsblatt auswählen darf. |
| [AllowSelectingUnlockedCell](../../aspose.cells/protection/allowselectingunlockedcell/) { get; set; } | Stellt dar, ob der Benutzer entsperrte Zellen in einem geschützten Arbeitsblatt auswählen darf. |
| [AllowSorting](../../aspose.cells/protection/allowsorting/) { get; set; } | Stellt dar, ob die Sortieroption in einem geschützten Arbeitsblatt erlaubt ist. |
| [AllowUsingPivotTable](../../aspose.cells/protection/allowusingpivottable/) { get; set; } | Stellt dar, ob der Benutzer Pivot-Tabellen in einem geschützten Arbeitsblatt manipulieren darf. |
| [IsProtectedWithPassword](../../aspose.cells/protection/isprotectedwithpassword/) { get; } | Gibt an, ob das Arbeitsblatt mit einem Passwort geschützt ist. |
| [Password](../../aspose.cells/protection/password/) { get; set; } | Stellt das Passwort zum Schutz des Arbeitsblatts dar. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Copy](../../aspose.cells/protection/copy/)(Protection) | Schutzinformationen kopieren. |
| [GetPasswordHash](../../aspose.cells/protection/getpasswordhash/)() | Ermittelt den Hash des aktuellen Passworts. |
| [VerifyPassword](../../aspose.cells/protection/verifypassword/)(string) | Verifiziert das Passwort. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectionDemo
    {
        public static void ProtectionExample()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Zugriff auf die Schutz-Einstellungen des Arbeitsblatts
            Protection protection = worksheet.Protection;

            // Festlegen verschiedener Schutzeigenschaften
            protection.AllowDeletingColumn = true;
            protection.AllowDeletingRow = true;
            protection.AllowFiltering = true;
            protection.AllowFormattingCell = true;
            protection.AllowFormattingColumn = true;
            protection.AllowFormattingRow = true;
            protection.AllowInsertingColumn = true;
            protection.AllowInsertingHyperlink = true;
            protection.AllowInsertingRow = true;
            protection.AllowSorting = true;
            protection.AllowUsingPivotTable = true;
            protection.AllowEditingContent = true;
            protection.AllowEditingObject = true;
            protection.AllowEditingScenario = true;
            protection.Password = "password123";
            protection.AllowSelectingLockedCell = true;
            protection.AllowSelectingUnlockedCell = true;

            // Überprüfen, ob das Arbeitsblatt mit einem Passwort geschützt ist
            bool isProtectedWithPassword = protection.IsProtectedWithPassword;

            // Speichern der Arbeitsmappe
            workbook.Save("ProtectionExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


