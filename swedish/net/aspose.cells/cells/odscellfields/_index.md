---
title: "Cells.OdsCellFields"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-egenskap. Hämtar listan över fält i ods"
type: docs
url: /sv/net/aspose.cells/cells/odscellfields/
---
## Cells.OdsCellFields property

Hämtar listan över fält i ods.

```csharp
public OdsCellFieldCollection OdsCellFields { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsPropertyOdsCellFieldsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Hämta Cells-samlingen
            Cells cells = worksheet.Cells;

            try
            {
                // Åtkomst till OdsCellFields-egenskapen (skrivskyddad)
                var odsCellFields = cells.OdsCellFields;

                // Visa information om OdsCellFields-samlingen
                Console.WriteLine("OdsCellFields collection count: " + odsCellFields.Count);

                // Iterera genom OdsCellFields-samlingen
                for (int i = 0; i < odsCellFields.Count; i++)
                {
                    var field = odsCellFields[i];
                    Console.WriteLine($"Field {i}: Type - {field.FieldType}");
                }

                // Demonstrera uppdatering av fältvärden
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

### Se även

* class [OdsCellFieldCollection](../../../aspose.cells.ods/odscellfieldcollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


