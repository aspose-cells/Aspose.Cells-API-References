---
title: "OdsCellField.Column"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OdsCellField. Ottiene e imposta l'indice di colonna della cella"
type: docs
url: /it/net/aspose.cells.ods/odscellfield/column/
---
## OdsCellField.Column property

Ottiene e imposta l'indice di colonna della cella.

```csharp
public int Column { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsCellFieldPropertyColumnDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            OdsCellFieldCollection odsCellFields = worksheet.Cells.OdsCellFields;

            // Aggiungi campi con tipi diversi e dimostra la proprietà Column
            odsCellFields.Add(0, 2, OdsCellFieldType.Date, "yyyy-mm-dd");
            odsCellFields.Add(1, 3, OdsCellFieldType.SheetName, null);
            odsCellFields.Add(2, 4, OdsCellFieldType.Title, null);

            // Accedi e visualizza la proprietà Column
            Console.WriteLine("Field Columns:");
            foreach (OdsCellField field in odsCellFields)
            {
                Console.WriteLine($"Type: {field.FieldType}, Column: {field.Column}");
                worksheet.Cells[field.Row, field.Column].PutValue($"Column: {field.Column}");
            }

            odsCellFields.UpdateFieldsValue();
            workbook.Save("OdsCellFieldColumnDemo.ods");
        }
    }
}
```

### Vedi anche

* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


