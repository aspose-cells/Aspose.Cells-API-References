---
title: "WorksheetCollection.Insert"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo WorksheetCollection. Inserisci un foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheetcollection/insert/
---
## Insert(int, SheetType) {#insert}

Inserisci un foglio di lavoro.

```csharp
public Worksheet Insert(int index, SheetType sheetType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | L'indice del foglio |
| sheetType | SheetType | Il tipo di foglio. |

### Valore di ritorno

Restituisce un foglio di lavoro inserito.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodInsertWithInt32SheetTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets.Insert(1, SheetType.Worksheet);
            worksheet.Name = "InsertedSheet";
            workbook.Worksheets[0].Cells["A1"].Value = "Referencing inserted sheet:";
            workbook.Worksheets[0].Cells["A2"].Formula = "='InsertedSheet'!A1";
        }
    }
}
```

### Vedi anche

* class [Worksheet](../../worksheet/)
* enum [SheetType](../../sheettype/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Insert(int, SheetType, string) {#insert_1}

Inserisci un foglio di lavoro.

```csharp
public Worksheet Insert(int index, SheetType sheetType, string sheetName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | L'indice del foglio |
| sheetType | SheetType | Il tipo di foglio. |
| sheetName | String | Il nome del foglio. |

### Valore di ritorno

Restituisce un foglio di lavoro inserito.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodInsertWithInt32SheetTypeStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Inserisci un nuovo foglio di lavoro all'indice 0 con nome "InsertedSheet"
            workbook.Worksheets.Insert(0, SheetType.Worksheet, "InsertedSheet");
            
            // Accedi al foglio di lavoro inserito
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Inserisci dei dati nella cella A1 del foglio inserito
            worksheet.Cells["A1"].PutValue("This sheet was inserted using Insert method");
            
            // Salva la cartella di lavoro
            workbook.Save("WorksheetInsertDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../../worksheet/)
* enum [SheetType](../../sheettype/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


