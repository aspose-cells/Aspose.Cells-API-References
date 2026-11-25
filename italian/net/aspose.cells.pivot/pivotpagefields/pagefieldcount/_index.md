---
title: "PivotPageFields.PageFieldCount"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotPageFields. Restituisce il numero di campi pagina"
type: docs
url: /it/net/aspose.cells.pivot/pivotpagefields/pagefieldcount/
---
## PivotPageFields.PageFieldCount property

Ottiene il numero di campi di pagina.

```csharp
public int PageFieldCount { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotPageFieldsPropertyPageFieldCountDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Crea fogli di lavoro di esempio con dati
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "Data1";
            FillSampleData(sheet1);

            Worksheet sheet2 = workbook.Worksheets.Add("Data2");
            FillSampleData(sheet2);

            // Crea un foglio pivot
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");

            // Crea un'istanza di PivotPageFields
            PivotPageFields pageFields = new PivotPageFields();

            // Aggiungi campi pagina per dimostrare la proprietà PageFieldCount
            pageFields.AddPageField(new string[] { "Category1", "Category2" });
            pageFields.AddPageField(new string[] { "Region1", "Region2" });

            try
            {
                // Visualizza il valore della proprietà PageFieldCount
                Console.WriteLine("Number of page fields: " + pageFields.PageFieldCount);

                // Aggiungi l'identificazione per i campi della pagina
                pageFields.AddIdentify(0, new int[] { 0, 1 });
                pageFields.AddIdentify(1, new int[] { 1, 0 });

                // Verifica che il conteggio rimanga lo stesso dopo aver aggiunto le identificazioni
                Console.WriteLine("PageFieldCount after adding identifications: " + pageFields.PageFieldCount);

                // Crea una tabella pivot utilizzando i campi della pagina
                string[] sources = { "=Data1!A1:C4", "=Data2!A1:C4" };
                pivotSheet.PivotTables.Add(sources, false, pageFields, "E3", "DemoPivot");

                // Salva la cartella di lavoro
                workbook.Save("PageFieldCountDemo.xlsx");
                Console.WriteLine("Demo completed successfully. File saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private static void FillSampleData(Worksheet sheet)
        {
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Category");
            cells["B1"].PutValue("Region");
            cells["C1"].PutValue("Value");

            cells["A2"].PutValue("Category1");
            cells["B2"].PutValue("Region1");
            cells["C2"].PutValue(100);

            cells["A3"].PutValue("Category2");
            cells["B3"].PutValue("Region2");
            cells["C3"].PutValue(200);
        }
    }
}
```

### Vedi anche

* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


