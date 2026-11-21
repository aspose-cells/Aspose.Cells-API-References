---
title: "GridWeb"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "La clase básica del control GridWeb."
type: docs
url: /es/java/com.aspose.gridweb/gridweb/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.WebControl](../../com.aspose.gridweb/webcontrol), [com.aspose.gridweb.ExtWebControl](../../com.aspose.gridweb/extwebcontrol), [com.aspose.gridweb.MainWeb](../../com.aspose.gridweb/mainweb)
```
public class GridWeb extends MainWeb
```

La clase básica del control GridWeb.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [GridWeb()](#GridWeb--) |  |
## Campos

| Campo | Descripción |
| --- | --- |
| [AfterColumnFilter](#AfterColumnFilter) | Ocurre después de que la columna se haya filtrado. |
| [AjaxCallFinished](#AjaxCallFinished) | Se dispara cuando la actualización ajax del control ha finalizado. |
| [BeforeColumnFilter](#BeforeColumnFilter) | Ocurre antes de que la columna sea filtrada. |
| [CellClickOnAjax](#CellClickOnAjax) | Ocurre cuando la celda se hace clic, y es necesario realizar ajaxcallback para este evento. |
| [CellClientUpdate](#CellClientUpdate) | Ocurre cuando ocurre una actualización de celda del cliente. |
| [CellCommand](#CellCommand) | Ocurre cuando se hace clic en el hipervínculo de comando de una celda. |
| [CellDoubleClick](#CellDoubleClick) | Ocurre cuando la celda se hace doble clic. |
| [CellModifiedOnAjax](#CellModifiedOnAjax) | Ocurre cuando la celda se modifica en ajaxcall. |
| [ColumnDeleted](#ColumnDeleted) | Ocurre cuando el usuario elimina una columna del menú del lado del cliente. |
| [ColumnDeleting](#ColumnDeleting) | Ocurre cuando el usuario intenta eliminar una columna del menú del lado del cliente. |
| [ColumnDoubleClick](#ColumnDoubleClick) | Ocurre cuando el encabezado de la columna se hace doble clic. |
| [ColumnInserted](#ColumnInserted) | Ocurre cuando el usuario inserta una columna desde el menú del lado del cliente. |
| [CustomCommand](#CustomCommand) | Ocurre cuando el usuario hace clic en un botón de comando personalizado. |
| [LoadCustomData](#LoadCustomData) | Se dispara cuando el SessionMode del control está configurado a Custom y necesita cargar los datos de la hoja. |
| [PageIndexChanged](#PageIndexChanged) | Ocurre cuando el índice de página de la hoja del control cambia. |
| [RowDeleted](#RowDeleted) | Ocurre cuando el usuario ha eliminado una fila del menú del lado del cliente. |
| [RowDeleting](#RowDeleting) | Ocurre cuando el usuario intenta eliminar una fila del menú del lado del cliente. |
| [RowDoubleClick](#RowDoubleClick) | Ocurre cuando el encabezado de fila se hace doble clic. |
| [RowInserted](#RowInserted) | Ocurre cuando el usuario inserta una fila desde el menú del lado del cliente. |
| [SaveCommand](#SaveCommand) | Ocurre cuando se hace clic en el botón "save". |
| [SheetAdded](#SheetAdded) | Ocurre cuando el usuario agrega una hoja de cálculo desde el menú de la barra de herramientas. |
| [SheetTabClick](#SheetTabClick) | Ocurre cuando se hace clic en la pestaña de la hoja. |
| [SubmitCommand](#SubmitCommand) | Ocurre cuando se hace clic en el botón "submit". |
| [UndoCommand](#UndoCommand) | Ocurre cuando se hace clic en el botón "undo". |
## Métodos

| Método | Descripción |
| --- | --- |
| [calculateFormula()](#calculateFormula--) | Calcula el resultado de las fórmulas. |
| [createChildControls()](#createChildControls--) | Implementa CreateChildControls de WebControl, solo de uso interno. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getACWClientPath()](#getACWClientPath--) | Obtiene la ruta web de los archivos de script/imagen del control. |
| [getACWLanguageFileUrl()](#getACWLanguageFileUrl--) | Obtiene la URL web del archivo de idioma del control. |
| [getActiveCell()](#getActiveCell--) | Obtiene la celda activa de la hoja actual. |
| [getActiveCellBgColor()](#getActiveCellBgColor--) | Especifica el color de fondo de la celda activa. |
| [getActiveCellColor()](#getActiveCellColor--) | Especifica el color de la celda activa. |
| [getActiveHeaderBgColor()](#getActiveHeaderBgColor--) | Especifica el color de fondo del encabezado activo de fila/columna. |
| [getActiveHeaderColor()](#getActiveHeaderColor--) | Especifica el color del encabezado activo de fila/columna. |
| [getActiveSheet()](#getActiveSheet--) | Obtiene la hoja activa |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | Obtiene el índice de la hoja activa. |
| [getActiveTabStyle()](#getActiveTabStyle--) | Especifica el estilo de la pestaña activa. |
| [getAutoRefreshChart()](#getAutoRefreshChart--) | Obtiene si la imagen del Chart se actualiza al actualizar el valor de la celda. El valor predeterminado es true. |
| [getBackColor()](#getBackColor--) | Obtiene el BackColor en el WebControl |
| [getBorderColor()](#getBorderColor--) | Obtiene el BorderColor en el WebControl |
| [getBorderStyle()](#getBorderStyle--) | Obtiene el BorderStyle en el WebControl |
| [getBorderWidth()](#getBorderWidth--) | Obtiene el BorderWidth en el WebControl |
| [getBottomTableStyle()](#getBottomTableStyle--) | Obtiene el estilo de la barra inferior del control. |
| [getClass()](#getClass--) |  |
| [getCssClass()](#getCssClass--) | Obtiene el CssClass en el WebControl |
| [getCurrentPageIndex()](#getCurrentPageIndex--) | Obtiene el índice de página actual en modo paginación. |
| [getCustomCalculationEngine()](#getCustomCalculationEngine--) | Representa el motor de cálculo personalizado del usuario para ampliar el motor de cálculo predeterminado de Aspose.Cells. |
| [getCustomCommandButtons()](#getCustomCommandButtons--) | Obtiene la colección de botones de comando personalizados |
| [getCustomStyleFileName()](#getCustomStyleFileName--) | Obtiene el nombre del archivo de estilo personalizado. |
| [getDPI()](#getDPI--) | Obtiene /Establece los DPI de la máquina. |
| [getDefaultFontName()](#getDefaultFontName--) | Obtiene el nombre de fuente predeterminado del control. |
| [getDefaultFontSize()](#getDefaultFontSize--) | Obtiene el tamaño de fuente predeterminado del control. |
| [getDefaultGridLineColor()](#getDefaultGridLineColor--) | Obtiene el color predeterminado de la línea de la cuadrícula. |
| [getDisplayCellTip()](#getDisplayCellTip--) | Obtiene si se deben mostrar sugerencias. El valor predeterminado es verdadero. |
| [getEditMode()](#getEditMode--) | Obtiene el modo de edición del control. |
| [getEnableAJAX()](#getEnableAJAX--) | Obtiene si se debe usar la llamada AJAX. El valor predeterminado es verdadero. |
| [getEnableAsync()](#getEnableAsync--) | Obtiene si se cargan los datos de celdas de forma asíncrona, se sugiere aplicarlo para una hoja con más de 10000 celdas. |
| [getEnableClientColumnOperations()](#getEnableClientColumnOperations--) | Obtiene si se habilitan las operaciones de columna del lado del cliente. |
| [getEnableClientFreeze()](#getEnableClientFreeze--) | Obtiene si se habilitan las operaciones de congelación del lado del cliente. |
| [getEnableClientMergeOperations()](#getEnableClientMergeOperations--) | Obtiene si se habilitan las operaciones de combinación del lado del cliente. |
| [getEnableClientResizeColumnRow()](#getEnableClientResizeColumnRow--) | Obtiene si se habilita el redimensionamiento de columnas y filas del lado del cliente. |
| [getEnableClientRowOperations()](#getEnableClientRowOperations--) | Obtiene si se habilitan las operaciones de fila del lado del cliente. |
| [getEnableDoubleClickEvent()](#getEnableDoubleClickEvent--) | Obtiene si se habilita el evento de doble clic del lado del cliente. |
| [getEnableMetalLightEffect()](#getEnableMetalLightEffect--) | Obtiene si se aplica el efecto de luz metálica. |
| [getEnablePaging()](#getEnablePaging--) | Obtiene si se habilita el modo de paginación del control. |
| [getEnableStyleDialogbox()](#getEnableStyleDialogbox--) | Obtiene si se habilita el cuadro de diálogo de estilo del lado del cliente. |
| [getEnabled()](#getEnabled--) | Obtiene el Enabled en el WebControl |
| [getFilteredPaging()](#getFilteredPaging--) | Obtiene si se habilita la paginación después de filtrar los datos, tendrá efecto cuando EnablePaging sea verdadero. |
| [getFont()](#getFont--) | Obtiene el Font en el WebControl |
| [getForceValidation()](#getForceValidation--) | Obtiene si se fuerza la validación del lado del cliente. |
| [getForeColor()](#getForeColor--) | Obtiene el ForeColor en el WebControl |
| [getFrameTableStyle()](#getFrameTableStyle--) | Obtiene el estilo del marco del control. |
| [getGoonDefaultSaveOperation()](#getGoonDefaultSaveOperation--) | Obtiene si GridWeb realizará la operación de guardado predeterminada, el valor predeterminado es verdadero. |
| [getHeaderBarHeight()](#getHeaderBarHeight--) | Obtiene la altura (System.Web.UI.WebControl.Unit) de la barra de encabezado superior del control. |
| [getHeaderBarStyle()](#getHeaderBarStyle--) | Obtiene el estilo de la barra de encabezado. |
| [getHeaderBarTableStyle()](#getHeaderBarTableStyle--) | Obtiene el estilo de la barra de encabezado del control. |
| [getHeaderBarWidth()](#getHeaderBarWidth--) | Obtiene el ancho( System.Web.UI.WebControl.Unit ) o la barra de encabezado izquierda del control. |
| [getHeight()](#getHeight--) | Obtiene la altura( System.Web.UI.WebControl.Unit ) del control. |
| [getIgnoreStyleWithNoData()](#getIgnoreStyleWithNoData--) | Obtiene si GridWeb ignora la visualización de filas o columnas que no contienen valores de celda pero que aún están con estilo. |
| [getLoadOptions()](#getLoadOptions--) | Representa las opciones de carga para GridWeb. |
| [getMaxColumn()](#getMaxColumn--) | Obtiene el índice máximo de columna visible (basado en cero) de la hoja web. |
| [getMaxRow()](#getMaxRow--) | Obtiene el índice máximo de fila visible (basado en cero) de la hoja web. |
| [getMessage()](#getMessage--) | Obtiene el mensaje para la cuadrícula. |
| [getMinColumn()](#getMinColumn--) | Obtiene el índice mínimo de columna visible (basado en cero) de la hoja web. |
| [getMinRow()](#getMinRow--) | Obtiene el índice mínimo de fila visible (basado en cero) de la hoja web. |
| [getModifiedCells()](#getModifiedCells--) | Obtiene la colección de celdas modificadas por el cliente. |
| [getNeedRenderGroupRows()](#getNeedRenderGroupRows--) | Obtiene si se deben mostrar filas de grupo. |
| [getNoHScroll()](#getNoHScroll--) | Obtiene un valor que indica si la barra de desplazamiento horizontal está oculta. |
| [getNoScroll()](#getNoScroll--) | Obtiene si se debe mostrar la barra de desplazamiento. |
| [getNoVScroll()](#getNoVScroll--) | Obtiene un valor que indica si la barra de desplazamiento vertical está oculta. |
| [getOnAjaxCallFinishedClientFunction()](#getOnAjaxCallFinishedClientFunction--) | Obtiene el nombre de la función del lado del cliente que se llamará cuando finalice la llamada ajax. |
| [getOnCellErrorClientFunction()](#getOnCellErrorClientFunction--) | Obtiene el nombre de la función del lado del cliente que se llamará cuando falle la validación de una celda. |
| [getOnCellSelectedAjaxCallBackClientFunction()](#getOnCellSelectedAjaxCallBackClientFunction--) | Obtiene la función del lado del cliente que se llamará cuando se seleccione una celda. |
| [getOnCellSelectedClientFunction()](#getOnCellSelectedClientFunction--) | Obtiene la función del lado del cliente que se llamará cuando se seleccione una celda. |
| [getOnCellUnselectedClientFunction()](#getOnCellUnselectedClientFunction--) | Obtiene la función del lado del cliente que se llamará cuando se deseleccione una celda. |
| [getOnCellUpdatedClientFunction()](#getOnCellUpdatedClientFunction--) | Obtiene el nombre de la función del lado del cliente que se llamará cuando se actualice el valor de una celda. |
| [getOnContextMenuShowClientFunction()](#getOnContextMenuShowClientFunction--) | Obtiene la función del lado del cliente que se llamará cuando se muestre el menú contextual. |
| [getOnDoubleClickCellClientFunction()](#getOnDoubleClickCellClientFunction--) | Obtiene el nombre de la función del lado del cliente que se llamará cuando se haga doble clic en una celda. |
| [getOnDoubleClickRowClientFunction()](#getOnDoubleClickRowClientFunction--) | Obtiene la función del lado del cliente que se llamará cuando se haga doble clic en una fila. |
| [getOnGridInitClientFunction()](#getOnGridInitClientFunction--) | Obtiene el nombre de la función del lado del cliente que se llamará cuando la cuadrícula se inicialice. |
| [getOnPageChangeClientFunction()](#getOnPageChangeClientFunction--) | Obtiene la función del lado del cliente que se llamará después de cambiar el índice de página. Solo tiene efecto cuando EnablePaging es verdadero. |
| [getOnPageSubmitClientFunction()](#getOnPageSubmitClientFunction--) | Obtiene la función del cliente que se llamará antes de que la página se envíe del lado del cliente. |
| [getOnShapeSelectedClientFunction()](#getOnShapeSelectedClientFunction--) | Obtiene la función del lado del cliente que se llamará cuando se seleccione una forma. |
| [getOnSubmitClientFunction()](#getOnSubmitClientFunction--) | Obtiene la función del cliente que se llamará antes de que el control se envíe en el lado del cliente. |
| [getOnlyAuto()](#getOnlyAuto--) | Obtiene si solo se ajustan las filas cuya altura no está personalizada, el valor predeterminado es false |
| [getPageSize()](#getPageSize--) | Obtiene el tamaño de página en modo de paginación. |
| [getPictureCachePath()](#getPictureCachePath--) | Obtiene la ruta de almacenamiento de imágenes para el libro de trabajo, todas las formas e imágenes se almacenarán en este directorio, la ruta predeterminada es acwcache bajo el Directorio Base de la aplicación actual; los usuarios deben implementar un servicio programado para limpiar los archivos que estén fuera del tiempo de sesión. |
| [getPresetStyle()](#getPresetStyle--) | Obtiene el estilo predefinido. |
| [getRefreshValidation()](#getRefreshValidation--) | Obtiene si se debe actualizar el valor de validación después de que cambie el valor de la celda. |
| [getRenderHiddenRow()](#getRenderHiddenRow--) | Obtiene si la fila oculta se representa en GridControl, el valor predeterminado es false. |
| [getRowHeightForCSV()](#getRowHeightForCSV--) | Obtiene el valor de la altura de fila en puntos para el archivo csv, el valor predeterminado es 14.5. |
| [getScrollBarArrowColor()](#getScrollBarArrowColor--) | Especifica el color del botón de flecha de la barra de desplazamiento. |
| [getScrollBarBaseColor()](#getScrollBarBaseColor--) | Especifica el color de la barra de desplazamiento del control. |
| [getSelectCellBgColor()](#getSelectCellBgColor--) | Especifica el color de fondo de las celdas seleccionadas en un rango de selección múltiple. |
| [getSelectCellColor()](#getSelectCellColor--) | Especifica el color de las celdas seleccionadas en un rango de selección múltiple. |
| [getSelectCells()](#getSelectCells--) | Obtiene la colección de celdas seleccionadas. |
| [getSessionStorePath()](#getSessionStorePath--) | Obtiene la ruta de almacenamiento de caché de sesión cuando el modo de sesión es File o ViewState, etc.: gridweb.SessionStorePath="c:/mytempdir/session"; luego almacenará los datos de sesión en c:/mytempdir/session |
| [getSettings()](#getSettings--) | Representa la configuración del libro de trabajo. |
| [getShowAddButton()](#getShowAddButton--) | Obtiene si se muestra el botón de agregar hoja de cálculo. |
| [getShowBottomBar()](#getShowBottomBar--) | Especifica si se muestra la barra de comandos (incluye barra de comandos y barra de pestañas) en la parte inferior del control. |
| [getShowCellEditBox()](#getShowCellEditBox--) | si Gridweb muestra la barra de herramientas del cuadro de edición como en MS-EXCEL. Si está habilitado, se mostrará un cuadro de edición para la celda actual en Gridweb. |
| [getShowCommandBarAtTop()](#getShowCommandBarAtTop--) | Especifica si se muestra la barra de comandos (incluye barra de comandos y barra de pestañas) en la parte superior del control. |
| [getShowContextMenu()](#getShowContextMenu--) | Obtiene si se muestra el menú contextual. El valor predeterminado es true. |
| [getShowDefaultGridLine()](#getShowDefaultGridLine--) | Obtiene si se muestran las líneas de cuadrícula predeterminadas de las celdas. |
| [getShowHeaderBar()](#getShowHeaderBar--) | Obtiene si se muestra la barra de encabezado |
| [getShowLoading()](#getShowLoading--) | Especifica si se muestra un cuadro de diálogo de carga mientras se envía la solicitud al servidor. |
| [getShowLoadingPosition()](#getShowLoadingPosition--) | Especifica la posición izquierda y superior (en px) para mostrar el cuadro de diálogo de carga mientras se envía la solicitud al servidor, etc. 100,200 significa que la posición izquierda y superior del cuadro de diálogo de carga está en 100px,200px. |
| [getShowSaveButton()](#getShowSaveButton--) | Obtiene si se muestra el botón de guardar. |
| [getShowSubmitButton()](#getShowSubmitButton--) | Obtiene si se muestra el botón de envío. |
| [getShowTabBar()](#getShowTabBar--) | Obtiene si se muestra la barra de pestañas. |
| [getShowTabNavigation()](#getShowTabNavigation--) | Obtiene si el botón de navegación de pestañas se muestra, el valor predeterminado es true. |
| [getShowUndoButton()](#getShowUndoButton--) | Obtiene si se muestra el botón deshacer. |
| [getSpanWrap()](#getSpanWrap--) | Especifica si se envuelve el contenido en el cell span, el valor predeterminado es true. |
| [getTabIndex()](#getTabIndex--) | Obtiene el TabIndex en el WebControl |
| [getTabStyle()](#getTabStyle--) | Obtiene el estilo de la barra de pestañas. |
| [getToolTip()](#getToolTip--) | Obtiene el ToolTip en el WebControl |
| [getUseClientPageHeight()](#getUseClientPageHeight--) | Obtiene si gridweb usa la altura de la página del cliente como altura del control, adecuado para cuando se establece Height="100%", el valor predeterminado es false. |
| [getVersion()](#getVersion--) | Obtiene la versión de lanzamiento. |
| [getViewPanelScrollLeft()](#getViewPanelScrollLeft--) | Obtiene la posición de la barra de desplazamiento del panel de vista de la cuadrícula. |
| [getViewPanelScrollTop()](#getViewPanelScrollTop--) | Obtiene la posición de la barra de desplazamiento del panel de vista de la cuadrícula. |
| [getViewTableStyle()](#getViewTableStyle--) | Obtiene el estilo del panel de vista de datos. |
| [getWidth()](#getWidth--) | Obtiene el ancho (System.Web.UI.WebControl.Unit) del control. |
| [getWorkSheets()](#getWorkSheets--) | Obtiene la colección de las hojas de cálculo. |
| [getXhtmlMode()](#getXhtmlMode--) | Obtiene si se usa el estilo XHTML, el valor predeterminado es true. |
| [hashCode()](#hashCode--) |  |
| [importExcelFile(InputStream stream)](#importExcelFile-java.io.InputStream-) | Importa desde un flujo de archivo Excel, incluyendo flujo de archivo en disco o flujo de memoria. |
| [importExcelFile(InputStream stream, String passwordtoOpen)](#importExcelFile-java.io.InputStream-java.lang.String-) | Importa desde un flujo de archivo Excel, incluyendo flujo de archivo en disco o flujo de memoria. |
| [importExcelFile(String fileName)](#importExcelFile-java.lang.String-) | Importa desde un archivo Excel. |
| [importExcelFile(String fileName, String passwordtoOpen)](#importExcelFile-java.lang.String-java.lang.String-) | Importa desde un archivo Excel. |
| [isCalculateFormula()](#isCalculateFormula--) | Obtiene si se calcula la fórmula después de que cambie el valor de la celda o después de importar el archivo. |
| [loadCSVFile(InputStream stream)](#loadCSVFile-java.io.InputStream-) | Carga datos desde un flujo de archivo CSV. |
| [loadCSVFile(String fileName)](#loadCSVFile-java.lang.String-) | Carga datos desde un archivo CSV. |
| [loadHTMLFile(InputStream stream)](#loadHTMLFile-java.io.InputStream-) | Carga datos desde un flujo de archivo HTML. |
| [loadHTMLFile(String fileName)](#loadHTMLFile-java.lang.String-) | Carga datos desde un archivo HTML. |
| [loadSpreadSheetMLFile(InputStream stream)](#loadSpreadSheetMLFile-java.io.InputStream-) | Carga datos desde un flujo de archivo SpreadSheetML. |
| [loadSpreadSheetMLFile(String fileName)](#loadSpreadSheetMLFile-java.lang.String-) | Carga datos desde un archivo SpreadSheetML. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshChartShape()](#refreshChartShape--) | Actualiza todas las imágenes de gráficos para la hoja de cálculo activa. |
| [saveCSVFile(OutputStream stream)](#saveCSVFile-java.io.OutputStream-) | Guarda datos en un flujo de archivo CSV. |
| [saveCSVFile(String targetFile)](#saveCSVFile-java.lang.String-) | Guarda datos en un archivo CSV. |
| [saveCustomStyleFile(String fileName)](#saveCustomStyleFile-java.lang.String-) | Guarda los datos de estilo actuales del control en un archivo XML. |
| [saveHTMLFile(OutputStream stream)](#saveHTMLFile-java.io.OutputStream-) | Guarda datos en un flujo de archivo HTML. |
| [saveHTMLFile(String targetFile)](#saveHTMLFile-java.lang.String-) | Guarda datos en un archivo HTML. |
| [saveSpreadSheetMLFile(OutputStream stream)](#saveSpreadSheetMLFile-java.io.OutputStream-) | Guarda datos en un flujo de archivo SpreadSheetML. |
| [saveSpreadSheetMLFile(String targetFile)](#saveSpreadSheetMLFile-java.lang.String-) | Guarda datos en un archivo SpreadSheetML. |
| [saveToExcelFile(OutputStream stream)](#saveToExcelFile-java.io.OutputStream-) | Guarda las hojas de cálculo en un archivo excel. |
| [saveToExcelFile(OutputStream stream, GridSaveOptions saveOptions)](#saveToExcelFile-java.io.OutputStream-com.aspose.gridweb.GridSaveOptions-) | Guarda las hojas de cálculo en un archivo excel. |
| [saveToExcelFile(OutputStream stream, int format)](#saveToExcelFile-java.io.OutputStream-int-) | Guarda las hojas de cálculo en un archivo excel. |
| [saveToExcelFile(String targetFile)](#saveToExcelFile-java.lang.String-) | Guarda las hojas de cálculo en un archivo excel con formato Excel 2003. |
| [saveToExcelFile(String targetFile, GridSaveOptions saveOptions)](#saveToExcelFile-java.lang.String-com.aspose.gridweb.GridSaveOptions-) | Guarda las hojas de cálculo en un archivo excel. |
| [saveToExcelFile(String targetFile, int format)](#saveToExcelFile-java.lang.String-int-) | Guarda las hojas de cálculo en un archivo excel. |
| [setACWClientPath(String value)](#setACWClientPath-java.lang.String-) | Establece la ruta web de los archivos script/imagen del control. |
| [setACWLanguageFileUrl(String value)](#setACWLanguageFileUrl-java.lang.String-) | Establece la URL web del archivo de idioma del control. |
| [setActiveCell(GridCell value)](#setActiveCell-com.aspose.gridweb.GridCell-) | Establece la celda activa de la hoja actual. |
| [setActiveCellBgColor(Color value)](#setActiveCellBgColor-com.aspose.gridweb.Color-) | Especifica el color de fondo de la celda activa. |
| [setActiveCellColor(Color value)](#setActiveCellColor-com.aspose.gridweb.Color-) | Especifica el color de la celda activa. |
| [setActiveHeaderBgColor(Color value)](#setActiveHeaderBgColor-com.aspose.gridweb.Color-) | Especifica el color de fondo del encabezado activo de fila/columna. |
| [setActiveHeaderColor(Color value)](#setActiveHeaderColor-com.aspose.gridweb.Color-) | Especifica el color del encabezado activo de fila/columna. |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | Establece el índice de la hoja activa. |
| [setActiveTabStyle(GridTableItemStyle value)](#setActiveTabStyle-com.aspose.gridweb.GridTableItemStyle-) | Especifica el estilo de la pestaña activa. |
| [setAutoRefreshChart(boolean value)](#setAutoRefreshChart-boolean-) | Establece si la imagen Chart se actualiza al actualizar el valor de la celda. el valor predeterminado es true |
| [setBackColor(Color value)](#setBackColor-com.aspose.gridweb.Color-) | Establece el BackColor en el WebControl |
| [setBorderColor(Color value)](#setBorderColor-com.aspose.gridweb.Color-) | Establece el BorderColor en el WebControl |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Establece el BorderStyle en el WebControl |
| [setBorderWidth(Unit value)](#setBorderWidth-com.aspose.gridweb.Unit-) | Establece el BorderWidth en el WebControl |
| [setBottomTableStyle(GridTableStyle value)](#setBottomTableStyle-com.aspose.gridweb.GridTableStyle-) | Establece el estilo de la barra inferior del control. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Establece si calcular la fórmula después de que cambie el valor de la celda o después de importar el File. |
| [setCssClass(String value)](#setCssClass-java.lang.String-) | Establece el CssClass en el WebControl |
| [setCurrentPageIndex(int value)](#setCurrentPageIndex-int-) | Establece el índice de página actual en modo paginación. |
| [setCustomCalculationEngine(GridAbstractCalculationEngine value)](#setCustomCalculationEngine-com.aspose.gridweb.GridAbstractCalculationEngine-) | Representa el motor de cálculo personalizado del usuario para ampliar el motor de cálculo predeterminado de Aspose.Cells. |
| [setCustomStyle(InputStream stream)](#setCustomStyle-java.io.InputStream-) | establece el archivo de estilo personalizado desde un flujo, incluyendo flujo de archivo en disco o flujo de memoria. |
| [setCustomStyleFileName(String value)](#setCustomStyleFileName-java.lang.String-) | Establece el nombre del archivo de estilo personalizado. |
| [setDPI(double value)](#setDPI-double-) | Obtiene /Establece los DPI de la máquina. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Establece el nombre de fuente predeterminado del control. |
| [setDefaultFontSize(FontUnit value)](#setDefaultFontSize-com.aspose.gridweb.FontUnit-) | Establece el tamaño de fuente predeterminado del control. |
| [setDefaultGridLineColor(Color value)](#setDefaultGridLineColor-com.aspose.gridweb.Color-) | Establece el color predeterminado de la línea de cuadrícula. |
| [setDisplayCellTip(boolean value)](#setDisplayCellTip-boolean-) | Establece si mostrar sugerencias. el valor predeterminado es true. |
| [setEditMode(boolean value)](#setEditMode-boolean-) | Establece el modo de edición del control. |
| [setEnableAJAX(boolean value)](#setEnableAJAX-boolean-) | Establece si usar la llamada AJAX. el valor predeterminado es true. |
| [setEnableAsync(boolean value)](#setEnableAsync-boolean-) | Establece si cargar los datos de celdas de forma asíncrona, se sugiere aplicar para una hoja con más de 10000 celdas. |
| [setEnableClientColumnOperations(boolean value)](#setEnableClientColumnOperations-boolean-) | Establece si habilitar las operaciones de columna del lado del cliente. |
| [setEnableClientFreeze(boolean value)](#setEnableClientFreeze-boolean-) | Establece si habilitar las operaciones de congelación del lado del cliente. |
| [setEnableClientMergeOperations(boolean value)](#setEnableClientMergeOperations-boolean-) | Establece si habilitar las operaciones de combinación del lado del cliente. |
| [setEnableClientResizeColumnRow(boolean value)](#setEnableClientResizeColumnRow-boolean-) | Establece si se habilita el redimensionamiento de columnas y filas del lado del cliente. |
| [setEnableClientRowOperations(boolean value)](#setEnableClientRowOperations-boolean-) | Establece si se habilitan las operaciones de filas del lado del cliente. |
| [setEnableDoubleClickEvent(boolean value)](#setEnableDoubleClickEvent-boolean-) | Establece si se habilita el evento de doble clic del lado del cliente. |
| [setEnableMetalLightEffect(boolean value)](#setEnableMetalLightEffect-boolean-) | Establece si se aplica el efecto de luz metálica. |
| [setEnablePaging(boolean value)](#setEnablePaging-boolean-) | Establece si se habilita el modo de paginación del control. |
| [setEnableStyleDialogbox(boolean value)](#setEnableStyleDialogbox-boolean-) | Establece si se habilita el cuadro de diálogo de estilo del lado del cliente. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Establece el Enabled en el WebControl |
| [setFilteredPaging(boolean value)](#setFilteredPaging-boolean-) | Establece si se habilita la paginación después de filtrar los datos; tendrá efecto cuando EnablePaging sea verdadero. |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | Establece la carpeta de fuentes |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Establece las carpetas de fuentes |
| [setForceValidation(boolean value)](#setForceValidation-boolean-) | Establece si se fuerza la validación del lado del cliente. |
| [setForeColor(Color value)](#setForeColor-com.aspose.gridweb.Color-) | Establece el ForeColor en el WebControl |
| [setFrameTableStyle(GridTableStyle value)](#setFrameTableStyle-com.aspose.gridweb.GridTableStyle-) | Establece el estilo del marco del control. |
| [setGoonDefaultSaveOperation(boolean value)](#setGoonDefaultSaveOperation-boolean-) | Establece si GridWeb realizará la operación de guardado predeterminada; el valor predeterminado es verdadero. |
| [setHeaderBarHeight(Unit value)](#setHeaderBarHeight-com.aspose.gridweb.Unit-) | Establece la altura (System.Web.UI.WebControl.Unit) de la barra de encabezado superior del control. |
| [setHeaderBarStyle(GridTableItemStyle value)](#setHeaderBarStyle-com.aspose.gridweb.GridTableItemStyle-) | Establece el estilo de la barra de encabezado. |
| [setHeaderBarTableStyle(GridTableStyle value)](#setHeaderBarTableStyle-com.aspose.gridweb.GridTableStyle-) | Establece el estilo de la barra de encabezado del control. |
| [setHeaderBarWidth(Unit value)](#setHeaderBarWidth-com.aspose.gridweb.Unit-) | Establece el ancho (System.Web.UI.WebControl.Unit) de la barra de encabezado izquierda del control. |
| [setHeight(Unit value)](#setHeight-com.aspose.gridweb.Unit-) | Establece la altura (System.Web.UI.WebControl.Unit) del control. |
| [setIgnoreStyleWithNoData(boolean value)](#setIgnoreStyleWithNoData-boolean-) | Establece si GridWeb ignora la visualización de filas o columnas que no contienen valores de celda pero que aún tienen estilo. |
| [setLoadOptions(GridLoadOptions value)](#setLoadOptions-com.aspose.gridweb.GridLoadOptions-) | Representa las opciones de carga para GridWeb. |
| [setMaxColumn(int value)](#setMaxColumn-int-) | Establece el índice máximo de columna visible (basado en cero) de la hoja web. |
| [setMaxRow(int value)](#setMaxRow-int-) | Establece el índice máximo de fila visible (basado en cero) de la hoja web. |
| [setMessage(String value)](#setMessage-java.lang.String-) | Establece el mensaje para la cuadrícula. |
| [setMinColumn(int value)](#setMinColumn-int-) | Establece el índice mínimo de columna visible (basado en cero) de la hoja web. |
| [setMinRow(int value)](#setMinRow-int-) | Establece el índice mínimo de fila visible (basado en cero) de la hoja web. |
| [setNeedRenderGroupRows(boolean value)](#setNeedRenderGroupRows-boolean-) | Establece si se muestran las filas de grupo. |
| [setNoHScroll(boolean value)](#setNoHScroll-boolean-) | Establece un valor que indica si la barra de desplazamiento horizontal está oculta. |
| [setNoScroll(boolean value)](#setNoScroll-boolean-) | Establece si se muestra la barra de desplazamiento. |
| [setNoVScroll(boolean value)](#setNoVScroll-boolean-) | Establece un valor que indica si la barra de desplazamiento vertical está oculta. |
| [setOnAjaxCallFinishedClientFunction(String value)](#setOnAjaxCallFinishedClientFunction-java.lang.String-) | Establece el nombre de la función del lado del cliente que se llamará cuando la llamada ajax haya finalizado. |
| [setOnCellErrorClientFunction(String value)](#setOnCellErrorClientFunction-java.lang.String-) | Establece el nombre de la función del lado del cliente que se llamará cuando falle la validación de una celda. |
| [setOnCellSelectedAjaxCallBackClientFunction(String value)](#setOnCellSelectedAjaxCallBackClientFunction-java.lang.String-) | Establece la función del lado del cliente que se llamará cuando se seleccione una celda. |
| [setOnCellSelectedClientFunction(String value)](#setOnCellSelectedClientFunction-java.lang.String-) | Establece la función del lado del cliente que se llamará cuando se seleccione una celda. |
| [setOnCellUnselectedClientFunction(String value)](#setOnCellUnselectedClientFunction-java.lang.String-) | Establece la función del lado del cliente que se llamará cuando se deseleccione una celda. |
| [setOnCellUpdatedClientFunction(String value)](#setOnCellUpdatedClientFunction-java.lang.String-) | Establece el nombre de la función del lado del cliente que se llamará cuando se actualice el valor de una celda. |
| [setOnContextMenuShowClientFunction(String value)](#setOnContextMenuShowClientFunction-java.lang.String-) | Establece la función del lado del cliente que se llamará cuando se muestre el menú contextual. |
| [setOnDoubleClickCellClientFunction(String value)](#setOnDoubleClickCellClientFunction-java.lang.String-) | Establece la función del lado del cliente que se llamará cuando se haga doble clic en una celda. |
| [setOnDoubleClickRowClientFunction(String value)](#setOnDoubleClickRowClientFunction-java.lang.String-) | Establece la función del lado del cliente que se llamará cuando se haga doble clic en una fila. |
| [setOnGridInitClientFunction(String value)](#setOnGridInitClientFunction-java.lang.String-) | Establece el nombre de la función del lado del cliente que se llamará cuando se inicialice la cuadrícula. |
| [setOnPageChangeClientFunction(String value)](#setOnPageChangeClientFunction-java.lang.String-) | Establece la función del lado del cliente que se llamará después de cambiar el índice de página. Solo tiene efecto cuando EnablePaging es verdadero. |
| [setOnPageSubmitClientFunction(String value)](#setOnPageSubmitClientFunction-java.lang.String-) | Establece la función del cliente que se llamará antes de que la página se envíe del lado del cliente. |
| [setOnShapeSelectedClientFunction(String value)](#setOnShapeSelectedClientFunction-java.lang.String-) | Establece la función del lado del cliente que se llamará cuando se seleccione una forma. |
| [setOnSubmitClientFunction(String value)](#setOnSubmitClientFunction-java.lang.String-) | Establece la función del cliente que se llamará antes de que el control se envíe del lado del cliente. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | Establece si solo se ajustan las filas cuya altura no está personalizada, el valor predeterminado es false. |
| [setPageSize(int value)](#setPageSize-int-) | Establece el tamaño de página en modo de paginación. |
| [setPictureCachePath(String value)](#setPictureCachePath-java.lang.String-) | Establece la ruta de almacenamiento de imágenes para el libro de trabajo; todas las formas e imágenes se almacenarán en este directorio, la ruta predeterminada es acwcache bajo el Directorio Base de la aplicación actual. Los usuarios deben implementar un servicio programado para limpiar los archivos que estén fuera del tiempo de sesión. |
| [setPresetStyle(int value)](#setPresetStyle-int-) | Establece el estilo predefinido. |
| [setRefreshValidation(boolean value)](#setRefreshValidation-boolean-) | Establece si se actualiza el valor de validación después de que cambie el valor de la celda. |
| [setRenderHiddenRow(boolean value)](#setRenderHiddenRow-boolean-) | Establece si la fila oculta se renderiza en GridControl, el valor predeterminado es false. |
| [setRowHeightForCSV(double value)](#setRowHeightForCSV-double-) | Establece el valor de la altura de fila en puntos para el archivo csv, el valor predeterminado es 14.5. |
| [setScrollBarArrowColor(Color value)](#setScrollBarArrowColor-com.aspose.gridweb.Color-) | Especifica el color del botón de flecha de la barra de desplazamiento. |
| [setScrollBarBaseColor(Color value)](#setScrollBarBaseColor-com.aspose.gridweb.Color-) | Especifica el color de la barra de desplazamiento del control. |
| [setSelectCellBgColor(Color value)](#setSelectCellBgColor-com.aspose.gridweb.Color-) | Especifica el color de fondo de las celdas seleccionadas en un rango de selección múltiple. |
| [setSelectCellColor(Color value)](#setSelectCellColor-com.aspose.gridweb.Color-) | Especifica el color de las celdas seleccionadas en un rango de selección múltiple. |
| [setSessionStorePath(String value)](#setSessionStorePath-java.lang.String-) | Establece la ruta de almacenamiento de caché de sesión cuando el modo de sesión es File o ViewState, etc.: gridweb.SessionStorePath=\"c:/mytempdir/session\"; luego almacenará los datos de sesión en c:/mytempdir/session. |
| [setSettings(GridWorkbookSettings value)](#setSettings-com.aspose.gridweb.GridWorkbookSettings-) | Representa la configuración del libro de trabajo. |
| [setShowAddButton(boolean value)](#setShowAddButton-boolean-) | Establece si se muestra el botón de agregar hoja de cálculo. |
| [setShowBottomBar(boolean value)](#setShowBottomBar-boolean-) | Especifica si se muestra la barra de comandos (incluye barra de comandos y barra de pestañas) en la parte inferior del control. |
| [setShowCellEditBox(boolean value)](#setShowCellEditBox-boolean-) | si Gridweb muestra la barra de herramientas del cuadro de edición como en MS-EXCEL. Si está habilitado, se mostrará un cuadro de edición para la celda actual en Gridweb. |
| [setShowCommandBarAtTop(boolean value)](#setShowCommandBarAtTop-boolean-) | Especifica si se muestra la barra de comandos (incluye barra de comandos y barra de pestañas) en la parte superior del control. |
| [setShowContextMenu(boolean value)](#setShowContextMenu-boolean-) | Establece si se muestra el menú contextual. El valor predeterminado es true. |
| [setShowDefaultGridLine(boolean value)](#setShowDefaultGridLine-boolean-) | Establece si se muestran las líneas de cuadrícula predeterminadas de las celdas. |
| [setShowHeaderBar(boolean value)](#setShowHeaderBar-boolean-) | Establece si se muestra la barra de encabezado |
| [setShowLoading(boolean value)](#setShowLoading-boolean-) | Especifica si se muestra un cuadro de diálogo de carga mientras se envía la solicitud al servidor. |
| [setShowLoadingPosition(String value)](#setShowLoadingPosition-java.lang.String-) | Especifica la posición izquierda y superior (en px) para mostrar el cuadro de diálogo de carga mientras se envía la solicitud al servidor, etc. 100,200 significa que la posición izquierda y superior del cuadro de diálogo de carga está en 100px,200px. |
| [setShowSaveButton(boolean value)](#setShowSaveButton-boolean-) | Establece si se muestra el botón de guardar. |
| [setShowSubmitButton(boolean value)](#setShowSubmitButton-boolean-) | Establece si se muestra el botón de enviar. |
| [setShowTabBar(boolean value)](#setShowTabBar-boolean-) | Establece si se muestra la barra de pestañas. |
| [setShowTabNavigation(boolean value)](#setShowTabNavigation-boolean-) | Establece si el botón de navegación de pestañas se muestra, el valor predeterminado es verdadero. |
| [setShowUndoButton(boolean value)](#setShowUndoButton-boolean-) | Establece si se muestra el botón de deshacer. |
| [setSpanWrap(boolean value)](#setSpanWrap-boolean-) | Especifica si se envuelve el contenido en el cell span, el valor predeterminado es true. |
| [setTabIndex(short value)](#setTabIndex-short-) | Establece el TabIndex en el WebControl |
| [setTabStyle(GridTableItemStyle value)](#setTabStyle-com.aspose.gridweb.GridTableItemStyle-) | Establece el estilo de la barra de pestañas. |
| [setToolTip(String value)](#setToolTip-java.lang.String-) | Establece el ToolTip en el WebControl |
| [setUseClientPageHeight(boolean value)](#setUseClientPageHeight-boolean-) | Establece si GridWeb usa la altura de la página del cliente como altura del control, adecuado cuando se establece Height=\"100%\", el valor predeterminado es falso. |
| [setViewPanelScrollLeft(String value)](#setViewPanelScrollLeft-java.lang.String-) | Establece la posición de la barra de desplazamiento del panel de vista de la cuadrícula. |
| [setViewPanelScrollTop(String value)](#setViewPanelScrollTop-java.lang.String-) | Establece la posición de la barra de desplazamiento del panel de vista de la cuadrícula. |
| [setViewTableStyle(GridTableStyle value)](#setViewTableStyle-com.aspose.gridweb.GridTableStyle-) | Establece el estilo del panel de vista de datos. |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | Establece el ancho (System.Web.UI.WebControl.Unit) del control. |
| [setXhtmlMode(boolean value)](#setXhtmlMode-boolean-) | Establece si se usa el estilo XHTML, el valor predeterminado es verdadero. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridWeb() {#GridWeb--}
```
public GridWeb()
```


### AfterColumnFilter {#AfterColumnFilter}
```
public RowColumnEventHandler AfterColumnFilter
```


Ocurre después de que la columna se haya filtrado.

### AjaxCallFinished {#AjaxCallFinished}
```
public WorkbookEventHandler AjaxCallFinished
```


Se dispara cuando la actualización ajax del control ha finalizado. (EnableAJAX debe estar configurado como verdadero).

### BeforeColumnFilter {#BeforeColumnFilter}
```
public RowColumnEventHandler BeforeColumnFilter
```


Ocurre antes de que la columna sea filtrada.

### CellClickOnAjax {#CellClickOnAjax}
```
public CellEventStringHandler CellClickOnAjax
```


Ocurre cuando la celda se hace clic, y es necesario realizar ajaxcallback para este evento.

### CellClientUpdate {#CellClientUpdate}
```
public CellEventHandler CellClientUpdate
```


Ocurre cuando se produce una actualización de una celda del cliente. Cuando se dispara este evento, su parámetro e.Argument contiene el nombre del comando.

### CellCommand {#CellCommand}
```
public CellEventHandler CellCommand
```


Ocurre cuando se hace clic en el hipervínculo de comando de una celda. Cuando se dispara este evento, su parámetro e.Argument contiene el nombre del comando.

### CellDoubleClick {#CellDoubleClick}
```
public CellEventHandler CellDoubleClick
```


Ocurre cuando la celda se hace doble clic.

### CellModifiedOnAjax {#CellModifiedOnAjax}
```
public CellEventHandler CellModifiedOnAjax
```


Ocurre cuando la celda se modifica en ajaxcall.

### ColumnDeleted {#ColumnDeleted}
```
public RowColumnEventHandler ColumnDeleted
```


Ocurre cuando el usuario elimina una columna del menú del lado del cliente.

### ColumnDeleting {#ColumnDeleting}
```
public RowColumnEventHandler ColumnDeleting
```


Ocurre cuando el usuario intenta eliminar una columna del menú del lado del cliente. Puede manejar este evento y establecer el parámetro cancel en Verdadero para cancelar la operación de eliminación.

### ColumnDoubleClick {#ColumnDoubleClick}
```
public RowColumnEventHandler ColumnDoubleClick
```


Ocurre cuando el encabezado de la columna se hace doble clic.

### ColumnInserted {#ColumnInserted}
```
public RowColumnEventHandler ColumnInserted
```


Ocurre cuando el usuario inserta una columna desde el menú del lado del cliente.

### CustomCommand {#CustomCommand}
```
public CustomCommandEventHandler CustomCommand
```


Ocurre cuando el usuario hace clic en un botón de comando personalizado.

### LoadCustomData {#LoadCustomData}
```
public WorkbookEventHandler LoadCustomData
```


Se dispara cuando el SessionMode del control está configurado como Custom y necesita cargar datos de la hoja. Puede manejar este evento en modo de sesión personalizada para cargar los datos de la hoja desde un archivo o base de datos.

### PageIndexChanged {#PageIndexChanged}
```
public WorkbookEventHandler PageIndexChanged
```


Ocurre cuando el índice de página de la hoja del control cambia.

### RowDeleted {#RowDeleted}
```
public RowColumnEventHandler RowDeleted
```


Ocurre cuando el usuario ha eliminado una fila del menú del lado del cliente.

### RowDeleting {#RowDeleting}
```
public RowColumnEventHandler RowDeleting
```


Ocurre cuando el usuario intenta eliminar una fila del menú del lado del cliente. Puede manejar este evento y lanzar una excepción RejectDeleteException para cancelar la operación de eliminación.

### RowDoubleClick {#RowDoubleClick}
```
public RowColumnEventHandler RowDoubleClick
```


Ocurre cuando el encabezado de fila se hace doble clic.

### RowInserted {#RowInserted}
```
public RowColumnEventHandler RowInserted
```


Ocurre cuando el usuario inserta una fila desde el menú del lado del cliente.

### SaveCommand {#SaveCommand}
```
public WorkbookEventHandler SaveCommand
```


Ocurre cuando se hace clic en el botón "save".

### SheetAdded {#SheetAdded}
```
public SheetEventHandler SheetAdded
```


Ocurre cuando el usuario agrega una hoja de cálculo desde el menú de la barra de herramientas.

### SheetTabClick {#SheetTabClick}
```
public WorkbookEventHandler SheetTabClick
```


Ocurre cuando se hace clic en la pestaña de la hoja.

### SubmitCommand {#SubmitCommand}
```
public WorkbookEventHandler SubmitCommand
```


Ocurre cuando se hace clic en el botón "submit".

### UndoCommand {#UndoCommand}
```
public WorkbookEventHandler UndoCommand
```


Ocurre cuando se hace clic en el botón "undo".

### calculateFormula() {#calculateFormula--}
```
public void calculateFormula()
```


Calcula el resultado de las fórmulas.

### createChildControls() {#createChildControls--}
```
public void createChildControls()
```


Implementa CreateChildControls de WebControl, solo de uso interno.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getACWClientPath() {#getACWClientPath--}
```
public String getACWClientPath()
```


Obtiene la ruta web de los archivos de script/imagen del control. Por ejemplo: \"http://localhost/acw\\_client\". También puede establecer este valor en el archivo web.config. Añada esta sección al bloque `<configuration>`:
`<appSettings>`
`<add key=\"aspose.cells.gridweb.acw_client_path\" value=\"/acw_client/\" />`
`</appSettings>`


**Returns:**
java.lang.String
### getACWLanguageFileUrl() {#getACWLanguageFileUrl--}
```
public String getACWLanguageFileUrl()
```


Obtiene la URL web del archivo de idioma del control. Por ejemplo: \"/acw\\_client/lang\\_en.js\".
Por defecto, se utiliza un archivo inglés incorporado.


**Returns:**
java.lang.String
### getActiveCell() {#getActiveCell--}
```
public GridCell getActiveCell()
```


Obtiene la celda activa de la hoja actual. Cambiado a editable desde la versión 1.9.0.1.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getActiveCellBgColor() {#getActiveCellBgColor--}
```
public Color getActiveCellBgColor()
```


Especifica el color de fondo de la celda activa.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveCellColor() {#getActiveCellColor--}
```
public Color getActiveCellColor()
```


Especifica el color de la celda activa.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveHeaderBgColor() {#getActiveHeaderBgColor--}
```
public Color getActiveHeaderBgColor()
```


Especifica el color de fondo del encabezado activo de fila/columna.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveHeaderColor() {#getActiveHeaderColor--}
```
public Color getActiveHeaderColor()
```


Especifica el color del encabezado activo de fila/columna.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveSheet() {#getActiveSheet--}
```
public GridWorksheet getActiveSheet()
```


Obtiene la hoja activa

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet)
### getActiveSheetIndex() {#getActiveSheetIndex--}
```
public int getActiveSheetIndex()
```


Obtiene el índice de la hoja activa. Igual a WebWorksheets.ActiveSheetIndex.

**Returns:**
int
### getActiveTabStyle() {#getActiveTabStyle--}
```
public GridTableItemStyle getActiveTabStyle()
```


Especifica el estilo de la pestaña activa.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getAutoRefreshChart() {#getAutoRefreshChart--}
```
public boolean getAutoRefreshChart()
```


Obtiene si la imagen del Chart se actualiza al actualizar el valor de la celda. El valor predeterminado es true.

**Returns:**
boolean
### getBackColor() {#getBackColor--}
```
public Color getBackColor()
```


Obtiene el BackColor en el WebControl

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderColor() {#getBorderColor--}
```
public Color getBorderColor()
```


Obtiene el BorderColor en el WebControl

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


Obtiene el BorderStyle en el WebControl

Ver [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Returns:**
int
### getBorderWidth() {#getBorderWidth--}
```
public Unit getBorderWidth()
```


Obtiene el BorderWidth en el WebControl

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getBottomTableStyle() {#getBottomTableStyle--}
```
public GridTableStyle getBottomTableStyle()
```


Obtiene el estilo de la barra inferior del control.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCssClass() {#getCssClass--}
```
public String getCssClass()
```


Obtiene el CssClass en el WebControl

**Returns:**
java.lang.String
### getCurrentPageIndex() {#getCurrentPageIndex--}
```
public int getCurrentPageIndex()
```


Obtiene el índice de página actual en modo paginación.

**Remarks**

Cuando está en modo de paginación, el control mostrará PageSize filas de datos una vez, y mostrará el control de selección de página en la barra de pestañas.

**Returns:**
int
### getCustomCalculationEngine() {#getCustomCalculationEngine--}
```
public GridAbstractCalculationEngine getCustomCalculationEngine()
```


Representa el motor de cálculo personalizado del usuario para ampliar el motor de cálculo predeterminado de Aspose.Cells.

**Returns:**
[GridAbstractCalculationEngine](../../com.aspose.gridweb/gridabstractcalculationengine)
### getCustomCommandButtons() {#getCustomCommandButtons--}
```
public CustomCommandButtonCollection getCustomCommandButtons()
```


Obtiene la colección de botones de comando personalizados

**Returns:**
[CustomCommandButtonCollection](../../com.aspose.gridweb/customcommandbuttoncollection)
### getCustomStyleFileName() {#getCustomStyleFileName--}
```
public String getCustomStyleFileName()
```


Obtiene el nombre del archivo de estilo personalizado.

**Remarks**

El archivo de estilo personalizado es un archivo XML. Cuando se establece el nombre del archivo, el archivo se cargará inmediatamente. Aquí está el contenido del "estilo preestablecido estándar" ------------------------------------------------------- <Aspose.Cells.GridWeb.ViewerStyleTemplate runat="server" HeaderBarWidth="30pt" ScrollBarBaseColor="" FrameTableStyle-BorderStyle="Solid" FrameTableStyle-LeftBorderStyle-BorderWidth="" FrameTableStyle-LeftBorderStyle-BorderColor="" FrameTableStyle-RightBorderStyle-BorderWidth="" FrameTableStyle-RightBorderStyle-BorderColor="" FrameTableStyle-BorderWidth="1px" FrameTableStyle-CellSpacing="0" FrameTableStyle-BorderColor="Gray" FrameTableStyle-CellPadding="0" FrameTableStyle-TopBorderStyle-BorderWidth="" FrameTableStyle-TopBorderStyle-BorderColor="" FrameTableStyle-BottomBorderStyle-BorderWidth="" FrameTableStyle-BottomBorderStyle-BorderColor="" HeaderBarStyle-LeftBorderStyle-BorderStyle="Solid" HeaderBarStyle-LeftBorderStyle-BorderWidth="1px" HeaderBarStyle-LeftBorderStyle-BorderColor="White" HeaderBarStyle-VerticalAlign="Middle" HeaderBarStyle-RightBorderStyle-BorderStyle="Solid" HeaderBarStyle-RightBorderStyle-BorderWidth="1px" HeaderBarStyle-RightBorderStyle-BorderColor="Gray" HeaderBarStyle-BorderWidth="1px" HeaderBarStyle-Font-Size="10pt" HeaderBarStyle-BorderColor="Gray" HeaderBarStyle-BorderStyle="Solid" HeaderBarStyle-HorizontalAlign="Center" HeaderBarStyle-ForeColor="Black" HeaderBarStyle-TopBorderStyle-BorderStyle="Solid" HeaderBarStyle-TopBorderStyle-BorderWidth="1px" HeaderBarStyle-TopBorderStyle-BorderColor="White" HeaderBarStyle-BackColor="\#E0E0E0" HeaderBarStyle-BottomBorderStyle-BorderStyle="Solid" HeaderBarStyle-BottomBorderStyle-BorderWidth="1px" HeaderBarStyle-BottomBorderStyle-BorderColor="Gray" ViewTableStyle-LeftBorderStyle-BorderWidth="" ViewTableStyle-LeftBorderStyle-BorderColor="" ViewTableStyle-LayoutFixed="Fixed" ViewTableStyle-RightBorderStyle-BorderWidth="" ViewTableStyle-RightBorderStyle-BorderColor="" ViewTableStyle-BorderWidth="0px" ViewTableStyle-CellSpacing="0" ViewTableStyle-CellPadding="0" ViewTableStyle-TopBorderStyle-BorderWidth="" ViewTableStyle-TopBorderStyle-BorderColor="" ViewTableStyle-BottomBorderStyle-BorderWidth="" ViewTableStyle-BottomBorderStyle-BorderColor="" BottomTableStyle-LeftBorderStyle-BorderWidth="" BottomTableStyle-LeftBorderStyle-BorderColor="" BottomTableStyle-LayoutFixed="Fixed" BottomTableStyle-RightBorderStyle-BorderWidth="" BottomTableStyle-RightBorderStyle-BorderColor="" BottomTableStyle-BorderWidth="0px" BottomTableStyle-CellSpacing="0" BottomTableStyle-CellPadding="1" BottomTableStyle-TopBorderStyle-BorderStyle="Solid" BottomTableStyle-TopBorderStyle-BorderWidth="1px" BottomTableStyle-TopBorderStyle-BorderColor="Gray" BottomTableStyle-BottomBorderStyle-BorderWidth="" BottomTableStyle-BottomBorderStyle-BorderColor="" HeaderBarHeight="15pt" ActiveTabStyle-LeftBorderStyle-BorderWidth="" ActiveTabStyle-LeftBorderStyle-BorderColor="" ActiveTabStyle-RightBorderStyle-BorderWidth="" ActiveTabStyle-RightBorderStyle-BorderColor="" ActiveTabStyle-Height="15pt" ActiveTabStyle-BorderWidth="1px" ActiveTabStyle-Font-Size="10pt" ActiveTabStyle-BorderColor="Gray" ActiveTabStyle-ForeColor="Black" ActiveTabStyle-TopBorderStyle-BorderWidth="" ActiveTabStyle-TopBorderStyle-BorderColor="" ActiveTabStyle-BackColor="White" ActiveTabStyle-BottomBorderStyle-BorderWidth="" ActiveTabStyle-BottomBorderStyle-BorderColor="" HeaderBarTableStyle-LeftBorderStyle-BorderWidth="" HeaderBarTableStyle-LeftBorderStyle-BorderColor="" HeaderBarTableStyle-LayoutFixed="Fixed" HeaderBarTableStyle-RightBorderStyle-BorderWidth="" HeaderBarTableStyle-RightBorderStyle-BorderColor="" HeaderBarTableStyle-BorderWidth="0px" HeaderBarTableStyle-CellSpacing="0" HeaderBarTableStyle-BorderCollapse="Separate" HeaderBarTableStyle-CellPadding="0" HeaderBarTableStyle-TopBorderStyle-BorderWidth="" HeaderBarTableStyle-TopBorderStyle-BorderColor="" HeaderBarTableStyle-BottomBorderStyle-BorderWidth="" HeaderBarTableStyle-BottomBorderStyle-BorderColor="" TabStyle-LeftBorderStyle-BorderWidth="" TabStyle-LeftBorderStyle-BorderColor="" TabStyle-RightBorderStyle-BorderWidth="" TabStyle-RightBorderStyle-BorderColor="" TabStyle-Height="15pt" TabStyle-BorderWidth="1px" TabStyle-Font-Size="10pt" TabStyle-BorderColor="Gray" TabStyle-ForeColor="Black" TabStyle-TopBorderStyle-BorderWidth="" TabStyle-TopBorderStyle-BorderColor="" TabStyle-BackColor="\#E0E0E0" TabStyle-BottomBorderStyle-BorderWidth="" TabStyle-BottomBorderStyle-BorderColor="" ScrollBarArrowColor=""></Aspose.Cells.GridWeb.ViewerStyleTemplate>

**Example**

```
         		GridWeb1.setCustomStyleFileName("c:\\style\\mystyle.xml");
```

**Returns:**
java.lang.String
### getDPI() {#getDPI--}
```
public static double getDPI()
```


Obtiene /Establece los DPI de la máquina.

**Remarks**

**Returns:**
double
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


Obtiene el nombre de fuente predeterminado del control.

**Example**

```
         		GridWeb1.setDefaultFontName("Arial");
```

**Returns:**
java.lang.String
### getDefaultFontSize() {#getDefaultFontSize--}
```
public FontUnit getDefaultFontSize()
```


Obtiene el tamaño de fuente predeterminado del control.

**Example**

```
         		GridWeb1.setDefaultFontSize(new FontUnit("10pt"));
```

**Returns:**
[FontUnit](../../com.aspose.gridweb/fontunit)
### getDefaultGridLineColor() {#getDefaultGridLineColor--}
```
public Color getDefaultGridLineColor()
```


Obtiene el color predeterminado de la línea de la cuadrícula.

**Example**

```
         		GridWeb1.setDefaultGridLineColor(Color.getRed());
```

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getDisplayCellTip() {#getDisplayCellTip--}
```
public boolean getDisplayCellTip()
```


Obtiene si se deben mostrar sugerencias. El valor predeterminado es verdadero.

**Returns:**
boolean
### getEditMode() {#getEditMode--}
```
public boolean getEditMode()
```


Obtiene el modo de edición del control.

**Remarks**

Cuando se establece en true, las celdas del control son editables y se muestran los íconos de "save" y "undo". Cuando se establece en false, las celdas del control son de solo lectura y los íconos de "save" y "undo" no se muestran.

**Returns:**
boolean
### getEnableAJAX() {#getEnableAJAX--}
```
public boolean getEnableAJAX()
```


Obtiene si se debe usar la llamada AJAX. El valor predeterminado es verdadero.

**Returns:**
boolean
### getEnableAsync() {#getEnableAsync--}
```
public boolean getEnableAsync()
```


Obtiene si se cargan los datos de celdas de forma asíncrona, se sugiere aplicarlo para una hoja con más de 10000 celdas.

**Returns:**
boolean
### getEnableClientColumnOperations() {#getEnableClientColumnOperations--}
```
public boolean getEnableClientColumnOperations()
```


Obtiene si se habilitan las operaciones de columna del lado del cliente.

**Remarks**

Cuando se establece en true, el usuario puede usar el menú contextual para agregar/quitar columnas.

**Returns:**
boolean
### getEnableClientFreeze() {#getEnableClientFreeze--}
```
public boolean getEnableClientFreeze()
```


Obtiene si se habilitan las operaciones de congelación del lado del cliente.

**Remarks**

Cuando se establece en true, el usuario puede usar el menú contextual para congelar/descongelar paneles.

**Returns:**
boolean
### getEnableClientMergeOperations() {#getEnableClientMergeOperations--}
```
public boolean getEnableClientMergeOperations()
```


Obtiene si se habilitan las operaciones de combinación del lado del cliente.

**Remarks**

Cuando se establece en true, el usuario puede usar el menú contextual para combinar/separar celdas.

**Returns:**
boolean
### getEnableClientResizeColumnRow() {#getEnableClientResizeColumnRow--}
```
public boolean getEnableClientResizeColumnRow()
```


Obtiene si se habilita el redimensionamiento de columnas y filas del lado del cliente.

**Remarks**

Cuando se establece en true, el usuario puede cambiar el tamaño de la columna y la fila del lado del cliente.

**Returns:**
boolean
### getEnableClientRowOperations() {#getEnableClientRowOperations--}
```
public boolean getEnableClientRowOperations()
```


Obtiene si se habilitan las operaciones de fila del lado del cliente.

**Remarks**

Cuando se establece en true, el usuario puede usar el menú contextual para agregar/quitar filas.

**Returns:**
boolean
### getEnableDoubleClickEvent() {#getEnableDoubleClickEvent--}
```
public boolean getEnableDoubleClickEvent()
```


Obtiene si se habilita el evento de doble clic del lado del cliente.

**Remarks**

Cuando se establece en true, el control recibirá eventos de doble clic del lado del cliente y podrá manejar estos eventos en el lado del servidor. De lo contrario, el control ignorará cualquier evento de doble clic.

**Returns:**
boolean
### getEnableMetalLightEffect() {#getEnableMetalLightEffect--}
```
public boolean getEnableMetalLightEffect()
```


Obtiene si se aplica el efecto de luz metálica.

**Returns:**
boolean
### getEnablePaging() {#getEnablePaging--}
```
public boolean getEnablePaging()
```


Obtiene si se habilita el modo de paginación del control.

**Remarks**

Cuando se establece en true, el control mostrará PageSize filas de datos de una vez y mostrará el control de selección de página en la barra de pestañas.

**Returns:**
boolean
### getEnableStyleDialogbox() {#getEnableStyleDialogbox--}
```
public boolean getEnableStyleDialogbox()
```


Obtiene si se habilita el cuadro de diálogo de estilo del lado del cliente.

**Remarks**

Cuando se establece en true, el usuario puede usar el cuadro de diálogo de estilo para establecer el estilo de una celda seleccionando "Format Cell..." del menú emergente.

**Returns:**
boolean
### getEnabled() {#getEnabled--}
```
public boolean getEnabled()
```


Obtiene el Enabled en el WebControl

**Returns:**
boolean
### getFilteredPaging() {#getFilteredPaging--}
```
public boolean getFilteredPaging()
```


Obtiene si se habilita la paginación después de filtrar los datos, tendrá efecto cuando EnablePaging sea verdadero.

**Remarks**

Cuando se establece en true, el control paginará basándose en los datos filtrados; el valor predeterminado es false.

**Returns:**
boolean
### getFont() {#getFont--}
```
public FontInfo getFont()
```


Obtiene el Font en el WebControl

**Returns:**
[FontInfo](../../com.aspose.gridweb/fontinfo)
### getForceValidation() {#getForceValidation--}
```
public boolean getForceValidation()
```


Obtiene si se fuerza la validación del lado del cliente.

**Remarks**

Cuando se establece en true, los datos no se enviarán al servidor hasta que todos los campos de entrada sean válidos.

**Returns:**
boolean
### getForeColor() {#getForeColor--}
```
public Color getForeColor()
```


Obtiene el ForeColor en el WebControl

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getFrameTableStyle() {#getFrameTableStyle--}
```
public GridTableStyle getFrameTableStyle()
```


Obtiene el estilo del marco del control.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getGoonDefaultSaveOperation() {#getGoonDefaultSaveOperation--}
```
public boolean getGoonDefaultSaveOperation()
```


Obtiene si GridWeb realizará la operación de guardado predeterminada, el valor predeterminado es verdadero.

**Returns:**
boolean
### getHeaderBarHeight() {#getHeaderBarHeight--}
```
public Unit getHeaderBarHeight()
```


Obtiene la altura (System.Web.UI.WebControl.Unit) de la barra de encabezado superior del control.

**Example**

```
         		GridWeb1.setHeaderBarWidth(new Unit(32, com.aspose.gridweb.UnitType.Point));
         		GridWeb1.setHeaderBarHeight(new Unit(24, com.aspose.gridweb.UnitType.Point));
```

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getHeaderBarStyle() {#getHeaderBarStyle--}
```
public GridTableItemStyle getHeaderBarStyle()
```


Obtiene el estilo de la barra de encabezado.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getHeaderBarTableStyle() {#getHeaderBarTableStyle--}
```
public GridTableStyle getHeaderBarTableStyle()
```


Obtiene el estilo de la barra de encabezado del control.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getHeaderBarWidth() {#getHeaderBarWidth--}
```
public Unit getHeaderBarWidth()
```


Obtiene el ancho( System.Web.UI.WebControl.Unit ) o la barra de encabezado izquierda del control.

**Example**

```
         		GridWeb1.setHeaderBarWidth(new Unit(32, com.aspose.gridweb.UnitType.Point));
         		GridWeb1.setHeaderBarHeight(new Unit(24, com.aspose.gridweb.UnitType.Point));
```

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getHeight() {#getHeight--}
```
public Unit getHeight()
```


Obtiene la altura( System.Web.UI.WebControl.Unit ) del control.

**Example**

```
         		GridWeb1.setWidth(new Unit(320, com.aspose.gridweb.UnitType.Point));
         		GridWeb1.setHeight(new Unit(240, com.aspose.gridweb.UnitType.Point));
```

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getIgnoreStyleWithNoData() {#getIgnoreStyleWithNoData--}
```
public boolean getIgnoreStyleWithNoData()
```


Obtiene si GridWeb ignora la visualización de filas o columnas que no contienen valores de celda pero que aún tienen estilo. Si se establece en true, el rendimiento será mejor. El valor predeterminado es false, lo que significa que si la última fila/columna consecutiva no tiene valores de celda pero tiene estilo, aún se mostrará. Esta opción solo es válida cuando EnableAsync es false. Esta opción no tiene efecto cuando EnableAsync es true, lo que significa que GridWeb mostrará todas las filas/columnas con estilo.

**Returns:**
boolean
### getLoadOptions() {#getLoadOptions--}
```
public GridLoadOptions getLoadOptions()
```


Representa las opciones de carga para GridWeb.

**Returns:**
[GridLoadOptions](../../com.aspose.gridweb/gridloadoptions)
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Obtiene el índice máximo de columna visible (basado en cero) de la hoja web. El control usa el valor mayor entre MaxColumn y la columna máxima de los datos de la hoja.

**Example**

```
         		// Creates a 4x4 "display window".
         		GridWeb1.setMinRow(2);
         		GridWeb1.setMaxRow(5);
         		GridWeb1.setMinColumn(3);
         		GridWeb1.setMaxColumn(6);
```

**Returns:**
int
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


Obtiene el índice máximo de fila visible (basado en cero) de la hoja web. El control usa el valor mayor entre MaxRow y la fila máxima de los datos de la hoja.

**Example**

```
         		// Creates a 4x4 "display window".
         		GridWeb1.setMinRow(2);
         		GridWeb1.setMaxRow(5);
         		GridWeb1.setMinColumn(3);
         		GridWeb1.setMaxColumn(6);
```

**Returns:**
int
### getMessage() {#getMessage--}
```
public String getMessage()
```


Obtiene el mensaje para la cuadrícula.

**Returns:**
java.lang.String
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```


Obtiene el índice mínimo de columna visible (basado en cero) de la hoja web. El control usa el valor menor entre MinColumn y la columna mínima de los datos de la hoja.

**Example**

```
         		// Creates a 4x4 "display window".
         		GridWeb1.setMinRow(2);
         		GridWeb1.setMaxRow(5);
         		GridWeb1.setMinColumn(3);
         		GridWeb1.setMaxColumn(6);
```

**Returns:**
int
### getMinRow() {#getMinRow--}
```
public int getMinRow()
```


Obtiene el índice mínimo de fila visible (basado en cero) de la hoja web. El control usa el valor menor entre MinRow y la fila mínima de los datos de la hoja.

**Example**

```
         		// Creates a 4x4 "display window".
         		GridWeb1.setMinRow(2);
         		GridWeb1.setMaxRow(5);
         		GridWeb1.setMinColumn(3);
         		GridWeb1.setMaxColumn(6);
```

**Returns:**
int
### getModifiedCells() {#getModifiedCells--}
```
public ArrayList getModifiedCells()
```


Obtiene la colección de celdas modificadas por el cliente.

**Returns:**
java.util.ArrayList
### getNeedRenderGroupRows() {#getNeedRenderGroupRows--}
```
public boolean getNeedRenderGroupRows()
```


Obtiene si se deben mostrar filas de grupo.

**Returns:**
boolean
### getNoHScroll() {#getNoHScroll--}
```
public boolean getNoHScroll()
```


Obtiene un valor que indica si la barra de desplazamiento horizontal está oculta.

**Returns:**
boolean
### getNoScroll() {#getNoScroll--}
```
public boolean getNoScroll()
```


Obtiene si se debe mostrar la barra de desplazamiento.

**Returns:**
boolean
### getNoVScroll() {#getNoVScroll--}
```
public boolean getNoVScroll()
```


Obtiene un valor que indica si la barra de desplazamiento vertical está oculta.

**Returns:**
boolean
### getOnAjaxCallFinishedClientFunction() {#getOnAjaxCallFinishedClientFunction--}
```
public String getOnAjaxCallFinishedClientFunction()
```


Obtiene el nombre de la función del lado del cliente que se llamará cuando ajaxcall finalice. La función del cliente debe declararse así:
function GridAjaxcallFinished()
\\{
alert(this.id+\" ajaxcall finished \");
\\}

Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento.

**Returns:**
java.lang.String
### getOnCellErrorClientFunction() {#getOnCellErrorClientFunction--}
```
public String getOnCellErrorClientFunction()
```


Obtiene el nombre de la función del lado del cliente que se llamará cuando falle la validación de una celda. La función del cliente debe declararse así:
function MyOnCellError(cell)
\\{
alert(this.getCellValueByCell(cell));
\\}

Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento.

**Returns:**
java.lang.String
### getOnCellSelectedAjaxCallBackClientFunction() {#getOnCellSelectedAjaxCallBackClientFunction--}
```
public String getOnCellSelectedAjaxCallBackClientFunction()
```


Obtiene la función del lado del cliente que se llamará cuando se seleccione una celda. La función del cliente debe declararse así:
function MyOnSelectCellAjaxCallBack(cell,customerdata)
\\{

\\}

Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento.

**Returns:**
java.lang.String
### getOnCellSelectedClientFunction() {#getOnCellSelectedClientFunction--}
```
public String getOnCellSelectedClientFunction()
```


Obtiene la función del lado del cliente que se llamará cuando se seleccione una celda. La función del cliente debe declararse así:
function MyOnSelectCell(cell)
\\{
GridWeb1.setCellValueByCell(cell, "test");
\\}

Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento.

**Returns:**
java.lang.String
### getOnCellUnselectedClientFunction() {#getOnCellUnselectedClientFunction--}
```
public String getOnCellUnselectedClientFunction()
```


Obtiene la función del lado del cliente que se llamará cuando se deseleccione una celda. La función del cliente debe declararse así:
function MyOnUnselectCell(cell)
\\{
this.setCellValueByCell(cell, "test");
\\}

Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento.

**Returns:**
java.lang.String
### getOnCellUpdatedClientFunction() {#getOnCellUpdatedClientFunction--}
```
public String getOnCellUpdatedClientFunction()
```


Obtiene el nombre de la función del lado del cliente que se llamará cuando se actualice el valor de una celda. La función del cliente debe declararse así:
function MyOnCellUpdated(cell)
\\{
alert(this.getCellValueByCell(cell));
\\}

Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento.

**Returns:**
java.lang.String
### getOnContextMenuShowClientFunction() {#getOnContextMenuShowClientFunction--}
```
public String getOnContextMenuShowClientFunction()
```


Obtiene la función del lado del cliente que se llamará cuando se muestre el menú contextual. La función del cliente debe declararse así:
function onContextMenuShow()
\\{
var menu = event.srcElement;
menu.setItemVisibility("Delete", "block");
menu.setItemVisibility("Update", "none");
\\}

Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento.

**Returns:**
java.lang.String
### getOnDoubleClickCellClientFunction() {#getOnDoubleClickCellClientFunction--}
```
public String getOnDoubleClickCellClientFunction()
```


Obtiene la función del lado del cliente que se llamará cuando se haga doble clic en una celda. La función del cliente debe declararse así:
function MyOnDoubleClickCell(cell)
\\{
this.setCellValueByCell(cell, "test");
\\}

Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento.

**Returns:**
java.lang.String
### getOnDoubleClickRowClientFunction() {#getOnDoubleClickRowClientFunction--}
```
public String getOnDoubleClickRowClientFunction()
```


Obtiene la función del lado del cliente que se llamará cuando se haga doble clic en una fila. La función del cliente debe declararse así:
function MyOnRowDoubleClick(row)
\\{
alert(row);
\\}

Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento.

**Returns:**
java.lang.String
### getOnGridInitClientFunction() {#getOnGridInitClientFunction--}
```
public String getOnGridInitClientFunction()
```


Obtiene el nombre de la función del lado del cliente que se llamará cuando se inicialice la cuadrícula. La función del cliente debe declararse así:
function MyOnGridInit(grid)
\\{
alert("The grid is initialized: " + grid.id);
\\}

Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento.

**Returns:**
java.lang.String
### getOnPageChangeClientFunction() {#getOnPageChangeClientFunction--}
```
public String getOnPageChangeClientFunction()
```


Obtiene la función del lado del cliente que se llamará después de cambiar el índice de página. Solo tiene efecto cuando EnablePaging es verdadero. La función del cliente debe declararse así:
function MyOnPageChange(index)
\\{
console.log("current page is:"+index);
\\}

Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento.

**Returns:**
java.lang.String
### getOnPageSubmitClientFunction() {#getOnPageSubmitClientFunction--}
```
public String getOnPageSubmitClientFunction()
```


Obtiene la función del cliente que se llamará antes de que la página se envíe del lado del cliente.

**Returns:**
java.lang.String
### getOnShapeSelectedClientFunction() {#getOnShapeSelectedClientFunction--}
```
public String getOnShapeSelectedClientFunction()
```


Obtiene la función del lado del cliente que se llamará cuando se seleccione una forma. La función del cliente debe declararse así:
function MyOnSelectShape(shape)
\\{
var name=shape.getAttribute("namevalue")
var text=shape.getAttribute("textvalue")
var value=shape.getAttribute("controlvalue")
var type=shape.getAttribute("msotype")
\\}

Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento.

**Returns:**
java.lang.String
### getOnSubmitClientFunction() {#getOnSubmitClientFunction--}
```
public String getOnSubmitClientFunction()
```


Obtiene la función del cliente que se llamará antes de que el control se envíe del lado del cliente. La función del cliente debe declararse así:
function MyOnSubmit(arg, cancelEdit)
\\{
return true;
\\}
El argumento arg es el argumento de envío, contiene el comando que se enviará al servidor. cancelEdit es un valor booleano que indica si el control ha descartado la entrada del usuario antes de enviar. El control continuará enviando si la función devuelve true.
Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento.

**Returns:**
java.lang.String
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```


Obtiene si solo se ajustan las filas cuya altura no está personalizada, el valor predeterminado es false

**Returns:**
boolean
### getPageSize() {#getPageSize--}
```
public int getPageSize()
```


Obtiene el tamaño de página en modo de paginación.

**Remarks**

Cuando está en modo de paginación, el control mostrará PageSize filas de datos una vez, y mostrará el control de selección de página en la barra de pestañas.

**Returns:**
int
### getPictureCachePath() {#getPictureCachePath--}
```
public static String getPictureCachePath()
```


Obtiene la ruta de almacenamiento de imágenes para el libro de trabajo, todas las formas e imágenes se almacenarán en este directorio, la ruta predeterminada es acwcache bajo el Directorio Base de la aplicación actual; los usuarios deben implementar un servicio programado para limpiar los archivos que estén fuera del tiempo de sesión.

**Returns:**
java.lang.String
### getPresetStyle() {#getPresetStyle--}
```
public int getPresetStyle()
```


Obtiene el estilo predefinido.

Ver [PresetStyle](../../com.aspose.gridweb/presetstyle).

**Example**

```
         		GridWeb1.setPresetStyle(PresetStyle.TRADITIONAL_1);
```

**Returns:**
int
### getRefreshValidation() {#getRefreshValidation--}
```
public boolean getRefreshValidation()
```


Obtiene si se debe actualizar el valor de validación después de que cambie el valor de la celda.

**Returns:**
boolean
### getRenderHiddenRow() {#getRenderHiddenRow--}
```
public boolean getRenderHiddenRow()
```


Obtiene si la fila oculta se renderiza en GridControl, el valor predeterminado es false. Si necesita volver a mostrar la fila oculta más tarde, debe establecerlo en true.

**Returns:**
boolean
### getRowHeightForCSV() {#getRowHeightForCSV--}
```
public double getRowHeightForCSV()
```


Obtiene el valor de la altura de fila en puntos para el archivo csv, el valor predeterminado es 14.5.

**Returns:**
double
### getScrollBarArrowColor() {#getScrollBarArrowColor--}
```
public Color getScrollBarArrowColor()
```


Especifica el color del botón de flecha de la barra de desplazamiento.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getScrollBarBaseColor() {#getScrollBarBaseColor--}
```
public Color getScrollBarBaseColor()
```


Especifica el color de la barra de desplazamiento del control.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSelectCellBgColor() {#getSelectCellBgColor--}
```
public Color getSelectCellBgColor()
```


Especifica el color de fondo de las celdas seleccionadas en un rango de selección múltiple.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSelectCellColor() {#getSelectCellColor--}
```
public Color getSelectCellColor()
```


Especifica el color de las celdas seleccionadas en un rango de selección múltiple.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSelectCells() {#getSelectCells--}
```
public ArrayList getSelectCells()
```


Obtiene la colección de celdas seleccionadas.

**Returns:**
java.util.ArrayList
### getSessionStorePath() {#getSessionStorePath--}
```
public String getSessionStorePath()
```


Obtiene la ruta de almacenamiento de caché de sesión cuando el modo de sesión es File o ViewState, etc.: gridweb.SessionStorePath="c:/mytempdir/session"; luego almacenará los datos de sesión en c:/mytempdir/session

**Returns:**
java.lang.String
### getSettings() {#getSettings--}
```
public GridWorkbookSettings getSettings()
```


Representa la configuración del libro de trabajo.

**Returns:**
[GridWorkbookSettings](../../com.aspose.gridweb/gridworkbooksettings)
### getShowAddButton() {#getShowAddButton--}
```
public boolean getShowAddButton()
```


Obtiene si se muestra el botón de agregar hoja de cálculo.

**Returns:**
boolean
### getShowBottomBar() {#getShowBottomBar--}
```
public boolean getShowBottomBar()
```


Especifica si se muestra la barra de comandos (incluye barra de comandos y barra de pestañas) en la parte inferior del control.

**Returns:**
boolean
### getShowCellEditBox() {#getShowCellEditBox--}
```
public boolean getShowCellEditBox()
```


Indica si Gridweb muestra la barra de herramientas del cuadro de edición como en MS-EXCEL. Si está habilitado, un cuadro de edición para la celda actual se mostrará en Gridweb. Si habilitamos esta función, debemos importar la biblioteca jquery js en sus archivos aspx para soportar esta nueva característica. Cualquier versión reciente de jquery está bien, etc.

**Returns:**
boolean
### getShowCommandBarAtTop() {#getShowCommandBarAtTop--}
```
public boolean getShowCommandBarAtTop()
```


Especifica si se muestra la barra de comandos (incluye barra de comandos y barra de pestañas) en la parte superior del control.

**Returns:**
boolean
### getShowContextMenu() {#getShowContextMenu--}
```
public boolean getShowContextMenu()
```


Obtiene si se muestra el menú contextual. El valor predeterminado es true.

**Returns:**
boolean
### getShowDefaultGridLine() {#getShowDefaultGridLine--}
```
public boolean getShowDefaultGridLine()
```


Obtiene si se muestran las líneas de cuadrícula predeterminadas de las celdas.

**Returns:**
boolean
### getShowHeaderBar() {#getShowHeaderBar--}
```
public boolean getShowHeaderBar()
```


Obtiene si se muestra la barra de encabezado

**Returns:**
boolean
### getShowLoading() {#getShowLoading--}
```
public boolean getShowLoading()
```


Especifica si se muestra un cuadro de diálogo de carga mientras se envía la solicitud al servidor.

**Returns:**
boolean
### getShowLoadingPosition() {#getShowLoadingPosition--}
```
public String getShowLoadingPosition()
```


Especifica la posición izquierda y superior (en px) para mostrar el cuadro de diálogo de carga mientras se envía la solicitud al servidor, etc. 100,200 significa que la posición izquierda y superior del cuadro de diálogo de carga está en 100px,200px.

**Returns:**
java.lang.String
### getShowSaveButton() {#getShowSaveButton--}
```
public boolean getShowSaveButton()
```


Obtiene si se muestra el botón de guardar.

**Returns:**
boolean
### getShowSubmitButton() {#getShowSubmitButton--}
```
public boolean getShowSubmitButton()
```


Obtiene si se muestra el botón de envío.

**Returns:**
boolean
### getShowTabBar() {#getShowTabBar--}
```
public boolean getShowTabBar()
```


Obtiene si se muestra la barra de pestañas.

**Returns:**
boolean
### getShowTabNavigation() {#getShowTabNavigation--}
```
public boolean getShowTabNavigation()
```


Obtiene si el botón de navegación de pestañas se muestra, el valor predeterminado es true.

**Returns:**
boolean
### getShowUndoButton() {#getShowUndoButton--}
```
public boolean getShowUndoButton()
```


Obtiene si se muestra el botón deshacer.

**Returns:**
boolean
### getSpanWrap() {#getSpanWrap--}
```
public boolean getSpanWrap()
```


Especifica si se envuelve el contenido en el cell span, el valor predeterminado es true.

**Returns:**
boolean
### getTabIndex() {#getTabIndex--}
```
public short getTabIndex()
```


Obtiene el TabIndex en el WebControl

**Returns:**
short
### getTabStyle() {#getTabStyle--}
```
public GridTableItemStyle getTabStyle()
```


Obtiene el estilo de la barra de pestañas.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getToolTip() {#getToolTip--}
```
public String getToolTip()
```


Obtiene el ToolTip en el WebControl

**Returns:**
java.lang.String
### getUseClientPageHeight() {#getUseClientPageHeight--}
```
public boolean getUseClientPageHeight()
```


Obtiene si gridweb usa la altura de la página del cliente como altura del control, adecuado para cuando se establece Height="100%", el valor predeterminado es false.

**Returns:**
boolean
### getVersion() {#getVersion--}
```
public static String getVersion()
```


Obtiene la versión de lanzamiento.

**Returns:**
java.lang.String - La versión de lanzamiento.
### getViewPanelScrollLeft() {#getViewPanelScrollLeft--}
```
public String getViewPanelScrollLeft()
```


Obtiene la posición de la barra de desplazamiento del panel de vista de la cuadrícula.

**Returns:**
java.lang.String
### getViewPanelScrollTop() {#getViewPanelScrollTop--}
```
public String getViewPanelScrollTop()
```


Obtiene la posición de la barra de desplazamiento del panel de vista de la cuadrícula.

**Returns:**
java.lang.String
### getViewTableStyle() {#getViewTableStyle--}
```
public GridTableStyle getViewTableStyle()
```


Obtiene el estilo del panel de vista de datos.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


Obtiene el ancho (System.Web.UI.WebControl.Unit) del control.

**Example**

```
         		GridWeb1.setWidth(new Unit(320, com.aspose.gridweb.UnitType.Point));
         		GridWeb1.setHeight(new Unit(240, com.aspose.gridweb.UnitType.Point));
```

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getWorkSheets() {#getWorkSheets--}
```
public GridWorksheetCollection getWorkSheets()
```


Obtiene la colección de las hojas de cálculo.

**Returns:**
[GridWorksheetCollection](../../com.aspose.gridweb/gridworksheetcollection)
### getXhtmlMode() {#getXhtmlMode--}
```
public boolean getXhtmlMode()
```


Obtiene si se usa el estilo XHTML, el valor predeterminado es true.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### importExcelFile(InputStream stream) {#importExcelFile-java.io.InputStream-}
```
public void importExcelFile(InputStream stream)
```


Importa desde un flujo de archivo Excel, incluyendo flujo de archivo en disco o flujo de memoria.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.InputStream | El flujo del archivo Excel, incluyendo el flujo de archivo en disco o el flujo de memoria. |

### importExcelFile(InputStream stream, String passwordtoOpen) {#importExcelFile-java.io.InputStream-java.lang.String-}
```
public void importExcelFile(InputStream stream, String passwordtoOpen)
```


Importa desde un flujo de archivo Excel, incluyendo flujo de archivo en disco o flujo de memoria.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.InputStream | El flujo del archivo Excel, incluyendo el flujo de archivo en disco o el flujo de memoria. |
| passwordtoOpen | java.lang.String | la contraseña de apertura para el archivo que está encriptado. |

### importExcelFile(String fileName) {#importExcelFile-java.lang.String-}
```
public void importExcelFile(String fileName)
```


Importa desde un archivo Excel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | java.lang.String | El nombre del archivo Excel. |

### importExcelFile(String fileName, String passwordtoOpen) {#importExcelFile-java.lang.String-java.lang.String-}
```
public void importExcelFile(String fileName, String passwordtoOpen)
```


Importa desde un archivo Excel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | java.lang.String | El nombre del archivo Excel. |
| passwordtoOpen | java.lang.String | la contraseña de apertura para el archivo que está encriptado. |

### isCalculateFormula() {#isCalculateFormula--}
```
public boolean isCalculateFormula()
```


Obtiene si se debe calcular la fórmula después de que cambie el valor de la celda o después de importar el archivo. El valor predeterminado es true.

**Returns:**
boolean
### loadCSVFile(InputStream stream) {#loadCSVFile-java.io.InputStream-}
```
public void loadCSVFile(InputStream stream)
```


Carga datos desde un flujo de archivo CSV.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.InputStream | El flujo de archivo. |

### loadCSVFile(String fileName) {#loadCSVFile-java.lang.String-}
```
public void loadCSVFile(String fileName)
```


Carga datos desde un archivo CSV.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | java.lang.String | El nombre del archivo. |

### loadHTMLFile(InputStream stream) {#loadHTMLFile-java.io.InputStream-}
```
public void loadHTMLFile(InputStream stream)
```


Carga datos desde un flujo de archivo HTML.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.InputStream | El flujo de archivo. |

### loadHTMLFile(String fileName) {#loadHTMLFile-java.lang.String-}
```
public void loadHTMLFile(String fileName)
```


Carga datos desde un archivo HTML.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | java.lang.String | El nombre del archivo. |

### loadSpreadSheetMLFile(InputStream stream) {#loadSpreadSheetMLFile-java.io.InputStream-}
```
public void loadSpreadSheetMLFile(InputStream stream)
```


Carga datos desde un flujo de archivo SpreadSheetML.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.InputStream | El flujo del archivo. |

### loadSpreadSheetMLFile(String fileName) {#loadSpreadSheetMLFile-java.lang.String-}
```
public void loadSpreadSheetMLFile(String fileName)
```


Carga datos desde un archivo SpreadSheetML.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | java.lang.String | El nombre del archivo. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshChartShape() {#refreshChartShape--}
```
public void refreshChartShape()
```


Actualiza todas las imágenes de gráficos para la hoja de cálculo activa.

### saveCSVFile(OutputStream stream) {#saveCSVFile-java.io.OutputStream-}
```
public void saveCSVFile(OutputStream stream)
```


Guarda datos en un flujo de archivo CSV.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.OutputStream | El flujo de archivo. |

### saveCSVFile(String targetFile) {#saveCSVFile-java.lang.String-}
```
public void saveCSVFile(String targetFile)
```


Guarda datos en un archivo CSV.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| targetFile | java.lang.String | El nombre del archivo. |

### saveCustomStyleFile(String fileName) {#saveCustomStyleFile-java.lang.String-}
```
public void saveCustomStyleFile(String fileName)
```


Guarda los datos de estilo actuales del control en un archivo xml. Puede usarse para crear su archivo de estilo personalizado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | java.lang.String | El nombre del archivo de estilo. |

### saveHTMLFile(OutputStream stream) {#saveHTMLFile-java.io.OutputStream-}
```
public void saveHTMLFile(OutputStream stream)
```


Guarda datos en un flujo de archivo HTML.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.OutputStream | El flujo de archivo. |

### saveHTMLFile(String targetFile) {#saveHTMLFile-java.lang.String-}
```
public void saveHTMLFile(String targetFile)
```


Guarda datos en un archivo HTML.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| targetFile | java.lang.String | El nombre del archivo. |

### saveSpreadSheetMLFile(OutputStream stream) {#saveSpreadSheetMLFile-java.io.OutputStream-}
```
public void saveSpreadSheetMLFile(OutputStream stream)
```


Guarda datos en un flujo de archivo SpreadSheetML.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.OutputStream | El flujo de archivo. |

### saveSpreadSheetMLFile(String targetFile) {#saveSpreadSheetMLFile-java.lang.String-}
```
public void saveSpreadSheetMLFile(String targetFile)
```


Guarda datos en un archivo SpreadSheetML.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| targetFile | java.lang.String | El nombre del archivo. |

### saveToExcelFile(OutputStream stream) {#saveToExcelFile-java.io.OutputStream-}
```
public void saveToExcelFile(OutputStream stream)
```


Guarda las hojas de cálculo en un archivo excel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.OutputStream | El flujo al que escribir. |

### saveToExcelFile(OutputStream stream, GridSaveOptions saveOptions) {#saveToExcelFile-java.io.OutputStream-com.aspose.gridweb.GridSaveOptions-}
```
public void saveToExcelFile(OutputStream stream, GridSaveOptions saveOptions)
```


Guarda las hojas de cálculo en un archivo excel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.OutputStream | El flujo al que escribir. |
| saveOptions | [GridSaveOptions](../../com.aspose.gridweb/gridsaveoptions) | Las opciones de guardado. |

### saveToExcelFile(OutputStream stream, int format) {#saveToExcelFile-java.io.OutputStream-int-}
```
public void saveToExcelFile(OutputStream stream, int format)
```


Guarda las hojas de cálculo en un archivo excel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.OutputStream | El flujo al que escribir. |
| format | int | [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat). El formato de archivo (Excel2003, Excel2007, CSV, SpreadsheetML) |

### saveToExcelFile(String targetFile) {#saveToExcelFile-java.lang.String-}
```
public void saveToExcelFile(String targetFile)
```


Guarda las hojas de cálculo en un archivo excel con formato Excel 2003.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| targetFile | java.lang.String | El nombre del archivo de destino al que escribir. |

### saveToExcelFile(String targetFile, GridSaveOptions saveOptions) {#saveToExcelFile-java.lang.String-com.aspose.gridweb.GridSaveOptions-}
```
public void saveToExcelFile(String targetFile, GridSaveOptions saveOptions)
```


Guarda las hojas de cálculo en un archivo excel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| targetFile | java.lang.String | El nombre del archivo de destino al que escribir. |
| saveOptions | [GridSaveOptions](../../com.aspose.gridweb/gridsaveoptions) | Las opciones de guardado. |

### saveToExcelFile(String targetFile, int format) {#saveToExcelFile-java.lang.String-int-}
```
public void saveToExcelFile(String targetFile, int format)
```


Guarda las hojas de cálculo en un archivo excel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| targetFile | java.lang.String | El nombre del archivo de destino al que escribir. |
| format | int | [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat). El formato de archivo (Excel2003, Excel2007, CSV, SpreadsheetML) |

### setACWClientPath(String value) {#setACWClientPath-java.lang.String-}
```
public void setACWClientPath(String value)
```


Establece la ruta web de los archivos de script/imagen del control. Por ejemplo: "http://localhost/acw\_client". También puede establecer este valor en el archivo web.config. Añada esta sección a la sección `<configuration>`:
`<appSettings>`
`<add key=\"aspose.cells.gridweb.acw_client_path\" value=\"/acw_client/\" />`
`</appSettings>`


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setACWLanguageFileUrl(String value) {#setACWLanguageFileUrl-java.lang.String-}
```
public void setACWLanguageFileUrl(String value)
```


Establece la URL web del archivo de idioma del control. Por ejemplo: "/acw\_client/lang\_en.js".
Por defecto, se utiliza un archivo inglés incorporado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setActiveCell(GridCell value) {#setActiveCell-com.aspose.gridweb.GridCell-}
```
public void setActiveCell(GridCell value)
```


Establece la celda activa de la hoja actual. Cambiado para ser editable desde la versión 1.9.0.1.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [GridCell](../../com.aspose.gridweb/gridcell) |  |

### setActiveCellBgColor(Color value) {#setActiveCellBgColor-com.aspose.gridweb.Color-}
```
public void setActiveCellBgColor(Color value)
```


Especifica el color de fondo de la celda activa.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveCellColor(Color value) {#setActiveCellColor-com.aspose.gridweb.Color-}
```
public void setActiveCellColor(Color value)
```


Especifica el color de la celda activa.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveHeaderBgColor(Color value) {#setActiveHeaderBgColor-com.aspose.gridweb.Color-}
```
public void setActiveHeaderBgColor(Color value)
```


Especifica el color de fondo del encabezado activo de fila/columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveHeaderColor(Color value) {#setActiveHeaderColor-com.aspose.gridweb.Color-}
```
public void setActiveHeaderColor(Color value)
```


Especifica el color del encabezado activo de fila/columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveSheetIndex(int value) {#setActiveSheetIndex-int-}
```
public void setActiveSheetIndex(int value)
```


Establece el índice de la hoja activa. Igual a WebWorksheets.ActiveSheetIndex.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setActiveTabStyle(GridTableItemStyle value) {#setActiveTabStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setActiveTabStyle(GridTableItemStyle value)
```


Especifica el estilo de la pestaña activa.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setAutoRefreshChart(boolean value) {#setAutoRefreshChart-boolean-}
```
public void setAutoRefreshChart(boolean value)
```


Establece si la imagen Chart se actualiza al actualizar el valor de la celda. el valor predeterminado es true

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setBackColor(Color value) {#setBackColor-com.aspose.gridweb.Color-}
```
public void setBackColor(Color value)
```


Establece el BackColor en el WebControl

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderColor(Color value) {#setBorderColor-com.aspose.gridweb.Color-}
```
public void setBorderColor(Color value)
```


Establece el BorderColor en el WebControl

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


Establece el BorderStyle en el WebControl

Ver [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setBorderWidth(Unit value) {#setBorderWidth-com.aspose.gridweb.Unit-}
```
public void setBorderWidth(Unit value)
```


Establece el BorderWidth en el WebControl

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setBottomTableStyle(GridTableStyle value) {#setBottomTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setBottomTableStyle(GridTableStyle value)
```


Establece el estilo de la barra inferior del control.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


Establece si se debe calcular la fórmula después de que cambie el valor de la celda o después de importar el archivo. El valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCssClass(String value) {#setCssClass-java.lang.String-}
```
public void setCssClass(String value)
```


Establece el CssClass en el WebControl

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setCurrentPageIndex(int value) {#setCurrentPageIndex-int-}
```
public void setCurrentPageIndex(int value)
```


Establece el índice de página actual en modo paginación.

**Remarks**

Cuando está en modo de paginación, el control mostrará PageSize filas de datos una vez, y mostrará el control de selección de página en la barra de pestañas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setCustomCalculationEngine(GridAbstractCalculationEngine value) {#setCustomCalculationEngine-com.aspose.gridweb.GridAbstractCalculationEngine-}
```
public void setCustomCalculationEngine(GridAbstractCalculationEngine value)
```


Representa el motor de cálculo personalizado del usuario para ampliar el motor de cálculo predeterminado de Aspose.Cells.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [GridAbstractCalculationEngine](../../com.aspose.gridweb/gridabstractcalculationengine) |  |

### setCustomStyle(InputStream stream) {#setCustomStyle-java.io.InputStream-}
```
public void setCustomStyle(InputStream stream)
```


establece el archivo de estilo personalizado desde un flujo, incluyendo flujo de archivo en disco o flujo de memoria.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.InputStream | El flujo del archivo, incluyendo flujo de archivo en disco o flujo de memoria. |

### setCustomStyleFileName(String value) {#setCustomStyleFileName-java.lang.String-}
```
public void setCustomStyleFileName(String value)
```


Establece el nombre del archivo de estilo personalizado.

**Remarks**

El archivo de estilo personalizado es un archivo XML. Cuando se establece el nombre del archivo, el archivo se cargará inmediatamente. Aquí está el contenido del "estilo preestablecido estándar" ------------------------------------------------------- <Aspose.Cells.GridWeb.ViewerStyleTemplate runat="server" HeaderBarWidth="30pt" ScrollBarBaseColor="" FrameTableStyle-BorderStyle="Solid" FrameTableStyle-LeftBorderStyle-BorderWidth="" FrameTableStyle-LeftBorderStyle-BorderColor="" FrameTableStyle-RightBorderStyle-BorderWidth="" FrameTableStyle-RightBorderStyle-BorderColor="" FrameTableStyle-BorderWidth="1px" FrameTableStyle-CellSpacing="0" FrameTableStyle-BorderColor="Gray" FrameTableStyle-CellPadding="0" FrameTableStyle-TopBorderStyle-BorderWidth="" FrameTableStyle-TopBorderStyle-BorderColor="" FrameTableStyle-BottomBorderStyle-BorderWidth="" FrameTableStyle-BottomBorderStyle-BorderColor="" HeaderBarStyle-LeftBorderStyle-BorderStyle="Solid" HeaderBarStyle-LeftBorderStyle-BorderWidth="1px" HeaderBarStyle-LeftBorderStyle-BorderColor="White" HeaderBarStyle-VerticalAlign="Middle" HeaderBarStyle-RightBorderStyle-BorderStyle="Solid" HeaderBarStyle-RightBorderStyle-BorderWidth="1px" HeaderBarStyle-RightBorderStyle-BorderColor="Gray" HeaderBarStyle-BorderWidth="1px" HeaderBarStyle-Font-Size="10pt" HeaderBarStyle-BorderColor="Gray" HeaderBarStyle-BorderStyle="Solid" HeaderBarStyle-HorizontalAlign="Center" HeaderBarStyle-ForeColor="Black" HeaderBarStyle-TopBorderStyle-BorderStyle="Solid" HeaderBarStyle-TopBorderStyle-BorderWidth="1px" HeaderBarStyle-TopBorderStyle-BorderColor="White" HeaderBarStyle-BackColor="\#E0E0E0" HeaderBarStyle-BottomBorderStyle-BorderStyle="Solid" HeaderBarStyle-BottomBorderStyle-BorderWidth="1px" HeaderBarStyle-BottomBorderStyle-BorderColor="Gray" ViewTableStyle-LeftBorderStyle-BorderWidth="" ViewTableStyle-LeftBorderStyle-BorderColor="" ViewTableStyle-LayoutFixed="Fixed" ViewTableStyle-RightBorderStyle-BorderWidth="" ViewTableStyle-RightBorderStyle-BorderColor="" ViewTableStyle-BorderWidth="0px" ViewTableStyle-CellSpacing="0" ViewTableStyle-CellPadding="0" ViewTableStyle-TopBorderStyle-BorderWidth="" ViewTableStyle-TopBorderStyle-BorderColor="" ViewTableStyle-BottomBorderStyle-BorderWidth="" ViewTableStyle-BottomBorderStyle-BorderColor="" BottomTableStyle-LeftBorderStyle-BorderWidth="" BottomTableStyle-LeftBorderStyle-BorderColor="" BottomTableStyle-LayoutFixed="Fixed" BottomTableStyle-RightBorderStyle-BorderWidth="" BottomTableStyle-RightBorderStyle-BorderColor="" BottomTableStyle-BorderWidth="0px" BottomTableStyle-CellSpacing="0" BottomTableStyle-CellPadding="1" BottomTableStyle-TopBorderStyle-BorderStyle="Solid" BottomTableStyle-TopBorderStyle-BorderWidth="1px" BottomTableStyle-TopBorderStyle-BorderColor="Gray" BottomTableStyle-BottomBorderStyle-BorderWidth="" BottomTableStyle-BottomBorderStyle-BorderColor="" HeaderBarHeight="15pt" ActiveTabStyle-LeftBorderStyle-BorderWidth="" ActiveTabStyle-LeftBorderStyle-BorderColor="" ActiveTabStyle-RightBorderStyle-BorderWidth="" ActiveTabStyle-RightBorderStyle-BorderColor="" ActiveTabStyle-Height="15pt" ActiveTabStyle-BorderWidth="1px" ActiveTabStyle-Font-Size="10pt" ActiveTabStyle-BorderColor="Gray" ActiveTabStyle-ForeColor="Black" ActiveTabStyle-TopBorderStyle-BorderWidth="" ActiveTabStyle-TopBorderStyle-BorderColor="" ActiveTabStyle-BackColor="White" ActiveTabStyle-BottomBorderStyle-BorderWidth="" ActiveTabStyle-BottomBorderStyle-BorderColor="" HeaderBarTableStyle-LeftBorderStyle-BorderWidth="" HeaderBarTableStyle-LeftBorderStyle-BorderColor="" HeaderBarTableStyle-LayoutFixed="Fixed" HeaderBarTableStyle-RightBorderStyle-BorderWidth="" HeaderBarTableStyle-RightBorderStyle-BorderColor="" HeaderBarTableStyle-BorderWidth="0px" HeaderBarTableStyle-CellSpacing="0" HeaderBarTableStyle-BorderCollapse="Separate" HeaderBarTableStyle-CellPadding="0" HeaderBarTableStyle-TopBorderStyle-BorderWidth="" HeaderBarTableStyle-TopBorderStyle-BorderColor="" HeaderBarTableStyle-BottomBorderStyle-BorderWidth="" HeaderBarTableStyle-BottomBorderStyle-BorderColor="" TabStyle-LeftBorderStyle-BorderWidth="" TabStyle-LeftBorderStyle-BorderColor="" TabStyle-RightBorderStyle-BorderWidth="" TabStyle-RightBorderStyle-BorderColor="" TabStyle-Height="15pt" TabStyle-BorderWidth="1px" TabStyle-Font-Size="10pt" TabStyle-BorderColor="Gray" TabStyle-ForeColor="Black" TabStyle-TopBorderStyle-BorderWidth="" TabStyle-TopBorderStyle-BorderColor="" TabStyle-BackColor="\#E0E0E0" TabStyle-BottomBorderStyle-BorderWidth="" TabStyle-BottomBorderStyle-BorderColor="" ScrollBarArrowColor=""></Aspose.Cells.GridWeb.ViewerStyleTemplate>

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setDPI(double value) {#setDPI-double-}
```
public static void setDPI(double value)
```


Obtiene /Establece los DPI de la máquina.

**Remarks**

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


Establece el nombre de fuente predeterminado del control.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setDefaultFontSize(FontUnit value) {#setDefaultFontSize-com.aspose.gridweb.FontUnit-}
```
public void setDefaultFontSize(FontUnit value)
```


Establece el tamaño de fuente predeterminado del control.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [FontUnit](../../com.aspose.gridweb/fontunit) |  |

### setDefaultGridLineColor(Color value) {#setDefaultGridLineColor-com.aspose.gridweb.Color-}
```
public void setDefaultGridLineColor(Color value)
```


Establece el color predeterminado de la línea de cuadrícula.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setDisplayCellTip(boolean value) {#setDisplayCellTip-boolean-}
```
public void setDisplayCellTip(boolean value)
```


Establece si mostrar sugerencias. el valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEditMode(boolean value) {#setEditMode-boolean-}
```
public void setEditMode(boolean value)
```


Establece el modo de edición del control.

**Remarks**

Cuando se establece en true, las celdas del control son editables y se muestran los íconos de "save" y "undo". Cuando se establece en false, las celdas del control son de solo lectura y los íconos de "save" y "undo" no se muestran.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEnableAJAX(boolean value) {#setEnableAJAX-boolean-}
```
public void setEnableAJAX(boolean value)
```


Establece si usar la llamada AJAX. el valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEnableAsync(boolean value) {#setEnableAsync-boolean-}
```
public void setEnableAsync(boolean value)
```


Establece si cargar los datos de celdas de forma asíncrona, se sugiere aplicar para una hoja con más de 10000 celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEnableClientColumnOperations(boolean value) {#setEnableClientColumnOperations-boolean-}
```
public void setEnableClientColumnOperations(boolean value)
```


Establece si habilitar las operaciones de columna del lado del cliente.

**Remarks**

Cuando se establece en true, el usuario puede usar el menú contextual para agregar/quitar columnas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEnableClientFreeze(boolean value) {#setEnableClientFreeze-boolean-}
```
public void setEnableClientFreeze(boolean value)
```


Establece si habilitar las operaciones de congelación del lado del cliente.

**Remarks**

Cuando se establece en true, el usuario puede usar el menú contextual para congelar/descongelar paneles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEnableClientMergeOperations(boolean value) {#setEnableClientMergeOperations-boolean-}
```
public void setEnableClientMergeOperations(boolean value)
```


Establece si habilitar las operaciones de combinación del lado del cliente.

**Remarks**

Cuando se establece en true, el usuario puede usar el menú contextual para combinar/separar celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEnableClientResizeColumnRow(boolean value) {#setEnableClientResizeColumnRow-boolean-}
```
public void setEnableClientResizeColumnRow(boolean value)
```


Establece si se habilita el redimensionamiento de columnas y filas del lado del cliente.

**Remarks**

Cuando se establece en true, el usuario puede cambiar el tamaño de la columna y la fila del lado del cliente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEnableClientRowOperations(boolean value) {#setEnableClientRowOperations-boolean-}
```
public void setEnableClientRowOperations(boolean value)
```


Establece si se habilitan las operaciones de filas del lado del cliente.

**Remarks**

Cuando se establece en true, el usuario puede usar el menú contextual para agregar/quitar filas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEnableDoubleClickEvent(boolean value) {#setEnableDoubleClickEvent-boolean-}
```
public void setEnableDoubleClickEvent(boolean value)
```


Establece si se habilita el evento de doble clic del lado del cliente.

**Remarks**

Cuando se establece en true, el control recibirá eventos de doble clic del lado del cliente y podrá manejar estos eventos en el lado del servidor. De lo contrario, el control ignorará cualquier evento de doble clic.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEnableMetalLightEffect(boolean value) {#setEnableMetalLightEffect-boolean-}
```
public void setEnableMetalLightEffect(boolean value)
```


Establece si se aplica el efecto de luz metálica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEnablePaging(boolean value) {#setEnablePaging-boolean-}
```
public void setEnablePaging(boolean value)
```


Establece si se habilita el modo de paginación del control.

**Remarks**

Cuando se establece en true, el control mostrará PageSize filas de datos de una vez y mostrará el control de selección de página en la barra de pestañas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEnableStyleDialogbox(boolean value) {#setEnableStyleDialogbox-boolean-}
```
public void setEnableStyleDialogbox(boolean value)
```


Establece si se habilita el cuadro de diálogo de estilo del lado del cliente.

**Remarks**

Cuando se establece en true, el usuario puede usar el cuadro de diálogo de estilo para establecer el estilo de una celda seleccionando "Format Cell..." del menú emergente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


Establece el Enabled en el WebControl

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFilteredPaging(boolean value) {#setFilteredPaging-boolean-}
```
public void setFilteredPaging(boolean value)
```


Establece si se habilita la paginación después de filtrar los datos; tendrá efecto cuando EnablePaging sea verdadero.

**Remarks**

Cuando se establece en true, el control paginará basándose en los datos filtrados; el valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFontFolder(String fontFolder, boolean recursive) {#setFontFolder-java.lang.String-boolean-}
```
public static void setFontFolder(String fontFolder, boolean recursive)
```


Establece la carpeta de fuentes

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fontFolder | java.lang.String | La carpeta que contiene fuentes TrueType. |
| recursive | boolean | Determina si se deben escanear o no las subcarpetas. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public static void setFontFolders(String[] fontFolders, boolean recursive)
```


Establece las carpetas de fuentes

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fontFolders | java.lang.String[] | Las carpetas que contienen fuentes TrueType. |
| recursive | boolean | Determina si se deben escanear o no las subcarpetas. |

### setForceValidation(boolean value) {#setForceValidation-boolean-}
```
public void setForceValidation(boolean value)
```


Establece si se fuerza la validación del lado del cliente.

**Remarks**

Cuando se establece en true, los datos no se enviarán al servidor hasta que todos los campos de entrada sean válidos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setForeColor(Color value) {#setForeColor-com.aspose.gridweb.Color-}
```
public void setForeColor(Color value)
```


Establece el ForeColor en el WebControl

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setFrameTableStyle(GridTableStyle value) {#setFrameTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setFrameTableStyle(GridTableStyle value)
```


Establece el estilo del marco del control.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setGoonDefaultSaveOperation(boolean value) {#setGoonDefaultSaveOperation-boolean-}
```
public void setGoonDefaultSaveOperation(boolean value)
```


Establece si GridWeb realizará la operación de guardado predeterminada; el valor predeterminado es verdadero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHeaderBarHeight(Unit value) {#setHeaderBarHeight-com.aspose.gridweb.Unit-}
```
public void setHeaderBarHeight(Unit value)
```


Establece la altura (System.Web.UI.WebControl.Unit) de la barra de encabezado superior del control.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setHeaderBarStyle(GridTableItemStyle value) {#setHeaderBarStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setHeaderBarStyle(GridTableItemStyle value)
```


Establece el estilo de la barra de encabezado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setHeaderBarTableStyle(GridTableStyle value) {#setHeaderBarTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setHeaderBarTableStyle(GridTableStyle value)
```


Establece el estilo de la barra de encabezado del control.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setHeaderBarWidth(Unit value) {#setHeaderBarWidth-com.aspose.gridweb.Unit-}
```
public void setHeaderBarWidth(Unit value)
```


Establece el ancho (System.Web.UI.WebControl.Unit) de la barra de encabezado izquierda del control.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setHeight(Unit value) {#setHeight-com.aspose.gridweb.Unit-}
```
public void setHeight(Unit value)
```


Establece la altura (System.Web.UI.WebControl.Unit) del control.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setIgnoreStyleWithNoData(boolean value) {#setIgnoreStyleWithNoData-boolean-}
```
public void setIgnoreStyleWithNoData(boolean value)
```


Establece si GridWeb ignora la visualización de filas o columnas que no contienen valores de celda pero están estilizadas. Si se establece en true, el rendimiento será mejor. El valor predeterminado es false, lo que significa que si la última fila/columna consecutiva no tiene valores de celda pero está estilizada, aún se mostrará. Esta opción solo es válida cuando EnableAsync es false. No tiene efecto cuando EnableAsync es true, lo que significa que GridWeb mostrará todas las filas/columnas con estilo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setLoadOptions(GridLoadOptions value) {#setLoadOptions-com.aspose.gridweb.GridLoadOptions-}
```
public void setLoadOptions(GridLoadOptions value)
```


Representa las opciones de carga para GridWeb.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [GridLoadOptions](../../com.aspose.gridweb/gridloadoptions) |  |

### setMaxColumn(int value) {#setMaxColumn-int-}
```
public void setMaxColumn(int value)
```


Establece el índice máximo de columna a mostrar (basado en cero) de la hoja web. El control usa el valor mayor entre MaxColumn y la columna máxima de los datos de la hoja.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMaxRow(int value) {#setMaxRow-int-}
```
public void setMaxRow(int value)
```


Establece el índice máximo de fila a mostrar (basado en cero) de la hoja web. El control usa el valor mayor entre MaxRow y la fila máxima de los datos de la hoja.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMessage(String value) {#setMessage-java.lang.String-}
```
public void setMessage(String value)
```


Establece el mensaje para la cuadrícula.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setMinColumn(int value) {#setMinColumn-int-}
```
public void setMinColumn(int value)
```


Establece el índice mínimo de columna a mostrar (basado en cero) de la hoja web. El control usa el valor menor entre MinColumn y la columna mínima de los datos de la hoja.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMinRow(int value) {#setMinRow-int-}
```
public void setMinRow(int value)
```


Establece el índice mínimo de fila a mostrar (basado en cero) de la hoja web. El control usa el valor menor entre MinRow y la fila mínima de los datos de la hoja.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setNeedRenderGroupRows(boolean value) {#setNeedRenderGroupRows-boolean-}
```
public void setNeedRenderGroupRows(boolean value)
```


Establece si se muestran las filas de grupo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setNoHScroll(boolean value) {#setNoHScroll-boolean-}
```
public void setNoHScroll(boolean value)
```


Establece un valor que indica si la barra de desplazamiento horizontal está oculta.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setNoScroll(boolean value) {#setNoScroll-boolean-}
```
public void setNoScroll(boolean value)
```


Establece si se muestra la barra de desplazamiento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setNoVScroll(boolean value) {#setNoVScroll-boolean-}
```
public void setNoVScroll(boolean value)
```


Establece un valor que indica si la barra de desplazamiento vertical está oculta.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setOnAjaxCallFinishedClientFunction(String value) {#setOnAjaxCallFinishedClientFunction-java.lang.String-}
```
public void setOnAjaxCallFinishedClientFunction(String value)
```


Establece el nombre de la función del lado del cliente que se llamará cuando ajaxcall finalice. La función del cliente debe declararse así:
function GridAjaxcallFinished()
\\{
alert(this.id+\" ajaxcall finished \");
\\}

Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setOnCellErrorClientFunction(String value) {#setOnCellErrorClientFunction-java.lang.String-}
```
public void setOnCellErrorClientFunction(String value)
```


Establece el nombre de la función del lado del cliente que se llamará cuando la validación de una celda falle. La función del cliente debe declararse así:
function MyOnCellError(cell)
\\{
alert(this.getCellValueByCell(cell));
\\}

Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setOnCellSelectedAjaxCallBackClientFunction(String value) {#setOnCellSelectedAjaxCallBackClientFunction-java.lang.String-}
```
public void setOnCellSelectedAjaxCallBackClientFunction(String value)
```


Establece la función del lado del cliente que se llamará cuando se seleccione una celda. La función del cliente debe declararse así:
function MyOnSelectCellAjaxCallBack(cell,customerdata)
\\{

\\}

Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setOnCellSelectedClientFunction(String value) {#setOnCellSelectedClientFunction-java.lang.String-}
```
public void setOnCellSelectedClientFunction(String value)
```


Establece la función del lado del cliente que se llamará cuando se seleccione una celda. La función del cliente debe declararse así:
function MyOnSelectCell(cell)
\\{
GridWeb1.setCellValueByCell(cell, "test");
\\}

Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setOnCellUnselectedClientFunction(String value) {#setOnCellUnselectedClientFunction-java.lang.String-}
```
public void setOnCellUnselectedClientFunction(String value)
```


Establece la función del lado del cliente que se llamará cuando se deseleccione una celda. La función del cliente debe declararse así:
function MyOnUnselectCell(cell)
\\{
this.setCellValueByCell(cell, "test");
\\}

Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setOnCellUpdatedClientFunction(String value) {#setOnCellUpdatedClientFunction-java.lang.String-}
```
public void setOnCellUpdatedClientFunction(String value)
```


Establece el nombre de la función del lado del cliente que se llamará cuando se actualice el valor de una celda. La función del cliente debe declararse así:
function MyOnCellUpdated(cell)
\\{
alert(this.getCellValueByCell(cell));
\\}

Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setOnContextMenuShowClientFunction(String value) {#setOnContextMenuShowClientFunction-java.lang.String-}
```
public void setOnContextMenuShowClientFunction(String value)
```


Establece la función del lado del cliente que se llamará cuando se muestre el menú contextual. La función del cliente debe declararse así:
function onContextMenuShow()
\\{
var menu = event.srcElement;
menu.setItemVisibility("Delete", "block");
menu.setItemVisibility("Update", "none");
\\}

Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setOnDoubleClickCellClientFunction(String value) {#setOnDoubleClickCellClientFunction-java.lang.String-}
```
public void setOnDoubleClickCellClientFunction(String value)
```


Establece la función del lado del cliente que se llamará cuando se haga doble clic en una celda. La función del cliente debe declararse así:
function MyOnDoubleClickCell(cell)
\\{
this.setCellValueByCell(cell, "test");
\\}

Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setOnDoubleClickRowClientFunction(String value) {#setOnDoubleClickRowClientFunction-java.lang.String-}
```
public void setOnDoubleClickRowClientFunction(String value)
```


Establece la función del lado del cliente que se llamará cuando se haga doble clic en una fila. La función del cliente debe declararse así:
function MyOnRowDoubleClick(row)
\\{
alert(row);
\\}

Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setOnGridInitClientFunction(String value) {#setOnGridInitClientFunction-java.lang.String-}
```
public void setOnGridInitClientFunction(String value)
```


Establece el nombre de la función del lado del cliente que se llamará cuando se inicialice la cuadrícula. La función del cliente debe declararse así:
function MyOnGridInit(grid)
\\{
alert("The grid is initialized: " + grid.id);
\\}

Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setOnPageChangeClientFunction(String value) {#setOnPageChangeClientFunction-java.lang.String-}
```
public void setOnPageChangeClientFunction(String value)
```


Establece la función del lado del cliente que se llamará después de cambiar el índice de página. Solo tiene efecto cuando EnablePaging es true. La función del cliente debe declararse así:
function MyOnPageChange(index)
\\{
console.log("current page is:"+index);
\\}

Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setOnPageSubmitClientFunction(String value) {#setOnPageSubmitClientFunction-java.lang.String-}
```
public void setOnPageSubmitClientFunction(String value)
```


Establece la función del cliente que se llamará antes de que la página se envíe del lado del cliente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setOnShapeSelectedClientFunction(String value) {#setOnShapeSelectedClientFunction-java.lang.String-}
```
public void setOnShapeSelectedClientFunction(String value)
```


Establece la función del lado del cliente que se llamará cuando se seleccione una forma. La función del cliente debe declararse así:
function MyOnSelectShape(shape)
\\{
var name=shape.getAttribute("namevalue")
var text=shape.getAttribute("textvalue")
var value=shape.getAttribute("controlvalue")
var type=shape.getAttribute("msotype")
\\}

Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setOnSubmitClientFunction(String value) {#setOnSubmitClientFunction-java.lang.String-}
```
public void setOnSubmitClientFunction(String value)
```


Establece la función del cliente que se llamará antes de que el control se envíe del lado del cliente. La función del cliente debe declararse así:
function MyOnSubmit(arg, cancelEdit)
\\{
return true;
\\}
El argumento arg es el argumento de envío, contiene el comando que se enviará al servidor. cancelEdit es un valor booleano que indica si el control ha descartado la entrada del usuario antes de enviar. El control continuará enviando si la función devuelve true.
Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```


Establece si solo se ajustan las filas cuya altura no está personalizada, el valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setPageSize(int value) {#setPageSize-int-}
```
public void setPageSize(int value)
```


Establece el tamaño de página en modo de paginación.

**Remarks**

Cuando está en modo de paginación, el control mostrará PageSize filas de datos una vez, y mostrará el control de selección de página en la barra de pestañas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPictureCachePath(String value) {#setPictureCachePath-java.lang.String-}
```
public static void setPictureCachePath(String value)
```


Establece la ruta de almacenamiento de imágenes para el libro de trabajo; todas las formas e imágenes se almacenarán en este directorio, la ruta predeterminada es acwcache bajo el Directorio Base de la aplicación actual. Los usuarios deben implementar un servicio programado para limpiar los archivos que estén fuera del tiempo de sesión.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setPresetStyle(int value) {#setPresetStyle-int-}
```
public void setPresetStyle(int value)
```


Establece el estilo predefinido.

Ver [PresetStyle](../../com.aspose.gridweb/presetstyle).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setRefreshValidation(boolean value) {#setRefreshValidation-boolean-}
```
public void setRefreshValidation(boolean value)
```


Establece si se actualiza el valor de validación después de que cambie el valor de la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setRenderHiddenRow(boolean value) {#setRenderHiddenRow-boolean-}
```
public void setRenderHiddenRow(boolean value)
```


Establece si la fila oculta se renderiza en GridControl, el valor predeterminado es false. Si necesita volver a mostrar la fila oculta más tarde, deberá establecerlo en true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setRowHeightForCSV(double value) {#setRowHeightForCSV-double-}
```
public void setRowHeightForCSV(double value)
```


Establece el valor de la altura de fila en puntos para el archivo csv, el valor predeterminado es 14.5.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setScrollBarArrowColor(Color value) {#setScrollBarArrowColor-com.aspose.gridweb.Color-}
```
public void setScrollBarArrowColor(Color value)
```


Especifica el color del botón de flecha de la barra de desplazamiento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setScrollBarBaseColor(Color value) {#setScrollBarBaseColor-com.aspose.gridweb.Color-}
```
public void setScrollBarBaseColor(Color value)
```


Especifica el color de la barra de desplazamiento del control.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSelectCellBgColor(Color value) {#setSelectCellBgColor-com.aspose.gridweb.Color-}
```
public void setSelectCellBgColor(Color value)
```


Especifica el color de fondo de las celdas seleccionadas en un rango de selección múltiple.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSelectCellColor(Color value) {#setSelectCellColor-com.aspose.gridweb.Color-}
```
public void setSelectCellColor(Color value)
```


Especifica el color de las celdas seleccionadas en un rango de selección múltiple.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSessionStorePath(String value) {#setSessionStorePath-java.lang.String-}
```
public void setSessionStorePath(String value)
```


Establece la ruta de almacenamiento de caché de sesión cuando el modo de sesión es File o ViewState, etc.: gridweb.SessionStorePath=\"c:/mytempdir/session\"; luego almacenará los datos de sesión en c:/mytempdir/session.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setSettings(GridWorkbookSettings value) {#setSettings-com.aspose.gridweb.GridWorkbookSettings-}
```
public void setSettings(GridWorkbookSettings value)
```


Representa la configuración del libro de trabajo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [GridWorkbookSettings](../../com.aspose.gridweb/gridworkbooksettings) |  |

### setShowAddButton(boolean value) {#setShowAddButton-boolean-}
```
public void setShowAddButton(boolean value)
```


Establece si se muestra el botón de agregar hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowBottomBar(boolean value) {#setShowBottomBar-boolean-}
```
public void setShowBottomBar(boolean value)
```


Especifica si se muestra la barra de comandos (incluye barra de comandos y barra de pestañas) en la parte inferior del control.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowCellEditBox(boolean value) {#setShowCellEditBox-boolean-}
```
public void setShowCellEditBox(boolean value)
```


Indica si Gridweb muestra la barra de herramientas del cuadro de edición como en MS-EXCEL. Si está habilitado, un cuadro de edición para la celda actual se mostrará en Gridweb. Si habilitamos esta función, debemos importar la biblioteca jquery js en sus archivos aspx para soportar esta nueva característica. Cualquier versión reciente de jquery está bien, etc.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowCommandBarAtTop(boolean value) {#setShowCommandBarAtTop-boolean-}
```
public void setShowCommandBarAtTop(boolean value)
```


Especifica si se muestra la barra de comandos (incluye barra de comandos y barra de pestañas) en la parte superior del control.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowContextMenu(boolean value) {#setShowContextMenu-boolean-}
```
public void setShowContextMenu(boolean value)
```


Establece si se muestra el menú contextual. El valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowDefaultGridLine(boolean value) {#setShowDefaultGridLine-boolean-}
```
public void setShowDefaultGridLine(boolean value)
```


Establece si se muestran las líneas de cuadrícula predeterminadas de las celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowHeaderBar(boolean value) {#setShowHeaderBar-boolean-}
```
public void setShowHeaderBar(boolean value)
```


Establece si se muestra la barra de encabezado

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowLoading(boolean value) {#setShowLoading-boolean-}
```
public void setShowLoading(boolean value)
```


Especifica si se muestra un cuadro de diálogo de carga mientras se envía la solicitud al servidor.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowLoadingPosition(String value) {#setShowLoadingPosition-java.lang.String-}
```
public void setShowLoadingPosition(String value)
```


Especifica la posición izquierda y superior (en px) para mostrar el cuadro de diálogo de carga mientras se envía la solicitud al servidor, etc. 100,200 significa que la posición izquierda y superior del cuadro de diálogo de carga está en 100px,200px.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setShowSaveButton(boolean value) {#setShowSaveButton-boolean-}
```
public void setShowSaveButton(boolean value)
```


Establece si se muestra el botón de guardar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowSubmitButton(boolean value) {#setShowSubmitButton-boolean-}
```
public void setShowSubmitButton(boolean value)
```


Establece si se muestra el botón de enviar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowTabBar(boolean value) {#setShowTabBar-boolean-}
```
public void setShowTabBar(boolean value)
```


Establece si se muestra la barra de pestañas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowTabNavigation(boolean value) {#setShowTabNavigation-boolean-}
```
public void setShowTabNavigation(boolean value)
```


Establece si el botón de navegación de pestañas se muestra, el valor predeterminado es verdadero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowUndoButton(boolean value) {#setShowUndoButton-boolean-}
```
public void setShowUndoButton(boolean value)
```


Establece si se muestra el botón de deshacer.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSpanWrap(boolean value) {#setSpanWrap-boolean-}
```
public void setSpanWrap(boolean value)
```


Especifica si se envuelve el contenido en el cell span, el valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setTabIndex(short value) {#setTabIndex-short-}
```
public void setTabIndex(short value)
```


Establece el TabIndex en el WebControl

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | short |  |

### setTabStyle(GridTableItemStyle value) {#setTabStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setTabStyle(GridTableItemStyle value)
```


Establece el estilo de la barra de pestañas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setToolTip(String value) {#setToolTip-java.lang.String-}
```
public void setToolTip(String value)
```


Establece el ToolTip en el WebControl

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setUseClientPageHeight(boolean value) {#setUseClientPageHeight-boolean-}
```
public void setUseClientPageHeight(boolean value)
```


Establece si GridWeb usa la altura de la página del cliente como altura del control, adecuado cuando se establece Height=\"100%\", el valor predeterminado es falso.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setViewPanelScrollLeft(String value) {#setViewPanelScrollLeft-java.lang.String-}
```
public void setViewPanelScrollLeft(String value)
```


Establece la posición de la barra de desplazamiento del panel de vista de la cuadrícula.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setViewPanelScrollTop(String value) {#setViewPanelScrollTop-java.lang.String-}
```
public void setViewPanelScrollTop(String value)
```


Establece la posición de la barra de desplazamiento del panel de vista de la cuadrícula.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setViewTableStyle(GridTableStyle value) {#setViewTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setViewTableStyle(GridTableStyle value)
```


Establece el estilo del panel de vista de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


Establece el ancho (System.Web.UI.WebControl.Unit) del control.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setXhtmlMode(boolean value) {#setXhtmlMode-boolean-}
```
public void setXhtmlMode(boolean value)
```


Establece si se usa el estilo XHTML, el valor predeterminado es verdadero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

