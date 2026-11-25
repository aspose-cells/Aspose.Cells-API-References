---
title: "PivotPageFields.AddIdentify"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotPageFields. Imposta quale etichetta dell'elemento in ogni campo pagina utilizzare per identificare l'intervallo di dati. La lunghezza di pageItemIndex deve essere uguale a PageFieldCount, quindi aggiungi prima il campo pagina."
type: docs
url: /it/net/aspose.cells.pivot/pivotpagefields/addidentify/
---
## PivotPageFields.AddIdentify method

Imposta quale etichetta dell'elemento in ogni campo di pagina utilizzare per identificare l'intervallo dati. La lunghezza di pageItemIndex deve essere uguale a PageFieldCount, quindi aggiungi prima il campo di pagina.

```csharp
public void AddIdentify(int rangeIndex, int[] pageItemIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rangeIndex | Int32 | L'indice dell'intervallo di dati di consolidamento. |
| pageItemIndex | Int32[] | L'indice dell'elemento pagina in ciascun campo pagina. pageItemIndex[2] = 1 significa che il secondo elemento nel terzo campo viene usato per identificare questo intervallo. pageItemIndex[1] = -1 significa che nessun elemento nel secondo campo viene usato per identificare questo intervallo e MS creerà automaticamente un elemento "blank" nel secondo campo per identificare questo intervallo. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotPageFieldsMethodAddIdentifyWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["B2"].PutValue("A");
            worksheet.Cells["B3"].PutValue("B");
            worksheet.Cells["B4"].PutValue("C");

            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "E5", "PivotTable");
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // Istanzia direttamente PivotPageFields invece di accedere tramite PivotTable
            PivotPageFields pageFields = new PivotPageFields();

            try
            {
                pageFields.AddIdentify(0, new int[] { 0, 1 });
                Console.WriteLine("AddIdentify executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("PivotPageFieldsMethodAddIdentifyWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


