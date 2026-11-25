---
title: "ListObject.PutCellValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ListObject. Inserisce il valore nella cella"
type: docs
url: /it/net/aspose.cells.tables/listobject/putcellvalue/
---
## PutCellValue(int, int, object) {#putcellvalue}

Inserisci il valore nella cella.

```csharp
public void PutCellValue(int rowOffset, int columnOffset, object value)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowOffset | Int32 | L'offset di riga nella tabella. |
| columnOffset | Int32 | L'offset di colonna nella tabella. |
| valore | Object | Il valore della cella. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodPutCellValueWithInt32Int32ObjectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["C1"].PutValue("Column3");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["C2"].PutValue(300);

            // Crea un oggetto elenco
            int index = worksheet.ListObjects.Add(0, 0, 2, 2, true);
            ListObject listObject = worksheet.ListObjects[index];

            // Dimostra PutCellValue con parametri Int32, Int32, Object
            listObject.PutCellValue(1, 0, 500); // Update row 1, column 0 with value 500
            listObject.PutCellValue(1, 1, "Updated Value"); // Update row 1, column 1 with string
            listObject.PutCellValue(1, 2, DateTime.Now); // Update row 1, column 2 with current date

            // Salva la cartella di lavoro
            workbook.Save("ListObjectPutCellValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## PutCellValue(int, int, object, bool) {#putcellvalue_1}

Inserisci il valore nella cella.

```csharp
public void PutCellValue(int rowOffset, int columnOffset, object value, bool isTotalsRowLabel)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowOffset | Int32 | L'offset di riga nella tabella. |
| columnOffset | Int32 | L'offset di colonna nella tabella. |
| valore | Object | Il valore della cella. |
| isTotalsRowLabel | Booleano | Indica se è un'etichetta per la riga totale, funziona solo per la riga totale. Se False e questa riga è la riga totale, verrà inserita una nuova riga. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodPutCellValueWithInt32Int32ObjectBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per creare un ListObject
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");
            
            // Crea un ListObject
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[index];
            
            // Usa PutCellValue per aggiornare una cella (riga 2, colonna 1) con un nuovo valore ed espandere la tabella
            listObject.PutCellValue(2, 1, "Updated Value", true);
            
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


