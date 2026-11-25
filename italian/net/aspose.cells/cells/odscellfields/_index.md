---
title: "Cells.OdsCellFields"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cells. Ottiene l'elenco dei campi di ods"
type: docs
url: /it/net/aspose.cells/cells/odscellfields/
---
## Cells.OdsCellFields property

Ottiene l'elenco dei campi di ods.

```csharp
public OdsCellFieldCollection OdsCellFields { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsPropertyOdsCellFieldsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Ottieni la collezione Cells
            Cells cells = worksheet.Cells;

            try
            {
                // Accedi alla proprietà OdsCellFields (sola lettura)
                var odsCellFields = cells.OdsCellFields;

                // Visualizza le informazioni sulla collezione OdsCellFields
                Console.WriteLine("OdsCellFields collection count: " + odsCellFields.Count);

                // Itera attraverso la collezione OdsCellFields
                for (int i = 0; i < odsCellFields.Count; i++)
                {
                    var field = odsCellFields[i];
                    Console.WriteLine($"Field {i}: Type - {field.FieldType}");
                }

                // Dimostra l'aggiornamento dei valori dei campi
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

### Vedi anche

* class [OdsCellFieldCollection](../../../aspose.cells.ods/odscellfieldcollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


