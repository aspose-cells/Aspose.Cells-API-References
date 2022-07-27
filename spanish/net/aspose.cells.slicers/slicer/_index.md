---
title: Slicer
second_title: Referencia de API de Aspose.Cells para .NET
description: descripción resumida de Slicer View
type: docs
weight: 5630
url: /es/net/aspose.cells.slicers/slicer/
---
## Slicer class

descripción resumida de Slicer View

```csharp
public class Slicer
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AlternativeText](../../aspose.cells.slicers/slicer/alternativetext) { get; set; } | Devuelve o establece la cadena de texto descriptiva (alternativa) del objeto Slicer. |
| [Caption](../../aspose.cells.slicers/slicer/caption) { get; set; } | Devuelve o establece el título de la segmentación de datos especificada. |
| [CaptionVisible](../../aspose.cells.slicers/slicer/captionvisible) { get; set; } | Devuelve o establece si el encabezado que muestra el subtítulo de la segmentación es visible el valor predeterminado es true |
| [ColumnWidth](../../aspose.cells.slicers/slicer/columnwidth) { get; set; } | Devuelve o establece el ancho, en puntos, de cada columna en la segmentación. |
| [ColumnWidthPixel](../../aspose.cells.slicers/slicer/columnwidthpixel) { get; set; } | Obtiene o establece el ancho en unidades de píxeles para cada columna de la segmentación. |
| [Height](../../aspose.cells.slicers/slicer/height) { get; set; } | Devuelve o establece la altura de la segmentación especificada, en puntos. |
| [HeightPixel](../../aspose.cells.slicers/slicer/heightpixel) { get; set; } | Devuelve o establece la altura de la segmentación especificada, en píxeles. |
| [IsLocked](../../aspose.cells.slicers/slicer/islocked) { get; set; } | Indica si la forma de corte está bloqueada. |
| [IsPrintable](../../aspose.cells.slicers/slicer/isprintable) { get; set; } | Indica si el objeto de segmentación es imprimible. |
| [LeftPixel](../../aspose.cells.slicers/slicer/leftpixel) { get; set; } | Devuelve o establece el desplazamiento horizontal de la forma de la segmentación desde su columna izquierda, en píxeles. |
| [LockedAspectRatio](../../aspose.cells.slicers/slicer/lockedaspectratio) { get; set; } | Indica si se bloquea la relación de aspecto. |
| [LockedPosition](../../aspose.cells.slicers/slicer/lockedposition) { get; set; } | Indica si la segmentación de datos especificada se puede mover o cambiar de tamaño mediante la interfaz de usuario. |
| [Name](../../aspose.cells.slicers/slicer/name) { get; set; } | Devuelve o establece el nombre de la segmentación especificada |
| [NumberOfColumns](../../aspose.cells.slicers/slicer/numberofcolumns) { get; set; } | Devuelve o establece el número de columnas en la segmentación de datos especificada. |
| [Parent](../../aspose.cells.slicers/slicer/parent) { get; } | Devuelve el objeto Worksheet que representa la hoja que contiene la segmentación. Solo lectura. |
| [Placement](../../aspose.cells.slicers/slicer/placement) { get; set; } | Representa la forma en que el objeto de dibujo se adjunta a las celdas debajo de él. La propiedad controla la ubicación de un objeto en una hoja de trabajo. |
| [RowHeight](../../aspose.cells.slicers/slicer/rowheight) { get; set; } | Devuelve o establece la altura, en puntos, de cada fila en la segmentación especificada. |
| [RowHeightPixel](../../aspose.cells.slicers/slicer/rowheightpixel) { get; set; } | Devuelve o establece la altura, en píxeles, de cada fila en la segmentación especificada. |
| [SlicerCache](../../aspose.cells.slicers/slicer/slicercache) { get; } | Devuelve el objeto SlicerCache asociado con la segmentación. Solo lectura. |
| [StyleType](../../aspose.cells.slicers/slicer/styletype) { get; set; } | Especifique el tipo de estilo de segmentación incorporado el tipo predeterminado es SlicerStyleLight1 |
| [Title](../../aspose.cells.slicers/slicer/title) { get; set; } | Especifica el título del objeto Slicer actual. |
| [TopPixel](../../aspose.cells.slicers/slicer/toppixel) { get; set; } | Devuelve o establece el desplazamiento vertical de la forma de la segmentación desde su fila superior, en píxeles. |
| [Width](../../aspose.cells.slicers/slicer/width) { get; set; } | Devuelve o establece el ancho de la segmentación especificada, en puntos. |
| [WidthPixel](../../aspose.cells.slicers/slicer/widthpixel) { get; set; } | Devuelve o establece el ancho de la segmentación especificada, en píxeles. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddPivotConnection](../../aspose.cells.slicers/slicer/addpivotconnection)(PivotTable) | Agrega conexión de tabla dinámica. |
| [Refresh](../../aspose.cells.slicers/slicer/refresh)() | Actualizar la segmentación. Mientras tanto, Actualizar y calcular tablas dinámicas relativas. |
| [RemovePivotConnection](../../aspose.cells.slicers/slicer/removepivotconnection)(PivotTable) | Elimina la conexión de tabla dinámica. |

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

int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
pivot.RefreshData();
pivot.CalculateData();

SlicerCollection slicers = sheet.Slicers;
int slicerIndex = slicers.Add(pivot, "E12", "fruit");
Slicer slicer = slicers[slicerIndex];
slicer.StyleType = SlicerStyleType.SlicerStyleLight2;

SlicerCacheItemCollection items = slicer.SlicerCache.SlicerCacheItems;
SlicerCacheItem item = items[0];
item.Selected = false;
//haz tu negocio
book.Save("out.xlsx");

[Visual Basic]

Dim book As Workbook = New Workbook()
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
Dim pivotIndex As Int32 = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable")
Dim pivot As PivotTable = pivots(pivotIndex)
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
Pivot.AddFieldToArea(PivotFieldType.Column, "year")
Pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10
pivot.RefreshData()
pivot.CalculateData()

Dim slicers As SlicerCollection = sheet.Slicers
Dim slicerIndex As Int32 = slicers.Add(pivot, "E12", "fruit")
Dim slicer As Slicer = slicers(slicerIndex)
slicer.StyleType = SlicerStyleType.SlicerStyleLight2

Dim items As SlicerCacheItemCollection = slicer.SlicerCache.SlicerCacheItems
Dim item As SlicerCacheItem = items(0)
item.Selected = False

book.Save("out_vb.xlsx")
```

### Ver también

* espacio de nombres [Aspose.Cells.Slicers](../../aspose.cells.slicers)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
