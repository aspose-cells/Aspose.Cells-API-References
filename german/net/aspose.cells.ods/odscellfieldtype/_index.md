---
title: "Enum OdsCellFieldType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Ods.OdsCellFieldType enum. Stellt den Zellenfeldtyp von ods dar"
type: docs
url: /de/net/aspose.cells.ods/odscellfieldtype/
---
## OdsCellFieldType enumeration

Stellt den Zellfeldtyp von ODS dar.

```csharp
public enum OdsCellFieldType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Date | `0` | Aktuelles Datum. |
| SheetName | `1` | Der Name des Blatts. |
| Title | `2` | Der Name der Datei. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;

    public class OdsCellFieldTypeDemo
    {
        public static void OdsCellFieldTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine OdsCellFieldCollection
            OdsCellFieldCollection odsCellFields = worksheet.Cells.OdsCellFields;

            // Füge ein neues OdsCellField für das aktuelle Datum hinzu
            int rowIndex = 0;
            int columnIndex = 0;
            string customFormat = "yyyy-mm-dd";
            odsCellFields.Add(rowIndex, columnIndex, OdsCellFieldType.Date, customFormat);

            // Füge ein weiteres OdsCellField für den Blattnamen hinzu
            rowIndex = 1;
            columnIndex = 0;
            odsCellFields.Add(rowIndex, columnIndex, OdsCellFieldType.SheetName, null);

            // Füge ein weiteres OdsCellField für den Titel hinzu
            rowIndex = 2;
            columnIndex = 0;
            odsCellFields.Add(rowIndex, columnIndex, OdsCellFieldType.Title, null);

            // Aktualisiere den Feldwert in den Zellen
            odsCellFields.UpdateFieldsValue();

            // Gib die Werte in der Konsole aus
            for (int i = 0; i < odsCellFields.Count; i++)
            {
                OdsCellField field = odsCellFields[i];
                worksheet.Cells[field.Row, field.Column].PutValue($"Field Type: {field.FieldType}, Custom Format: {field.CustomFormat}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("OdsCellFieldTypeExample.ods");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


