---
title: "WorksheetCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WorksheetCollection. Añade una hoja de cálculo a la colección"
type: docs
url: /es/net/aspose.cells/worksheetcollection/add/
---
## Add(SheetType) {#add_2}

Agrega una hoja de cálculo a la colección.

```csharp
public int Add(SheetType type)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | SheetType | Tipo Worksheet. |

### Valor de retorno

[`Worksheet`](../../worksheet/) object index.

### Ejemplos

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
            
            // Agregar una nueva hoja de gráfico usando el parámetro SheetType
            workbook.Worksheets.Add(SheetType.Chart);
            
            // Agregar datos a la primera hoja de cálculo
            Cells cells = workbook.Worksheets[0].Cells;
            cells["C2"].PutValue(5000);
            cells["C3"].PutValue(3000);
            cells["C4"].PutValue(4000);
            cells["C5"].PutValue(5000);
            cells["C6"].PutValue(6000);
            
            // Crear gráfico en la hoja de gráfico
            Aspose.Cells.Charts.ChartCollection charts = workbook.Worksheets[1].Charts;
            int chartIndex = charts.Add(Aspose.Cells.Charts.ChartType.Column, 10, 10, 20, 20);
            Aspose.Cells.Charts.Chart chart = charts[chartIndex];
            chart.NSeries.Add("Sheet1!C2:C6", true);
            
            // Guardar el libro de trabajo (opcional)
            // workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* enum [SheetType](../../sheettype/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add() {#add_1}

Agrega una hoja de cálculo a la colección.

```csharp
public int Add()
```

### Valor de retorno

[`Worksheet`](../../worksheet/) object index.

### Ver también

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add}

Agrega una hoja de cálculo a la colección.

```csharp
public Worksheet Add(string sheetName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetName | String | Nombre de la hoja de cálculo |

### Valor de retorno

[`Worksheet`](../../worksheet/) object.

### Ejemplos

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
            
            // Agregar datos a la nueva hoja de cálculo
            worksheet.Cells["A1"].PutValue("Worksheet added successfully!");
            
            // Guarda el libro de trabajo
            wb.Save("WorksheetCollectionMethodAddWithStringDemo_output.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


