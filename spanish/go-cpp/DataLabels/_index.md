---
title: "Clase DataLabels"
linktitle: "DataLabels"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase DataLabels. Encapsula el objeto que representa datalabels en Go."
type: docs
weight: 200
url: /es/go-cpp/datalabels/
---

## DataLabels class

Encapsulates a collection of all the DataLabel objects for the specified Series.

```go

type DataLabels struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
| [NewDataLabels](./newdatalabels/) | Constructs from a parent object. |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [GetBorder](./getborder/) | Gets the Line</see>. |
| [GetArea](./getarea/) | Gets the Area</see>. |
| [IsAutoText](./isautotext/) | Indicates the text is auto generated. |
| [SetIsAutoText](./setisautotext/) | Indicates the text is auto generated. |
| [GetDirectionType](./getdirectiontype/) | Gets and sets the direction of text. |
| [SetDirectionType](./setdirectiontype/) | Gets and sets the direction of text. |
| [GetText](./gettext/) | Obtiene o establece el texto de la etiqueta de datos. |
| [SetText](./settext/) | Obtiene o establece el texto de la etiqueta de datos. |
| [IsTextWrapped](./istextwrapped/) | Gets or sets a value indicating whether the text is wrapped. |
| [SetIsTextWrapped](./setistextwrapped/) | Gets or sets a value indicating whether the text is wrapped. |
| [GetBackgroundMode](./getbackgroundmode/) | Gets and sets the display mode of the background |
| [SetBackgroundMode](./setbackgroundmode/) | Gets and sets the display mode of the background |
| [GetShowValue](./getshowvalue/) | Representa el comportamiento de visualización de los valores de la etiqueta de datos de un gráfico especificado. True muestra los valores. False para ocultarlos. |
| [SetShowValue](./setshowvalue/) | Representa el comportamiento de visualización de los valores de la etiqueta de datos de un gráfico especificado. True muestra los valores. False para ocultarlos. |
| [GetShowCellRange](./getshowcellrange/) | Indica si se muestra el rango de celdas como etiquetas de datos. |
| [SetShowCellRange](./setshowcellrange/) | Indica si se muestra el rango de celdas como etiquetas de datos. |
| [GetShowPercentage](./getshowpercentage/) | Representa el comportamiento de visualización del valor de porcentaje de la etiqueta de datos de un gráfico especificado. True muestra el valor de porcentaje. False para ocultarlo. |
| [SetShowPercentage](./setshowpercentage/) | Representa el comportamiento de visualización del valor de porcentaje de la etiqueta de datos de un gráfico especificado. True muestra el valor de porcentaje. False para ocultarlo. |
| [GetShowBubbleSize](./getshowbubblesize/) | Representa el comportamiento de visualización del valor de porcentaje de la etiqueta de datos de un gráfico especificado. True muestra el valor de porcentaje. False oculta el valor de porcentaje. |
| [SetShowBubbleSize](./setshowbubblesize/) | Representa el comportamiento de visualización del valor de porcentaje de la etiqueta de datos de un gráfico especificado. True muestra el valor de porcentaje. False oculta el valor de porcentaje. |
| [GetShowCategoryName](./getshowcategoryname/) | Representa el comportamiento de visualización del nombre de categoría de la etiqueta de datos de un gráfico especificado. True para mostrar el nombre de categoría en las etiquetas de datos de un gráfico. False para ocultarlo. |
| [SetShowCategoryName](./setshowcategoryname/) | Representa el comportamiento de visualización del nombre de categoría de la etiqueta de datos de un gráfico especificado. True para mostrar el nombre de categoría en las etiquetas de datos de un gráfico. False para ocultarlo. |
| [GetShowSeriesName](./getshowseriesname/) | Indica si el nombre de la serie se muestra en las etiquetas de datos de un gráfico. True para mostrar el nombre de la serie. False para ocultarlo. |
| [SetShowSeriesName](./setshowseriesname/) | Indica si el nombre de la serie se muestra en las etiquetas de datos de un gráfico. True para mostrar el nombre de la serie. False para ocultarlo. |
| [GetShowLegendKey](./getshowlegendkey/) | Representa el comportamiento de visualización de la clave de leyenda de la etiqueta de datos de un gráfico especificado. True si la clave de leyenda de la etiqueta de datos es visible. |
| [SetShowLegendKey](./setshowlegendkey/) | Representa el comportamiento de visualización de la clave de leyenda de la etiqueta de datos de un gráfico especificado. True si la clave de leyenda de la etiqueta de datos es visible. |
| [Get_NumberFormat](./get_numberformat/) | Representa la cadena de formato para el objeto DataLabels. |
| [SetNumberFormat](./setnumberformat/) | Representa la cadena de formato para el objeto DataLabels. |
| [GetNumber](./getnumber/) | Obtiene y establece el formato numérico incorporado. |
| [SetNumber](./setnumber/) | Obtiene y establece el formato numérico incorporado. |
| [GetNumberFormatLinked](./getnumberformatlinked/) | True if the number format is linked to the cells(so that the number format changes in the labels when it changes in the cells). |
| [SetNumberFormatLinked](./setnumberformatlinked/) | True if the number format is linked to the cells(so that the number format changes in the labels when it changes in the cells). |
| [ApplyFont](./applyfont/) | Aplica la fuente de las etiquetas de datos a todos los nodos hijos. |
| [GetFont](./getfont/) | Obtiene la fuente de DataLabels; |
| [GetSeparatorType](./getseparatortype/) | Obtiene o establece el tipo de separador utilizado para las etiquetas de datos en un gráfico. |
| [SetSeparatorType](./setseparatortype/) | Obtiene o establece el tipo de separador utilizado para las etiquetas de datos en un gráfico. |
| [GetSeparatorValue](./getseparatorvalue/) | Obtiene o establece el valor del separador utilizado para las etiquetas de datos en un gráfico. |
| [SetSeparatorValue](./setseparatorvalue/) | Obtiene o establece el valor del separador utilizado para las etiquetas de datos en un gráfico. |
| [GetPosition](./getposition/) | Representa la posición de la etiqueta de datos. |
| [SetPosition](./setposition/) | Representa la posición de la etiqueta de datos. |
| [IsNeverOverlap](./isneveroverlap/) | Indica si las etiquetas de datos nunca se superponen al generar una imagen de gráfico circular. Nota: esta propiedad solo tiene sentido cuando se genera una imagen de gráfico circular. |
| [SetIsNeverOverlap](./setisneveroverlap/) | Indica si las etiquetas de datos nunca se superponen al generar una imagen de gráfico circular. Nota: esta propiedad solo tiene sentido cuando se genera una imagen de gráfico circular. |
| [GetShapeType](./getshapetype/) | Obtiene o establece el tipo de forma de la etiqueta de datos. |
| [SetShapeType](./setshapetype/) | Obtiene o establece el tipo de forma de la etiqueta de datos. |
| [IsInnerMode](./isinnermode/) | Indicates whether the size of the plot area size includes the tick marks, and the axis labels.False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
| [SetIsInnerMode](./setisinnermode/) | Indicates whether the size of the plot area size includes the tick marks, and the axis labels.False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
| [GetShadow](./getshadow/) | True if the frame has a shadow. |
| [SetShadow](./setshadow/) | True if the frame has a shadow. |
| [GetShapeProperties](./getshapeproperties/) | Gets the ShapeProperties object. |
| [IsDefaultPosBeSet](./isdefaultposbeset/) | Indicates whether the default position (DefaultX, DefaultY, DefaultWidth and DefaultHeight) is set. |
| [GetDefaultXRatioToChart](./getdefaultxratiotochart/) | Represents x of default position in units of Fraction of the chart area. |
| [GetDefaultYRatioToChart](./getdefaultyratiotochart/) | Represents y of the default position in units of the fraction of the chart area. |
| [GetDefaultWidthRatioToChart](./getdefaultwidthratiotochart/) | Represents width of default position in units of Fraction of the chart area. |
| [GetDefaultHeightRatioToChart](./getdefaultheightratiotochart/) | Represents the height of the default position in units of the fraction of the chart area. |
| [GetTextOptions](./gettextoptions/) | Gets and sets the options of the text. |
| [GetAutoScaleFont](./getautoscalefont/) | True if the text in the object changes font size when the object size changes. The default value is True. |
| [SetAutoScaleFont](./setautoscalefont/) | True if the text in the object changes font size when the object size changes. The default value is True. |
| [IsAutomaticSize](./isautomaticsize/) | Indicates whether the chart frame is automatic sized. |
| [SetIsAutomaticSize](./setisautomaticsize/) | Indicates whether the chart frame is automatic sized. |
| [GetXRatioToChart](./getxratiotochart/) | Gets or sets the x coordinate of the upper left corner in units of ratio of the chart area. |
| [SetXRatioToChart](./setxratiotochart/) | Gets or sets the x coordinate of the upper left corner in units of ratio of the chart area. |
| [GetYRatioToChart](./getyratiotochart/) | Gets or sets the y coordinate of the upper left corner in units of the ratio of the chart area. |
| [SetYRatioToChart](./setyratiotochart/) | Gets or sets the y coordinate of the upper left corner in units of the ratio of the chart area. |
| [GetWidthRatioToChart](./getwidthratiotochart/) | Gets or sets the width of frame in units of ratio of the chart area. |
| [SetWidthRatioToChart](./setwidthratiotochart/) | Gets or sets the width of frame in units of ratio of the chart area. |
| [GetHeightRatioToChart](./getheightratiotochart/) | Gets or sets the height of the frame in units of the ratio of the chart area. |
| [SetHeightRatioToChart](./setheightratiotochart/) | Gets or sets the height of the frame in units of the ratio of the chart area. |
| [GetXPixel](./getxpixel/) | Gets or sets the x coordinate of the upper left corner in units of Pixel. |
| [SetXPixel](./setxpixel/) | Gets or sets the x coordinate of the upper left corner in units of Pixel. |
| [GetYPixel](./getypixel/) | Gets or sets the y coordinate of the upper left corner in units of pixels. |
| [SetYPixel](./setypixel/) | Gets or sets the y coordinate of the upper left corner in units of pixels. |
| [GetWidthPixel](./getwidthpixel/) | Gets or sets the width of frame in units of Pixel. |
| [SetWidthPixel](./setwidthpixel/) | Gets or sets the width of frame in units of Pixel. |
| [GetHeightPixel](./getheightpixel/) | Gets or sets the height of the frame in units of pixels. |
| [SetHeightPixel](./setheightpixel/) | Gets or sets the height of the frame in units of pixels. |
| [SetPositionAuto](./setpositionauto/) | Set position of the frame to automatic |
| [IsDeleted](./isdeleted/) | Indicates whether this data label is deleted. |
| [SetIsDeleted](./setisdeleted/) | Indicates whether this data label is deleted. |
| [GetTextHorizontalAlignment](./gettexthorizontalalignment/) | Gets and sets the text horizontal alignment. |
| [SetTextHorizontalAlignment](./settexthorizontalalignment/) | Gets and sets the text horizontal alignment. |
| [GetTextVerticalAlignment](./gettextverticalalignment/) | Gets or sets the text vertical alignment of text. |
| [SetTextVerticalAlignment](./settextverticalalignment/) | Gets or sets the text vertical alignment of text. |
| [GetRotationAngle](./getrotationangle/) | Represents the text rotation angle. |
| [SetRotationAngle](./setrotationangle/) | Represents the text rotation angle. |
| [IsAutomaticRotation](./isautomaticrotation/) | Indicates whether the text of the chart is automatically rotated. |
| [Characters](./characters/) | Returns a Characters object that represents a range of characters within the text. |
| [GetReadingOrder](./getreadingorder/) | Represents text reading order. |
| [SetReadingOrder](./setreadingorder/) | Represents text reading order. |
| [IsResizeShapeToFitText](./isresizeshapetofittext/) | Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting iswhen text within a shape is scaled in order to contain all the text inside. |
| [SetIsResizeShapeToFitText](./setisresizeshapetofittext/) | Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting iswhen text within a shape is scaled in order to contain all the text inside. |
| [GetLinkedSource](./getlinkedsource/) | Gets and sets a reference to the worksheet. |
| [SetLinkedSource](./setlinkedsource/) | Gets and sets a reference to the worksheet. |
