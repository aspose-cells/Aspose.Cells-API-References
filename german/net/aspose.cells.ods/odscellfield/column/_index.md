---
title: "OdsCellField.Column"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OdsCellField-Eigenschaft. Liest und setzt den Spaltenindex der Zelle"
type: docs
url: /de/net/aspose.cells.ods/odscellfield/column/
---
## OdsCellField.Column property

Liest und schreibt den Spaltenindex der Zelle.

```csharp
public int Column { get; set; }
```

### Beispiele

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

            // Felder mit unterschiedlichen Typen hinzufügen und die Column-Eigenschaft demonstrieren
            odsCellFields.Add(0, 2, OdsCellFieldType.Date, "yyyy-mm-dd");
            odsCellFields.Add(1, 3, OdsCellFieldType.SheetName, null);
            odsCellFields.Add(2, 4, OdsCellFieldType.Title, null);

            // Zugriff auf und Anzeige der Column-Eigenschaft
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

### Siehe auch

* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


