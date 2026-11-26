---
title: "SeriesCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SeriesCollection. Añade la colección Series a un gráfico"
type: docs
url: /es/net/aspose.cells.charts/seriescollection/add/
---
## Add(string, bool) {#add}

Añade la colección [`Series`](../../series/) a un gráfico.

```csharp
public int Add(string dataArea, bool isVertical)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dataArea | String | Especifica los valores a partir de los cuales trazar la serie de datos |
| isVertical | Boolean | Especifica si se deben trazar las series a partir de un rango de valores de celdas por fila o por columna. Si es verdadero, [`Series`](../../series/) se añadirá columna por columna |

### Valor de retorno

Devuelve el primer índice de la ASeries añadida en la NSeries.

### Observaciones

Si se establecen datos en celdas contiguas, use dos puntos para separarlas.Por ejemplo, $C$2:$C$5.Si se establecen datos en celdas no contiguas, use comas para separarlas.Por ejemplo: ($C$2,$D$5).Este método solo procesa *dataArea* como rango de datos. Si desea comprobar de forma inteligente el método ChartCollection.Add().

### Ejemplos

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
            
            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(30);

            // Crear gráfico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Agregar series usando parámetros de cadena y booleanos
            chart.NSeries.Add("=Sheet1!A1:B4", true);
            
            // Guarda el libro de trabajo
            workbook.Save("SeriesCollectionMethodAddWithStringBooleanDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, bool, bool) {#add_1}

Añade la colección [`Series`](../../series/) a un gráfico.

```csharp
public int Add(string area, bool isVertical, bool checkLabels)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| área | String | Especifica los valores a partir de los cuales trazar la serie de datos |
| isVertical | Booleano | Especifica si se debe trazar la serie a partir de un rango de valores de celdas por fila o por columna. |
| checkLabels | Booleano | Indica si el rango contiene el nombre de la serie |

### Valor de retorno

Devuelve el primer índice de la ASeries añadida en la NSeries.

### Observaciones

Si se establecen datos en celdas contiguas, use dos puntos para separarlas. Por ejemplo, $C$2:$C$5.Si se establecen datos en celdas no contiguas, use comas para separarlas. Por ejemplo, ($C$2,$D$5).

### Ejemplos

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
            
            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("Category1");
            sheet.Cells["A2"].PutValue(10);
            sheet.Cells["A3"].PutValue(20);
            sheet.Cells["B1"].PutValue("Category2");
            sheet.Cells["B2"].PutValue(30);
            sheet.Cells["B3"].PutValue(40);

            // Crear gráfico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Agregar series usando el método Add con parámetros de cadena y booleanos
            chart.NSeries.Add("=Sheet1!$B$2:$B$3", true, false);
            chart.NSeries.CategoryData = "=Sheet1!$A$1:$B$1";
            
            // Guarda el libro de trabajo
            wb.Save("SeriesCollectionMethodAddWithStringBooleanBooleanDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


