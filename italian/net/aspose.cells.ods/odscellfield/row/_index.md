---
title: "OdsCellField.Row"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OdsCellField. Ottiene e imposta l'indice di riga della cella"
type: docs
url: /it/net/aspose.cells.ods/odscellfield/row/
---
## OdsCellField.Row property

Ottiene e imposta l'indice di riga della cella.

```csharp
public int Row { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsCellFieldPropertyRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            OdsCellFieldCollection odsCellFields = worksheet.Cells.OdsCellFields;
            
            // Aggiungi campi con tipi diversi
            odsCellFields.Add(0, 0, OdsCellFieldType.Date, "yyyy-mm-dd");
            odsCellFields.Add(1, 0, OdsCellFieldType.SheetName, null);
            odsCellFields.Add(2, 0, OdsCellFieldType.Title, null);
            
            odsCellFields.UpdateFieldsValue();

            // Dimostra l'uso della proprietà Row
            for (int i = 0; i < odsCellFields.Count; i++)
            {
                OdsCellField field = odsCellFields[i];
                int row = field.Row; // Using Row property
                worksheet.Cells[row, 1].PutValue($"Row: {row}, Type: {field.FieldType}");
            }

            workbook.Save("OdsCellFieldRowDemo.ods");
        }
    }
}
```

### Vedi anche

* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


