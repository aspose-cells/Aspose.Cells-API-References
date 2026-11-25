---
title: "WorksheetCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo WorksheetCollection. Aggiunge un foglio di lavoro alla collezione"
type: docs
url: /it/net/aspose.cells/worksheetcollection/add/
---
## Add(SheetType) {#add_2}

Aggiunge un foglio di lavoro alla collezione.

```csharp
public int Add(SheetType type)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | SheetType | Tipo Worksheet. |

### Valore di ritorno

[`Worksheet`](../../worksheet/) object index.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodAddWithSheetTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Aggiungi un nuovo foglio grafico usando il parametro SheetType
            workbook.Worksheets.Add(SheetType.Chart);
            
            // Aggiungi dati al primo foglio di lavoro
            Cells cells = workbook.Worksheets[0].Cells;
            cells["C2"].PutValue(5000);
            cells["C3"].PutValue(3000);
            cells["C4"].PutValue(4000);
            cells["C5"].PutValue(5000);
            cells["C6"].PutValue(6000);
            
            // Crea un grafico nel foglio grafico
            Aspose.Cells.Charts.ChartCollection charts = workbook.Worksheets[1].Charts;
            int chartIndex = charts.Add(Aspose.Cells.Charts.ChartType.Column, 10, 10, 20, 20);
            Aspose.Cells.Charts.Chart chart = charts[chartIndex];
            chart.NSeries.Add("Sheet1!C2:C6", true);
            
            // Salva la cartella di lavoro (opzionale)
            // workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* enum [SheetType](../../sheettype/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add() {#add_1}

Aggiunge un foglio di lavoro alla collezione.

```csharp
public int Add()
```

### Valore di ritorno

[`Worksheet`](../../worksheet/) object index.

### Vedi anche

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add}

Aggiunge un foglio di lavoro alla collezione.

```csharp
public Worksheet Add(string sheetName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetName | String | Nome foglio di lavoro |

### Valore di ritorno

[`Worksheet`](../../worksheet/) object.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets.Add("NewSheet");
            
            // Aggiungi dati al nuovo foglio di lavoro
            worksheet.Cells["A1"].PutValue("Worksheet added successfully!");
            
            // Salva la cartella di lavoro
            wb.Save("WorksheetCollectionMethodAddWithStringDemo_output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


