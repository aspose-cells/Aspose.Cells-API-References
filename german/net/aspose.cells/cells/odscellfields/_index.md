---
title: "Cells.OdsCellFields"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Eigenschaft. Gibt die Liste der Felder von ods zurück."
type: docs
url: /de/net/aspose.cells/cells/odscellfields/
---
## Cells.OdsCellFields property

Ruft die Liste der Felder von ods ab.

```csharp
public OdsCellFieldCollection OdsCellFields { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsPropertyOdsCellFieldsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Rufe die Cells-Sammlung ab.
            Cells cells = worksheet.Cells;

            try
            {
                // Greifen Sie auf die OdsCellFields-Eigenschaft zu (schreibgeschützt).
                var odsCellFields = cells.OdsCellFields;

                // Informationen über die OdsCellFields-Sammlung anzeigen.
                Console.WriteLine("OdsCellFields collection count: " + odsCellFields.Count);

                // Durchlaufen Sie die OdsCellFields-Sammlung.
                for (int i = 0; i < odsCellFields.Count; i++)
                {
                    var field = odsCellFields[i];
                    Console.WriteLine($"Field {i}: Type - {field.FieldType}");
                }

                // Demonstrieren Sie das Aktualisieren von Feldwerten.
                odsCellFields.UpdateFieldsValue();

                Console.WriteLine("OdsCellFields demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [OdsCellFieldCollection](../../../aspose.cells.ods/odscellfieldcollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


