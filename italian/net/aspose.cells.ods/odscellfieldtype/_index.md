---
title: "Enum OdsCellFieldType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Ods.OdsCellFieldType enum. Rappresenta il tipo di campo cella di ods"
type: docs
url: /it/net/aspose.cells.ods/odscellfieldtype/
---
## OdsCellFieldType enumeration

Rappresenta il tipo di campo cella di ODS.

```csharp
public enum OdsCellFieldType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Date | `0` | Data corrente. |
| SheetName | `1` | Il nome del foglio. |
| Title | `2` | Il nome del file. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una OdsCellFieldCollection
            OdsCellFieldCollection odsCellFields = worksheet.Cells.OdsCellFields;

            // Aggiungi un nuovo OdsCellField per la data corrente
            int rowIndex = 0;
            int columnIndex = 0;
            string customFormat = "yyyy-mm-dd";
            odsCellFields.Add(rowIndex, columnIndex, OdsCellFieldType.Date, customFormat);

            // Aggiungi un altro OdsCellField per il nome del foglio
            rowIndex = 1;
            columnIndex = 0;
            odsCellFields.Add(rowIndex, columnIndex, OdsCellFieldType.SheetName, null);

            // Aggiungi un altro OdsCellField per il titolo
            rowIndex = 2;
            columnIndex = 0;
            odsCellFields.Add(rowIndex, columnIndex, OdsCellFieldType.Title, null);

            // Aggiorna il valore dei campi nelle celle
            odsCellFields.UpdateFieldsValue();

            // Stampa i valori nella console
            for (int i = 0; i < odsCellFields.Count; i++)
            {
                OdsCellField field = odsCellFields[i];
                worksheet.Cells[field.Row, field.Column].PutValue($"Field Type: {field.FieldType}, Custom Format: {field.CustomFormat}");
            }

            // Salva la cartella di lavoro
            workbook.Save("OdsCellFieldTypeExample.ods");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


