---
title: "Clase PivotFieldTop10AutoShowSettings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Pivot.PivotFieldTop10AutoShowSettings. Representa la configuración Top 10 AutoShow para un campo pivot"
type: docs
url: /es/net/aspose.cells.pivot/pivotfieldtop10autoshowsettings/
---
## PivotFieldTop10AutoShowSettings class

Representa la configuración AutoShow Top 10 para un campo de tabla dinámica.

```csharp
public class PivotFieldTop10AutoShowSettings
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AutoShowCount](../../aspose.cells.pivot/pivotfieldtop10autoshowsettings/autoshowcount/) { get; set; } | Representa el número de elementos superiores o inferiores que se muestran automáticamente en el campo PivotTable especificado. |
| [IsAutoShow](../../aspose.cells.pivot/pivotfieldtop10autoshowsettings/isautoshow/) { get; set; } | Indica si se aplica un filtro "Top 10 AutoShow" a este campo. |
| [IsTop](../../aspose.cells.pivot/pivotfieldtop10autoshowsettings/istop/) { get; set; } | Indica si el campo de tabla dinámica especificado se muestra automáticamente en orden ascendente. |
| [RankBy](../../aspose.cells.pivot/pivotfieldtop10autoshowsettings/rankby/) { get; set; } | Especifica el índice del campo de datos para la clasificación AutoShow. Representa el índice del campo auto mostrado. -1 significa el propio PivotField. Debe ser el índice de los campos de datos. |

### Observaciones

En xls: Implementar filtros de los 10 principales en Xls mediante Top 10 AutoShow. En archivos ooxml: el formato de archivo ooxml subyacente admite Top10 AutoShow, pero la interfaz de usuario de Excel 2007 y posteriores solo brinda acceso mediante el filtro Top10. Si no se requiere compatibilidad con XLS, se recomienda usar el filtro Top10 en su lugar.

### Ejemplos

```csharp

[C#]

Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
cells[0, 0].Value = "fruit";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "blueberry";
cells[3, 0].Value = "kiwi";
cells[4, 0].Value = "cherry";
cells[5, 0].Value = "grape";
cells[6, 0].Value = "blueberry";
cells[7, 0].Value = "kiwi";
cells[8, 0].Value = "cherry";

cells[0, 1].Value = "year";
cells[1, 1].Value = 2020;
cells[2, 1].Value = 2020;
cells[3, 1].Value = 2020;
cells[4, 1].Value = 2020;
cells[5, 1].Value = 2021;
cells[6, 1].Value = 2021;
cells[7, 1].Value = 2021;
cells[8, 1].Value = 2021;

cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;
cells[5, 2].Value = 90;
cells[6, 2].Value = 100;
cells[7, 2].Value = 110;
cells[8, 2].Value = 120;

PivotTableCollection pivots = sheet.PivotTables;

PivotTable pivot = pivots.Add("=Sheet1!A1:C9", "A12");

pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");
           
pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
           
 //Cambiar los atributos del PivotField
PivotField rowField = pivot.RowFields[0];
rowField.DisplayName = "custom display name";

//Mostrar los 2 elementos principales por etiqueta de campo de fila.
rowField.Top10AutoShow(true, true, 2, -1);

PivotFieldTop10AutoShowSettings sortSetting = rowField.Top10AutoShowSettings;
Console.WriteLine(sortSetting.IsAutoShow);

 pivot.CalculateData();

book.Save("out.xlsx");

[Visual Basic]

Dim book As New Workbook()
Dim sheet As Worksheet = book.Worksheets(0)
Dim cells As Cells = sheet.Cells
cells(0, 0).Value = "fruit"
cells(1, 0).Value = "grape"
cells(2, 0).Value = "blueberry"
cells(3, 0).Value = "kiwi"
cells(4, 0).Value = "cherry"
cells(5, 0).Value = "grape"
cells(6, 0).Value = "blueberry"
cells(7, 0).Value = "kiwi"
cells(8, 0).Value = "cherry"

cells(0, 1).Value = "year"
cells(1, 1).Value = 2020
cells(2, 1).Value = 2020
cells(3, 1).Value = 2020
cells(4, 1).Value = 2020
cells(5, 1).Value = 2021
cells(6, 1).Value = 2021
cells(7, 1).Value = 2021
cells(8, 1).Value = 2021

cells(0, 2).Value = "amount"
cells(1, 2).Value = 50
cells(2, 2).Value = 60
cells(3, 2).Value = 70
cells(4, 2).Value = 80
cells(5, 2).Value = 90
cells(6, 2).Value = 100
cells(7, 2).Value = 110
cells(8, 2).Value = 120

Dim pivots As PivotTableCollection = sheet.PivotTables

Dim pivot As PivotTable = pivots.Add("=Sheet1!A1:C9", "A12")
 
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
pivot.AddFieldToArea(PivotFieldType.Column, "year")
pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10

'Change PivotField's attributes
Dim rowField As PivotField = pivot.RowFields(0)
rowField.DisplayName = "custom display name"

'Show top 2 items by row field label.
rowField.Top10AutoShow(True, True, 2, -1)

Dim sortSetting As PivotFieldTop10AutoShowSettings = rowField.Top10AutoShowSettings
Console.WriteLine(sortSetting.IsAutoShow)

pivot.CalculateData()

book.Save("out.xlsx")
```

### Ver también

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


