---
title: "SeriesCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SeriesCollection. Aggiunge la collezione Series a un grafico"
type: docs
url: /it/net/aspose.cells.charts/seriescollection/add/
---
## Add(string, bool) {#add}

Aggiunge la collezione [`Series`](../../series/) a un grafico.

```csharp
public int Add(string dataArea, bool isVertical)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dataArea | String | Specifica i valori da cui tracciare la serie di dati |
| isVertical | Boolean | Specifica se tracciare la serie da un intervallo di valori di celle per riga o per colonna. Se vero, [`Series`](../../series/) verrà aggiunta colonna per colonna |

### Valore di ritorno

Restituisce il primo indice della ASeries aggiunta in NSeries.

### Osservazioni

Se i dati sono impostati su celle contigue, usa i due punti per separarle. Ad esempio, $C$2:$C$5. Se i dati sono impostati su celle non contigue, usa la virgola per separarle. Ad esempio: ($C$2,$D$5). Questo metodo elabora semplicemente *dataArea* come intervallo di dati. Se desideri verificare in modo intelligente il metodo ChartCollection.Add().

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodAddWithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(30);

            // Crea grafico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Aggiungi serie usando parametri stringa e booleani
            chart.NSeries.Add("=Sheet1!A1:B4", true);
            
            // Salva la cartella di lavoro
            workbook.Save("SeriesCollectionMethodAddWithStringBooleanDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, bool, bool) {#add_1}

Aggiunge la collezione [`Series`](../../series/) a un grafico.

```csharp
public int Add(string area, bool isVertical, bool checkLabels)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| area | String | Specifica i valori da cui tracciare la serie di dati |
| isVertical | Booleano | Specifica se tracciare la serie da un intervallo di valori di cella per riga o per colonna. |
| checkLabels | Booleano | Indica se l'intervallo contiene il nome della serie |

### Valore di ritorno

Restituisce il primo indice della ASeries aggiunta in NSeries.

### Osservazioni

Se i dati sono impostati su celle contigue, usa i due punti per separarle. Ad esempio, $C$2:$C$5. Se i dati sono impostati su celle non contigue, usa la virgola per separarle. Ad esempio, ($C$2,$D$5).

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodAddWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("Category1");
            sheet.Cells["A2"].PutValue(10);
            sheet.Cells["A3"].PutValue(20);
            sheet.Cells["B1"].PutValue("Category2");
            sheet.Cells["B2"].PutValue(30);
            sheet.Cells["B3"].PutValue(40);

            // Crea grafico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Aggiungi serie usando il metodo Add con parametri stringa e booleani
            chart.NSeries.Add("=Sheet1!$B$2:$B$3", true, false);
            chart.NSeries.CategoryData = "=Sheet1!$A$1:$B$1";
            
            // Salva la cartella di lavoro
            wb.Save("SeriesCollectionMethodAddWithStringBooleanBooleanDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


