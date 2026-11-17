---
title: "Clase Series"
linktitle: "Series"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase Series. Encapsula el objeto que representa series en Go."
type: docs
weight: 200
url: /es/go-cpp/series/
---

## Series class

Encapsulates the object that represents a single data series in a chart.

```go

type Series struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [IsFiltered](./isfiltered/) | Indica si la serie está seleccionada o filtrada. True indica que esta serie está filtrada y no se mostrará en el gráfico. |
| [SetIsFiltered](./setisfiltered/) | Indica si la serie está seleccionada o filtrada. True indica que esta serie está filtrada y no se mostrará en el gráfico. |
| [GetLayoutProperties](./getlayoutproperties/) | Representa las propiedades del diseño. |
| [Move](./move/) | Mueve la serie hacia arriba o abajo. |
| [GetPoints](./getpoints/) | Obtiene la colección de puntos en una serie en un gráfico. |
| [GetArea](./getarea/) | Representa el área de fondo del objeto Series. |
| [GetBorder](./getborder/) | Representa el borde de un objeto Series. |
| [GetName](./getname/) | Obtiene o establece el nombre de la serie de datos. |
| [SetName](./setname/) | Obtiene o establece el nombre de la serie de datos. |
| [GetDisplayName](./getdisplayname/) | Obtiene el nombre de la serie que se muestra en el gráfico. |
| [GetCountOfDataValues](./getcountofdatavalues/) | Obtiene el número de los valores de datos. |
| [IsVerticalValues](./isverticalvalues/) | Indica si la fuente de datos es vertical. |
| [GetValues](./getvalues/) | Representa los valores Y de esta serie de gráfico. |
| [SetValues](./setvalues/) | Representa los valores Y de esta serie de gráfico. |
| [GetPointValues](./getpointvalues/) | Obtiene los valores reales que se utilizan para trazar cada pointof de esta serie en el gráfico. |
| [GetCategoryValues](./getcategoryvalues/) | Obtiene los valores reales de categoría que se utilizan para trazar cada pointof de esta serie en el gráfico. |
| [GetValuesFormatCode](./getvaluesformatcode/) | Representa el código de formato de la Values NumberList. |
| [SetValuesFormatCode](./setvaluesformatcode/) | Representa el código de formato de la Values NumberList. |
| [GetXValuesFormatCode](./getxvaluesformatcode/) | Representa el código de formato de la X Values' NumberList. |
| [SetXValuesFormatCode](./setxvaluesformatcode/) | Representa el código de formato de la X Values' NumberList. |
| [GetXValues](./getxvalues/) | Representa los valores X de esta serie de gráfico. |
| [SetXValues](./setxvalues/) | Representa los valores X de esta serie de gráfico. |
| [GetBubbleSizes](./getbubblesizes/) | Obtiene o establece los valores de tamaño de burbuja de la serie de gráfico. |
| [SetBubbleSizes](./setbubblesizes/) | Obtiene o establece los valores de tamaño de burbuja de la serie de gráfico. |
| [GetTrendLines](./gettrendlines/) | Devuelve todas las líneas de tendencia de esta serie. |
| [GetSmooth](./getsmooth/) | Representa el suavizado de curvas.Verdadero si el suavizado de curvas está activado para el gráfico de líneas o de dispersión.Se aplica solo a gráficos de líneas y gráficos de dispersión con líneas. |
| [SetSmooth](./setsmooth/) | Representa el suavizado de curvas.Verdadero si el suavizado de curvas está activado para el gráfico de líneas o de dispersión.Se aplica solo a gráficos de líneas y gráficos de dispersión con líneas. |
| [GetShadow](./getshadow/) | Verdadero si la serie tiene una sombra. |
| [SetShadow](./setshadow/) | Verdadero si la serie tiene una sombra. |
| [GetHas3DEffect](./gethas3deffect/) | Verdadero si la serie tiene una apariencia tridimensional. |
| [SetHas3DEffect](./sethas3deffect/) | Verdadero si la serie tiene una apariencia tridimensional. |
| [GetBar3DShapeType](./getbar3dshapetype/) | Obtiene o establece el tipo de forma 3D utilizado con el gráfico de barras o columnas 3-D. |
| [SetBar3DShapeType](./setbar3dshapetype/) | Obtiene o establece el tipo de forma 3D utilizado con el gráfico de barras o columnas 3-D. |
| [GetDataLabels](./getdatalabels/) | Representa el objeto DataLabels para el ASeries especificado. |
| [GetType](./gettype/) | Obtiene o establece el tipo de una serie de datos. |
| [SetType](./settype/) | Obtiene o establece el tipo de una serie de datos. |
| [GetMarker](./getmarker/) | Obtiene el Marker</see>. |
| [GetPlotOnSecondAxis](./getplotonsecondaxis/) | Indica si esta serie se traza en el segundo eje de valores. |
| [SetPlotOnSecondAxis](./setplotonsecondaxis/) | Indica si esta serie se traza en el segundo eje de valores. |
| [GetXErrorBar](./getxerrorbar/) | Representa la barra de error de dirección X de la serie. |
| [GetYErrorBar](./getyerrorbar/) | Representa la barra de error de dirección Y de la serie. |
| [GetHasHiLoLines](./gethashilolines/) | Verdadero si el gráfico de líneas tiene líneas alto-bajo.Se aplica solo a gráficos de líneas. |
| [SetHasHiLoLines](./sethashilolines/) | Verdadero si el gráfico de líneas tiene líneas alto-bajo.Se aplica solo a gráficos de líneas. |
| [GetHiLoLines](./gethilolines/) | Devuelve un objeto HiLoLines que representa las líneas alto-bajo para una serie en un gráfico de líneas.Se aplica solo a gráficos de líneas. |
| [GetHasSeriesLines](./gethasserieslines/) | Verdadero si un gráfico de columnas apiladas o de barras tiene líneas de serie o si un gráfico de pastel dentro de pastel o de barra dentro de pastel tiene líneas de conexión entre las dos secciones. Se aplica solo a gráficos de columnas apiladas, gráficos de barras, gráficos de pastel dentro de pastel o de barra dentro de pastel. |
| [SetHasSeriesLines](./sethasserieslines/) | Verdadero si un gráfico de columnas apiladas o de barras tiene líneas de serie o si un gráfico de pastel dentro de pastel o de barra dentro de pastel tiene líneas de conexión entre las dos secciones. Se aplica solo a gráficos de columnas apiladas, gráficos de barras, gráficos de pastel dentro de pastel o de barra dentro de pastel. |
| [GetSeriesLines](./getserieslines/) | Devuelve un objeto SeriesLines que representa las líneas de serie para un gráfico de barras apiladas o un gráfico de columnas apiladas. Se aplica solo a gráficos de barras apiladas y de columnas apiladas. |
| [GetHasDropLines](./gethasdroplines/) | Verdadero si el gráfico tiene líneas de caída. Se aplica solo a gráficos de líneas o de áreas. |
| [SetHasDropLines](./sethasdroplines/) | Verdadero si el gráfico tiene líneas de caída. Se aplica solo a gráficos de líneas o de áreas. |
| [GetDropLines](./getdroplines/) | Devuelve un objeto Line que representa las líneas de caída para una serie en el gráfico de líneas o de áreas. Se aplica solo a gráficos de líneas o de áreas. |
| [GetHasUpDownBars](./gethasupdownbars/) | Verdadero si un gráfico de líneas tiene barras ascendentes y descendentes. Se aplica solo a gráficos de líneas. |
| [SetHasUpDownBars](./sethasupdownbars/) | Verdadero si un gráfico de líneas tiene barras ascendentes y descendentes. Se aplica solo a gráficos de líneas. |
| [GetUpBars](./getupbars/) | Devuelve un objeto DropBars que representa las barras ascendentes en un gráfico de líneas. Se aplica solo a gráficos de líneas. |
| [GetDownBars](./getdownbars/) | Devuelve un objeto DropBars que representa las barras descendentes en un gráfico de líneas. Se aplica solo a gráficos de líneas. |
| [IsColorVaried](./iscolorvaried/) | Representa si el color de los puntos varía. El gráfico debe contener solo una serie o ser un gráfico de pastel. |
| [SetIsColorVaried](./setiscolorvaried/) | Representa si el color de los puntos varía. El gráfico debe contener solo una serie o ser un gráfico de pastel. |
| [GetGapWidth](./getgapwidth/) | Returns or sets the space between bar or column clusters, as a percentage of the bar or column width.The value of this property must be between 0 and 500. |
| [SetGapWidth](./setgapwidth/) | Returns or sets the space between bar or column clusters, as a percentage of the bar or column width.The value of this property must be between 0 and 500. |
| [GetFirstSliceAngle](./getfirstsliceangle/) | Obtiene o establece el ángulo de la primera porción de gráfico de pastel o de rosquilla, en grados (en sentido horario desde la vertical). Se aplica solo a gráficos de pastel, pastel 3D y rosquilla, con valores de 0 a 360. |
| [SetFirstSliceAngle](./setfirstsliceangle/) | Obtiene o establece el ángulo de la primera porción de gráfico de pastel o de rosquilla, en grados (en sentido horario desde la vertical). Se aplica solo a gráficos de pastel, pastel 3D y rosquilla, con valores de 0 a 360. |
| [GetOverlap](./getoverlap/) | Especifica cómo se posicionan las barras y columnas. Puede ser un valor entre -100 y 100. Se aplica solo a gráficos de barras 2D y columnas 2D. |
| [SetOverlap](./setoverlap/) | Especifica cómo se posicionan las barras y columnas. Puede ser un valor entre -100 y 100. Se aplica solo a gráficos de barras 2D y columnas 2D. |
| [GetSecondPlotSize](./getsecondplotsize/) | Devuelve o establece el tamaño de la sección secundaria de un gráfico de pastel dentro de pastel o de barra dentro de pastel, como porcentaje del tamaño del pastel principal. Puede ser un valor de 5 a 200. |
| [SetSecondPlotSize](./setsecondplotsize/) | Devuelve o establece el tamaño de la sección secundaria de un gráfico de pastel dentro de pastel o de barra dentro de pastel, como porcentaje del tamaño del pastel principal. Puede ser un valor de 5 a 200. |
| [GetSplitType](./getsplittype/) | Devuelve o establece un valor que determina cómo se eligen los puntos de datos que están en el segundo pastel o barra en un gráfico de pastel dentro de pastel o de barra dentro de pastel. |
| [SetSplitType](./setsplittype/) | Devuelve o establece un valor que determina cómo se eligen los puntos de datos que están en el segundo pastel o barra en un gráfico de pastel dentro de pastel o de barra dentro de pastel. |
| [GetSplitValue](./getsplitvalue/) | Devuelve o establece un valor que se utilizará para determinar qué puntos de datos están en el segundo pastel o barra en un gráfico de pastel dentro de pastel o de barra dentro de pastel. |
| [SetSplitValue](./setsplitvalue/) | Devuelve o establece un valor que se utilizará para determinar qué puntos de datos están en el segundo pastel o barra en un gráfico de pastel dentro de pastel o de barra dentro de pastel. |
| [IsAutoSplit](./isautosplit/) | Indica si el valor del umbral es automático. |
| [GetBubbleScale](./getbubblescale/) | Obtiene o establece el factor de escala para las burbujas en el grupo de gráficos especificado. Puede ser un valor entero de 0 (cero) a 300, correspondiente a un porcentaje del tamaño predeterminado. Se aplica solo a gráficos de burbujas. |
| [SetBubbleScale](./setbubblescale/) | Obtiene o establece el factor de escala para las burbujas en el grupo de gráficos especificado. Puede ser un valor entero de 0 (cero) a 300, correspondiente a un porcentaje del tamaño predeterminado. Se aplica solo a gráficos de burbujas. |
| [GetSizeRepresents](./getsizerepresents/) | Obtiene o establece lo que representa el tamaño de la burbuja en un gráfico de burbujas. |
| [SetSizeRepresents](./setsizerepresents/) | Obtiene o establece lo que representa el tamaño de la burbuja en un gráfico de burbujas. |
| [GetShowNegativeBubbles](./getshownegativebubbles/) | Verdadero si se muestran burbujas negativas para el grupo de gráficos. Válido solo para gráficos de burbujas. |
| [SetShowNegativeBubbles](./setshownegativebubbles/) | Verdadero si se muestran burbujas negativas para el grupo de gráficos. Válido solo para gráficos de burbujas. |
| [GetDoughnutHoleSize](./getdoughnutholesize/) | Devuelve o establece el tamaño del agujero en un grupo de gráficos de rosquilla. El tamaño del agujero se expresa como un porcentaje del tamaño del gráfico, entre el 10 y el 90 por ciento. |
| [SetDoughnutHoleSize](./setdoughnutholesize/) | Devuelve o establece el tamaño del agujero en un grupo de gráficos de rosquilla. El tamaño del agujero se expresa como un porcentaje del tamaño del gráfico, entre el 10 y el 90 por ciento. |
| [GetExplosion](./getexplosion/) | La distancia de una porción de pastel abierta desde el centro del gráfico de pastel se expresa como un porcentaje del diámetro del pastel. |
| [SetExplosion](./setexplosion/) | La distancia de una porción de pastel abierta desde el centro del gráfico de pastel se expresa como un porcentaje del diámetro del pastel. |
| [GetHasRadarAxisLabels](./gethasradaraxislabels/) | Verdadero si un gráfico de radar tiene etiquetas en el eje de categorías. Se aplica solo a gráficos de radar. |
| [SetHasRadarAxisLabels](./sethasradaraxislabels/) | Verdadero si un gráfico de radar tiene etiquetas en el eje de categorías. Se aplica solo a gráficos de radar. |
| [GetHasLeaderLines](./gethasleaderlines/) | Verdadero si la serie tiene líneas guía. |
| [SetHasLeaderLines](./sethasleaderlines/) | Verdadero si la serie tiene líneas guía. |
| [GetLeaderLines](./getleaderlines/) | Representa líneas guía en un gráfico. Las líneas guía conectan las etiquetas de datos con los puntos de datos. Este objeto no es una colección; no hay un objeto que represente una sola línea guía. |
| [GetLegendEntry](./getlegendentry/) | Obtiene la entrada de leyenda correspondiente a esta serie. |
| [GetShapeProperties](./getshapeproperties/) | Obtiene el objeto ShapePropertyCollection que contiene las propiedades visuales de forma de la Serie. |
