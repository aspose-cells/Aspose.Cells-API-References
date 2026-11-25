---
title: "ListObject.Filter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ListObject. Filtra la tabella"
type: docs
url: /it/net/aspose.cells.tables/listobject/filter/
---
## ListObject.Filter method

Filtra la tabella.

```csharp
[Obsolete("Use set ListObject.HasAutoFilter property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public AutoFilter Filter()
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, impostare la proprietà ListObject.HasAutoFilter./// Questa proprietà sarà rimossa tra 12 mesi a partire da ottobre 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListObjectMethodFilterDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola dati di esempio per list object
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Smartphone");
            worksheet.Cells["B3"].PutValue(800);
            worksheet.Cells["A4"].PutValue("Monitor");
            worksheet.Cells["B4"].PutValue(250);

            try
            {
                // Crea un list object dall'intervallo di dati usando ListObjects.Add con i parametri corretti
                int listObjectIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
                ListObject listObject = worksheet.ListObjects[listObjectIndex];
                
                // Ottieni AutoFilter tramite il metodo Filter
                AutoFilter autoFilter = listObject.Filter();

                // Applica il filtro sulla colonna Price (indice 1) per mostrare gli elementi >= 800
                autoFilter.Custom(1, FilterOperatorType.GreaterOrEqual, 800);

                Console.WriteLine("Filter applied successfully. Showing items with Price >= 800.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Filter method: {ex.Message}");
            }

            workbook.Save("ListObjectMethodFilterDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [AutoFilter](../../../aspose.cells/autofilter/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


