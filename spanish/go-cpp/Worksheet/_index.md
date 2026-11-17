---
title: "Clase Worksheet"
linktitle: "Worksheet"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase Worksheet. Encapsula el objeto que representa una hoja de cálculo en Go."
type: docs
weight: 200
url: /es/go-cpp/worksheet/
---

## Worksheet class

Encapsulates the object that represents a single worksheet.

```go

type Worksheet struct  {
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
| [Dispose](./dispose/) | Performs application-defined tasks associated with freeing, releasing, orresetting unmanaged resources. |
| [GetProtection](./getprotection/) | Representa los distintos tipos de opciones de protección disponibles para una hoja de cálculo. Soporta opciones de protección avanzadas en ExcelXP y versiones posteriores. |
| [GetUniqueId](./getuniqueid/) | Obtiene y establece el id único, es el mismo que {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [SetUniqueId](./setuniqueid/) | Obtiene y establece el id único, es el mismo que {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [GetPanes](./getpanes/) | Obtiene los paneles de la ventana. |
| [GetWorkbook](./getworkbook/) | Obtiene el objeto libro de trabajo que contiene esta hoja. |
| [GetCells](./getcells/) | Obtiene la colección Aspose.Cells.Cells. |
| [GetQueryTables](./getquerytables/) | Obtiene QueryTableCollection en la hoja de cálculo. |
| [GetType](./gettype/) | Representa el tipo de hoja de cálculo. |
| [SetType](./settype/) | Representa el tipo de hoja de cálculo. |
| [GetName](./getname/) | Obtiene o establece el nombre de la hoja de cálculo. |
| [SetName](./setname/) | Obtiene o establece el nombre de la hoja de cálculo. |
| [GetShowFormulas](./getshowformulas/) | Indica si se deben mostrar las fórmulas o sus resultados. |
| [SetShowFormulas](./setshowformulas/) | Indica si se deben mostrar las fórmulas o sus resultados. |
| [GetShowDataTypeIcons](./getshowdatatypeicons/) | Indica si se deben mostrar los íconos de tipo de datos. |
| [SetShowDataTypeIcons](./setshowdatatypeicons/) | Indica si se deben mostrar los íconos de tipo de datos. |
| [IsGridlinesVisible](./isgridlinesvisible/) | Obtiene o establece un valor que indica si las líneas de cuadrícula son visibles. El valor predeterminado es verdadero. |
| [SetIsGridlinesVisible](./setisgridlinesvisible/) | Obtiene o establece un valor que indica si las líneas de cuadrícula son visibles. El valor predeterminado es verdadero. |
| [IsRowColumnHeadersVisible](./isrowcolumnheadersvisible/) | Obtiene o establece un valor que indica si la hoja de cálculo mostrará encabezados de filas y columnas. El valor predeterminado es verdadero. |
| [SetIsRowColumnHeadersVisible](./setisrowcolumnheadersvisible/) | Obtiene o establece un valor que indica si la hoja de cálculo mostrará encabezados de filas y columnas. El valor predeterminado es verdadero. |
| [GetPaneState](./getpanestate/) | Indica si el panel tiene divisiones horizontales o verticales, y si esas divisiones están congeladas. |
| [GetDisplayZeros](./getdisplayzeros/) | Verdadero si se muestran valores cero. |
| [SetDisplayZeros](./setdisplayzeros/) | Verdadero si se muestran valores cero. |
| [GetDisplayRightToLeft](./getdisplayrighttoleft/) | Indica si la hoja de cálculo especificada se muestra de derecha a izquierda en lugar de izquierda a derecha. El valor predeterminado es falso. |
| [SetDisplayRightToLeft](./setdisplayrighttoleft/) | Indica si la hoja de cálculo especificada se muestra de derecha a izquierda en lugar de izquierda a derecha. El valor predeterminado es falso. |
| [IsOutlineShown](./isoutlineshown/) | Indica si se muestra el contorno. |
| [SetIsOutlineShown](./setisoutlineshown/) | Indica si se muestra el contorno. |
| [IsSelected](./isselected/) | Indica si esta hoja de cálculo está seleccionada cuando se abre el libro de trabajo. |
| [SetIsSelected](./setisselected/) | Indica si esta hoja de cálculo está seleccionada cuando se abre el libro de trabajo. |
| [FreezePanes_Int_Int_Int_Int](./freezepanes_int_int_int_int/) | Congela los paneles en la celda especificada de la hoja de cálculo. |
| [GetFreezedPanes](./getfreezedpanes/) | Obtiene los paneles congelados. |
| [Split](./split/) | Divide la ventana. |
| [FreezePanes_String_Int_Int](./freezepanes_string_int_int/) | Congela los paneles en la celda especificada de la hoja de cálculo. |
| [UnFreezePanes](./unfreezepanes/) | Descongela los paneles en la hoja de cálculo. |
| [RemoveSplit](./removesplit/) | Elimina la división de la ventana. |
| [GetPivotTables](./getpivottables/) | Obtiene todas las tablas dinámicas en esta hoja de cálculo. |
| [GetListObjects](./getlistobjects/) | Obtiene todos los ListObjects en esta hoja de cálculo. |
| [GetTabId](./gettabid/) | Especifica el identificador interno de la hoja. |
| [SetTabId](./settabid/) | Especifica el identificador interno de la hoja. |
| [GetHorizontalPageBreaks](./gethorizontalpagebreaks/) | Obtiene la colección HorizontalPageBreakCollection. |
| [GetVerticalPageBreaks](./getverticalpagebreaks/) | Obtiene la colección VerticalPageBreakCollection. |
| [AddPageBreaks](./addpagebreaks/) | Agrega un salto de página. |
| [GetHyperlinks](./gethyperlinks/) | Obtiene la colección HyperlinkCollection. |
| [Copy_Worksheet](./copy_worksheet/) | Copia el contenido y los formatos de otra hoja de cálculo. |
| [Copy_Worksheet_CopyOptions](./copy_worksheet_copyoptions/) | Copia el contenido y los formatos de otra hoja de cálculo. |
| [AutoFitColumn_Int_Int_Int](./autofitcolumn_int_int_int/) | Ajusta automáticamente el ancho de la columna. |
| [AutoFitColumns](./autofitcolumns/) | Ajusta automáticamente todas las columnas en esta hoja de cálculo. |
| [AutoFitColumns_AutoFitterOptions](./autofitcolumns_autofitteroptions/) | Ajusta automáticamente todas las columnas en esta hoja de cálculo. |
| [AutoFitColumn_Int](./autofitcolumn_int/) | Ajusta automáticamente el ancho de la columna. |
| [AutoFitColumns_Int_Int](./autofitcolumns_int_int/) | Ajusta automáticamente el ancho de las columnas. |
| [AutoFitColumns_Int_Int_AutoFitterOptions](./autofitcolumns_int_int_autofitteroptions/) | Ajusta automáticamente el ancho de las columnas. |
| [AutoFitColumns_Int_Int_Int_Int](./autofitcolumns_int_int_int_int/) | Ajusta automáticamente el ancho de las columnas. |
| [AutoFitColumns_Int_Int_Int_Int_AutoFitterOptions](./autofitcolumns_int_int_int_int_autofitteroptions/) | Ajusta automáticamente el ancho de las columnas. |
| [AutoFitRow_Int_Int_Int](./autofitrow_int_int_int/) | Ajusta automáticamente la altura de la fila. |
| [AutoFitRow_Int_Int_Int_AutoFitterOptions](./autofitrow_int_int_int_autofitteroptions/) | Ajusta automáticamente la altura de la fila. |
| [AutoFitRows](./autofitrows/) | Ajusta automáticamente todas las filas en esta hoja de cálculo. |
| [AutoFitRows_Bool](./autofitrows_bool/) | Ajusta automáticamente todas las filas en esta hoja de cálculo. |
| [AutoFitRows_AutoFitterOptions](./autofitrows_autofitteroptions/) | Ajusta automáticamente todas las filas en esta hoja de cálculo. |
| [AutoFitRows_Int_Int](./autofitrows_int_int/) | Ajusta automáticamente la altura de la fila en un rango. |
| [AutoFitRows_Int_Int_AutoFitterOptions](./autofitrows_int_int_autofitteroptions/) | Ajusta automáticamente la altura de la fila en un rango. |
| [AutoFitRow_Int_Int_Int_Int](./autofitrow_int_int_int_int/) | Ajusta automáticamente la altura de la fila en un rango rectangular. |
| [AutoFitRow_Int](./autofitrow_int/) | Ajusta automáticamente la altura de la fila. |
| [GetPageSetup](./getpagesetup/) | Representa la descripción de la configuración de página en esta hoja. |
| [GetAutoFilter](./getautofilter/) | Representa el filtro automático para la hoja de cálculo especificada. |
| [Filter](./filter/) | Filtra el rango. |
| [GetAdvancedFilter](./getadvancedfilter/) | Obtiene la configuración del filtro avanzado. |
| [Advanced_Filter](./advanced_filter/) | Filtra datos usando criterios complejos. |
| [RemoveAutoFilter](./removeautofilter/) | Elimina el filtro automático de la hoja de cálculo. |
| [GetHasAutofilter](./gethasautofilter/) | Indica si esta hoja de cálculo tiene filtro automático. |
| [GetTransitionEvaluation](./gettransitionevaluation/) | Indica si la opción Evaluación de Fórmula de Transición (compatibilidad con Lotus) está habilitada. |
| [SetTransitionEvaluation](./settransitionevaluation/) | Indica si la opción Evaluación de Fórmula de Transición (compatibilidad con Lotus) está habilitada. |
| [GetTransitionEntry](./gettransitionentry/) | Indica si la opción Entrada de Fórmula de Transición (compatibilidad con Lotus) está habilitada. |
| [SetTransitionEntry](./settransitionentry/) | Indica si la opción Entrada de Fórmula de Transición (compatibilidad con Lotus) está habilitada. |
| [GetVisibilityType](./getvisibilitytype/) | Indica el estado visible de esta hoja. |
| [SetVisibilityType](./setvisibilitytype/) | Indica el estado visible de esta hoja. |
| [SetVisible](./setvisible/) | Establece las opciones visibles. |
| [IsVisible](./isvisible/) | Representa si la hoja de cálculo es visible. |
| [SetIsVisible](./setisvisible/) | Representa si la hoja de cálculo es visible. |
| [SelectRange](./selectrange/) | Selecciona un rango. |
| [RemoveAllDrawingObjects](./removealldrawingobjects/) | Elimina todos los objetos de dibujo en esta hoja de cálculo. |
| [ClearComments](./clearcomments/) | Borra todos los comentarios en la hoja de cálculo del diseñador. |
| [GetSparklineGroups](./getsparklinegroups/) | Obtiene los grupos de sparkline en la hoja de cálculo. |
| [GetCharts](./getcharts/) | Obtiene una colección de gráficos |
| [GetComments](./getcomments/) | Obtiene la colección de comentarios. |
| [GetPictures](./getpictures/) | Obtiene una colección de imágenes. |
| [GetAllPictures](./getallpictures/) | Obtiene todas las imágenes, incluidas las que están incrustadas en la celda y sobre las celdas. |
| [GetTextBoxes](./gettextboxes/) | Obtiene una colección de cuadros de texto. |
| [GetCheckBoxes](./getcheckboxes/) | Obtiene una colección de casillas de verificación. |
| [GetOleObjects](./getoleobjects/) | Representa una colección de OleObject en una hoja de cálculo. |
| [GetShapes](./getshapes/) | Devuelve todas las formas de dibujo en esta hoja de cálculo. |
| [GetSlicers](./getslicers/) | Obtén la colección de segmentadores en la hoja de cálculo |
| [GetTimelines](./gettimelines/) | Obtén la colección de líneas de tiempo en la hoja de cálculo |
| [Protect_ProtectionType](./protect_protectiontype/) | Protege la hoja de cálculo. |
| [Protect_ProtectionType_String_String](./protect_protectiontype_string_string/) | Protege la hoja de cálculo. |
| [Unprotect](./unprotect/) | Desprotege la hoja de cálculo. |
| [Unprotect_String](./unprotect_string/) | Desprotege la hoja de cálculo. |
| [GetIndex](./getindex/) | Obtiene el índice de la hoja en la colección de hojas de cálculo. |
| [MoveTo](./moveto/) | Mueve la hoja a otra ubicación en la hoja de cálculo. |
| [IsProtected](./isprotected/) | Indica si la hoja de cálculo está protegida. |
| [GetValidations](./getvalidations/) | Obtiene la colección de configuraciones de validación de datos en la hoja de cálculo. |
| [GetAllowEditRanges](./getalloweditranges/) | Obtiene la colección de rangos de edición permitida en la hoja de cálculo. |
| [GetErrorCheckOptions](./geterrorcheckoptions/) | Obtiene la configuración de comprobación de errores aplicada a ciertos rangos. |
| [GetOutline](./getoutline/) | Obtiene el contorno en esta hoja de cálculo. |
| [GetFirstVisibleRow](./getfirstvisiblerow/) | Representa el índice de la primera fila visible. |
| [SetFirstVisibleRow](./setfirstvisiblerow/) | Representa el índice de la primera fila visible. |
| [GetFirstVisibleColumn](./getfirstvisiblecolumn/) | Representa el índice de la primera columna visible. |
| [SetFirstVisibleColumn](./setfirstvisiblecolumn/) | Representa el índice de la primera columna visible. |
| [Replace](./replace/) | Reemplaza el texto de todas las celdas con una nueva cadena. |
| [GetZoom](./getzoom/) | Representa el factor de escala en porcentaje. Debe estar entre 10 y 400. |
| [SetZoom](./setzoom/) | Representa el factor de escala en porcentaje. Debe estar entre 10 y 400. |
| [GetViewType](./getviewtype/) | Obtiene y establece el tipo de vista. |
| [SetViewType](./setviewtype/) | Obtiene y establece el tipo de vista. |
| [IsPageBreakPreview](./ispagebreakpreview/) | Indica si la hoja de cálculo especificada se muestra en vista normal o en vista previa de salto de página. |
| [SetIsPageBreakPreview](./setispagebreakpreview/) | Indica si la hoja de cálculo especificada se muestra en vista normal o en vista previa de salto de página. |
| [IsRulerVisible](./isrulervisible/) | Indica si la regla es visible. Esta propiedad solo se aplica en la vista previa de salto de página. |
| [SetIsRulerVisible](./setisrulervisible/) | Indica si la regla es visible. Esta propiedad solo se aplica en la vista previa de salto de página. |
| [GetSelectedAreas](./getselectedareas/) | Obtiene los rangos de celdas seleccionados en la hoja de cálculo del diseñador. |
| [GetTabColor](./gettabcolor/) | Representa el color de la pestaña de la hoja de cálculo. |
| [SetTabColor](./settabcolor/) | Representa el color de la pestaña de la hoja de cálculo. |
| [GetGridlineColor](./getgridlinecolor/) | Obtiene y establece el color de la línea de cuadrícula |
| [SetGridlineColor](./setgridlinecolor/) | Obtiene y establece el color de la línea de cuadrícula |
| [GetCodeName](./getcodename/) | Obtiene el nombre de código de la hoja de cálculo. |
| [SetCodeName](./setcodename/) | Obtiene el nombre de código de la hoja de cálculo. |
| [GetBackgroundImage](./getbackgroundimage/) | Obtiene y establece la imagen de fondo de la hoja de cálculo. |
| [SetBackgroundImage](./setbackgroundimage/) | Obtiene y establece la imagen de fondo de la hoja de cálculo. |
| [GetConditionalFormattings](./getconditionalformattings/) | Obtiene los ConditionalFormattings en la hoja de cálculo. |
| [GetActiveCell](./getactivecell/) | Obtiene o establece la celda activa en la hoja de cálculo. |
| [SetActiveCell](./setactivecell/) | Obtiene o establece la celda activa en la hoja de cálculo. |
| [GetCustomProperties](./getcustomproperties/) | Obtiene un objeto que representa la información de identificador asociada a una hoja de cálculo. |
| [GetPrintingPageBreaks](./getprintingpagebreaks/) | Obtiene los saltos de página automáticos. |
| [GetSmartTagSetting](./getsmarttagsetting/) | Obtiene todos los objetos SmartTagCollection de la hoja de cálculo. |
| [ToString](./tostring/) | Devuelve una cadena que representa el objeto Worksheet actual. |
| [GetScenarios](./getscenarios/) | Obtiene la colección de Scenario. |
| [StartAccessCache](./startaccesscache/) | Inicia la sesión que usa cachés para acceder a los datos en esta hoja de cálculo. |
| [CloseAccessCache](./closeaccesscache/) | Cierra la sesión que usa cachés para acceder a los datos en esta hoja de cálculo. |
| [ConvertFormulaReferenceStyle](./convertformulareferencestyle/) | Convierte el estilo de referencia de la fórmula. |
| [CalculateFormula_String](./calculateformula_string/) | Calcula una fórmula. |
| [CalculateFormula_String_CalculationOptions](./calculateformula_string_calculationoptions/) | Calcula una expresión de fórmula directamente. |
| [CalculateFormula_String_FormulaParseOptions_CalculationOptions_Int_Int_CalculationData](./calculateformula_string_formulaparseoptions_calculationoptions_int_int_calculationdata/) | Calcula una expresión de fórmula directamente. |
| [CalculateArrayFormula_String_CalculationOptions](./calculatearrayformula_string_calculationoptions/) | Calcula una fórmula como fórmula de matriz. |
| [CalculateArrayFormula_String_CalculationOptions_Int_Int](./calculatearrayformula_string_calculationoptions_int_int/) | Calcula una fórmula como fórmula de matriz. |
| [CalculateArrayFormula_String_FormulaParseOptions_CalculationOptions_Int_Int_Int_Int_CalculationData](./calculatearrayformula_string_formulaparseoptions_calculationoptions_int_int_int_int_calculationdata/) | Calcula una fórmula como fórmula de matriz. |
| [CalculateFormula_CalculationOptions_Bool](./calculateformula_calculationoptions_bool/) | Calcula todas las fórmulas en esta hoja de cálculo. |
| [GetAreasOfXmlMapQuery](./getareasofxmlmapquery/) | Consulta áreas de celdas que están mapeadas/enlazadas a la ruta específica del mapa xml. |
| [GetCellWatches](./getcellwatches/) | Obtiene la colección de celdas en esta hoja de cálculo que se están observando en la 'ventana de observación'. |
| [RefreshPivotTables](./refreshpivottables/) | Actualiza todas las tablas dinámicas en esta hoja de cálculo. |
| [RefreshPivotTables_PivotTableRefreshOption](./refreshpivottables_pivottablerefreshoption/) | Actualiza todas las tablas dinámicas en esta hoja de cálculo. |
