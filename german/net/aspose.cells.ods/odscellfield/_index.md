---
title: "Klasse OdsCellField"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Ods.OdsCellField‑Klasse. Stellt das Zellfeld von ODS dar."
type: docs
url: /de/net/aspose.cells.ods/odscellfield/
---
## OdsCellField class

Stellt das Zellfeld von ODS dar.

```csharp
public class OdsCellField
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Column](../../aspose.cells.ods/odscellfield/column/) { get; set; } | Liest und schreibt den Spaltenindex der Zelle. |
| [CustomFormat](../../aspose.cells.ods/odscellfield/customformat/) { get; set; } | Stellt das benutzerdefinierte Format des Feldwerts dar. |
| [FieldType](../../aspose.cells.ods/odscellfield/fieldtype/) { get; set; } | Liest und schreibt den Typ des Feldes. |
| [Row](../../aspose.cells.ods/odscellfield/row/) { get; set; } | Liest und schreibt den Zeilenindex der Zelle. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Ods;

    public class OdsClassOdsCellFieldDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            try
            {
                // -----------------------------------------------------------------
                // 1. Erstelle ein OdsCellField über die Sammlung (kein parameterloser Konstruktor)
                // -----------------------------------------------------------------
                OdsCellFieldCollection odsFields = sheet.Cells.OdsCellFields;
                odsFields.Add(2, 1, OdsCellFieldType.Title, "Demo Title");

                // Rufe das Feld ab, das wir gerade hinzugefügt haben
                OdsCellField manualField = odsFields[odsFields.Count - 1];

                // Schreibe etwas in die Zelle, die durch das OdsCellField identifiziert wird
                sheet.Cells[manualField.Row, manualField.Column].PutValue("Manual Field");

                // --------------------------------------------------------------
                // 2. Füge dasselbe Feld erneut hinzu, um die Verwendung der Sammlung zu demonstrieren (optional)
                // --------------------------------------------------------------
                odsFields.Add(manualField.Row, manualField.Column, manualField.FieldType, manualField.CustomFormat);

                // Aktualisiere alle ODS‑Felder, damit sie in der gespeicherten Datei berücksichtigt werden
                odsFields.UpdateFieldsValue();

                // Gib die Eigenschaftswerte in der Konsole aus
                Console.WriteLine($"Created OdsCellField -> Row: {manualField.Row}, Column: {manualField.Column}, " +
                                  $"Type: {manualField.FieldType}, Format: {manualField.CustomFormat}");

                // Speichere die Arbeitsmappe als ODS‑Datei
                workbook.Save("OdsClassOdsCellFieldDemo.ods");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while working with OdsCellField: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


