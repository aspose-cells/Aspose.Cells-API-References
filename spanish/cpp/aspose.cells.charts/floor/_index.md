---
title: Aspose::Cells::Charts::Floor class
linktitle: Floor
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::Floor class. Encapsulates the object that represents the floor of a 3-D chart in C++.'
type: docs
weight: 1700
url: /es/cpp/aspose.cells.charts/floor/
---
## Floor class


Encapsulates the object that represents the floor of a 3-D chart.

```cpp
class Floor : public Aspose::Cells::Drawing::Area
```

## Methods

| Method | Description |
| --- | --- |
| [Area(Area_Impl* impl)](../../aspose.cells.drawing/area/area/) | Constructs from an implementation object. |
| [Area(const Area\& src)](../../aspose.cells.drawing/area/area/) | Copy constructor. |
| [Floor(Floor_Impl* impl)](./floor/) | Constructs from an implementation object. |
| [Floor(const Floor\& src)](./floor/) | Copy constructor. |
| [Floor(const Area\& src)](./floor/) | Constructs from a parent object. |
| [GetBackgroundColor()](../../aspose.cells.drawing/area/getbackgroundcolor/) | Gets or sets the background [Color](../../aspose.cells/color/) of the [Area](../../aspose.cells.drawing/area/). |
| [GetBorder()](./getborder/) | Gets or sets the border Line. |
| [GetFillFormat()](../../aspose.cells.drawing/area/getfillformat/) | Represents a [FillFormat](../../aspose.cells.drawing/fillformat/) object that contains fill formatting properties for the specified chart or shape. |
| [GetForegroundColor()](../../aspose.cells.drawing/area/getforegroundcolor/) | Gets or sets the foreground [Color](../../aspose.cells/color/). |
| [GetFormatting()](../../aspose.cells.drawing/area/getformatting/) | Represents the formatting of the area. |
| [GetInvertIfNegative()](../../aspose.cells.drawing/area/getinvertifnegative/) | If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [GetTransparency()](../../aspose.cells.drawing/area/gettransparency/) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Floor\& src)](./operator_asm/) | operator= |
| [operator=(const Area\& src)](../../aspose.cells.drawing/area/operator_asm/) | operator= |
| [SetBackgroundColor(const Aspose::Cells::Color\& value)](../../aspose.cells.drawing/area/setbackgroundcolor/) | Gets or sets the background [Color](../../aspose.cells/color/) of the [Area](../../aspose.cells.drawing/area/). |
| [SetBorder(const Line\& value)](./setborder/) | Gets or sets the border Line. |
| [SetForegroundColor(const Aspose::Cells::Color\& value)](../../aspose.cells.drawing/area/setforegroundcolor/) | Gets or sets the foreground [Color](../../aspose.cells/color/). |
| [SetFormatting(FormattingType value)](../../aspose.cells.drawing/area/setformatting/) | Represents the formatting of the area. |
| [SetInvertIfNegative(bool value)](../../aspose.cells.drawing/area/setinvertifnegative/) | If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [SetTransparency(double value)](../../aspose.cells.drawing/area/settransparency/) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [~Area()](../../aspose.cells.drawing/area/~area/) | Destructor. |
| [~Floor()](./~floor/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
//Instanciar la clase License
License license;

//Pasar solo el nombre del archivo de licencia incrustado en el ensamblado
license.SetLicense(u"Aspose.Cells.lic");

//Instanciar el objeto workbook
Workbook workbook;

//Obtener la colección de celdas
Cells cells = workbook.GetWorksheets().Get(0).GetCells();

//Colocar valores en celdas
cells.Get(u"A1").PutValue(1);

cells.Get(u"A2").PutValue(2);

cells.Get(u"A3").PutValue(3);

//obtener colección de gráficos
ChartCollection charts = workbook.GetWorksheets().Get(0).GetCharts();

//agregar un nuevo gráfico
int index = charts.Add(ChartType::Column3DStacked, 5, 0, 15, 5);

//obtener el gráfico recién añadido
Chart chart = charts.Get(index);

//establecer nseries de gráficos
chart.GetNSeries().Add(u"A1:A3", true);

//Mostrar etiquetas de datos
chart.GetNSeries().Get(0).GetDataLabels().SetShowValue(true);

//Obtener el piso del gráfico
Floor floor = chart.GetFloor();

//establecer el borde del piso como rojo
floor.GetBorder().SetColor(Color{ 0xff, 0xff, 0, 0 });

//establecer formato de relleno
floor.GetFillFormat().SetPresetColorGradient(GradientPresetType::CalmWater, GradientStyleType::DiagonalDown, 2);

//guardar el archivo
workbook.Save(u"dest.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Class [Area](../../aspose.cells.drawing/area/)
* Namespace [Aspose::Cells::Charts](../)
* Library [Aspose.Cells for C++](../../)
