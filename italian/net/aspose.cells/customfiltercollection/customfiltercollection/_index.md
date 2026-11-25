---
title: "CustomFilterCollection.CustomFilterCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore CustomFilterCollection. Costruisce una nuova istanza"
type: docs
url: /it/net/aspose.cells/customfiltercollection/customfiltercollection/
---
## CustomFilterCollection constructor

Costruisce una nuova istanza.

```csharp
[Obsolete("Use FilterColumn.CustomFilters, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public CustomFilterCollection()
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, imposta FilterColumn.FilterType su FilterType.CustomFilters e poi ottieni FilterColumn.CustomFilters. Questa proprietà sarà rimossa tra 12 mesi a partire da giugno 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterCollectionMethodSharpctorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].Value = "Numbers";
            worksheet.Cells["A2"].Value = 10;
            worksheet.Cells["A3"].Value = 20;
            worksheet.Cells["A4"].Value = 30;
            worksheet.Cells["A5"].Value = 40;
            worksheet.Cells["A6"].Value = 50;

            try
            {
                // Crea una nuova CustomFilterCollection usando il costruttore
                CustomFilterCollection filters = new CustomFilterCollection();

                // Visualizza il valore predefinito della proprietà And
                Console.WriteLine($"Default And property value: {filters.And}");

                // Il costruttore crea una collezione vuota
                Console.WriteLine($"Number of filters in collection: {filters.Count}");

                // Salva la cartella di lavoro
                workbook.Save("CustomFilterCollectionDemo.xlsx");
                Console.WriteLine("CustomFilterCollection created successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating CustomFilterCollection: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


