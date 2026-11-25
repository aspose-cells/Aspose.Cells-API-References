---
title: "Worksheet.AdvancedFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Filtra i dati usando criteri complessi"
type: docs
url: /it/net/aspose.cells/worksheet/advancedfilter/
---
## Worksheet.AdvancedFilter method

Filtra i dati usando criteri complessi.

```csharp
public void AdvancedFilter(bool isFilter, string listRange, string criteriaRange, string copyTo, 
    bool uniqueRecordOnly)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isFilter | Booleano | Indica se filtrare l'elenco in loco. |
| listRange | String | L'intervallo dell'elenco. |
| criteriaRange | String | L'intervallo dei criteri. |
| copyTo | String | L'intervallo dove copiare i dati. |
| uniqueRecordOnly | Booleano | Solo visualizzare o copiare righe uniche. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAdvancedFilterWithBooleanStringStringStringBooleDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio per il filtraggio
            // Intestazioni
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["C1"].PutValue("Price");
            
            // Criteri
            worksheet.Cells["A2"].PutValue("Product");
            worksheet.Cells["B2"].PutValue("Category");
            worksheet.Cells["C2"].PutValue("Fruits");
            
            // Dati
            worksheet.Cells["A4"].PutValue("Apple");
            worksheet.Cells["B4"].PutValue("Fruits");
            worksheet.Cells["C4"].PutValue(2.5);
            
            worksheet.Cells["A5"].PutValue("Carrot");
            worksheet.Cells["B5"].PutValue("Vegetables");
            worksheet.Cells["C5"].PutValue(1.2);
            
            worksheet.Cells["A6"].PutValue("Banana");
            worksheet.Cells["B6"].PutValue("Fruits");
            worksheet.Cells["C6"].PutValue(1.8);

            // Applica filtro avanzato (filtra in loco, solo record unici)
            worksheet.AdvancedFilter(false, "A4:C6", "A1:C2", null, true);

            // Salva la cartella di lavoro
            workbook.Save("AdvancedFilterDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


