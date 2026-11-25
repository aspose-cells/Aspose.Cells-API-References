---
title: "ListObject.PutCellFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ListObject. Inserisce la formula nella cella della tabella"
type: docs
url: /it/net/aspose.cells.tables/listobject/putcellformula/
---
## PutCellFormula(int, int, string) {#putcellformula}

Inserisci la formula nella cella della tabella.

```csharp
public void PutCellFormula(int rowOffset, int columnOffset, string formula)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowOffset | Int32 | L'offset di riga nella tabella. |
| columnOffset | Int32 | L'offset di colonna nella tabella. |
| formula | String | La formula della cella. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodPutCellFormulaWithInt32Int32StringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Aggiungi dati di esempio per creare una tabella
            sheet.Cells["A1"].PutValue("ID");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["C1"].PutValue("Formula");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["B3"].PutValue(20);

            // Crea un oggetto lista (tabella)
            int index = sheet.ListObjects.Add("A1", "C3", true);
            ListObject table = sheet.ListObjects[index];

            // Aggiungi una nuova riga e imposta valori/formula
            table.PutCellValue(4, 0, 3); // Row 4, Column 0 (ID)
            table.PutCellValue(4, 1, 30); // Row 4, Column 1 (Value)
            table.PutCellFormula(4, 2, "=B3*2"); // Row 4, Column 2 (Formula)

            // Salva la cartella di lavoro
            wb.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## PutCellFormula(int, int, string, bool) {#putcellformula_1}

Inserisci la formula nella cella della tabella.

```csharp
public void PutCellFormula(int rowOffset, int columnOffset, string formula, bool isTotalsRowFormula)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowOffset | Int32 | L'offset di riga nella tabella. |
| columnOffset | Int32 | L'offset di colonna nella tabella. |
| formula | String | La formula della cella. |
| isTotalsRowFormula | Booleano |  |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodPutCellFormulaWithInt32Int32StringBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per creare un oggetto elenco
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            
            // Crea oggetto elenco
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            ListObject listObject = worksheet.ListObjects[index];
            
            // Dimostra PutCellFormula
            listObject.PutCellFormula(3, 0, "=SUM(A2:A3)", true);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


