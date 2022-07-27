---
title: MainWeb
second_title: Referencia de API de Aspose.Cells para .NET
description: Clase principal del control GridWeb. Solo para uso interno.
type: docs
weight: 850
url: /es/net/aspose.cells.gridweb/mainweb/
---
## MainWeb class

Clase principal del control GridWeb. Solo para uso interno.

```csharp
public class MainWeb : ExtWebControl, INamingContainer, IPostBackDataHandler, 
    IPostBackEventHandler, ISerializable
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [MainWeb](mainweb)() | Constructor predeterminado |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ActiveCell](../../aspose.cells.gridweb/mainweb/activecell) { get; set; } | Obtiene o establece la celda activa de la hoja actual. Cambiado para poder escribir desde la versión 1.9.0.1. |
| [ActiveCellBgColor](../../aspose.cells.gridweb/mainweb/activecellbgcolor) { get; set; } | Especifica el color de fondo de la celda activa. |
| [ActiveCellColor](../../aspose.cells.gridweb/mainweb/activecellcolor) { get; set; } | Especifica el color de la celda activa. |
| [ActiveHeaderBgColor](../../aspose.cells.gridweb/mainweb/activeheaderbgcolor) { get; set; } | Especifica el color de fondo del encabezado de fila/columna activo. |
| [ActiveHeaderColor](../../aspose.cells.gridweb/mainweb/activeheadercolor) { get; set; } | Especifica el color del encabezado de fila/columna activo. |
| [ActiveSheet](../../aspose.cells.gridweb/mainweb/activesheet) { get; } | Obtiene la hoja activa |
| [ActiveSheetIndex](../../aspose.cells.gridweb/mainweb/activesheetindex) { get; set; } | Obtiene o establece el índice de la hoja activa. Igual a WebWorksheets.ActiveSheetIndex. |
| [ActiveTabStyle](../../aspose.cells.gridweb/mainweb/activetabstyle) { get; set; } | Especifica el estilo de la pestaña activa. |
| [ACWClientPath](../../aspose.cells.gridweb/mainweb/acwclientpath) { get; set; } | Obtiene o establece la ruta web de los archivos de script/imagen del control. Por ejemplo: "http://localhost/acw_client". También puede establecer este valor en el archivo web.config. Agregue esta sección a la sección &lt;configuration&gt;: &lt;configuración de la aplicación&gt;&lt;agregar clave="aspose.cells.gridweb.acw_client_path" value="/acw_client/" /&gt;&lt;/aplicaciónConfiguración&gt; |
| [ACWLanguageFileUrl](../../aspose.cells.gridweb/mainweb/acwlanguagefileurl) { get; set; } | Obtiene o establece la URL web del archivo de idioma del control. Por ejemplo: "/acw_client/lang_en.js". De forma predeterminada, se utiliza un archivo en inglés incorporado. |
| [AutoRefreshChart](../../aspose.cells.gridweb/mainweb/autorefreshchart) { get; set; } | Obtiene o establece si la imagen del gráfico se actualiza mientras se actualiza el valor de la celda. El valor predeterminado es true |
| [BottomTableStyle](../../aspose.cells.gridweb/mainweb/bottomtablestyle) { get; set; } | Obtiene o establece el estilo de la barra inferior del control. |
| [CurrentPageIndex](../../aspose.cells.gridweb/mainweb/currentpageindex) { get; set; } |  |
| [CustomCalculationEngine](../../aspose.cells.gridweb/mainweb/customcalculationengine) { get; set; } | Representa el motor de cálculo personalizado del usuario para ampliar el motor de cálculo predeterminado de Aspose.Cells. |
| [CustomCommandButtons](../../aspose.cells.gridweb/mainweb/customcommandbuttons) { get; } |  |
| [CustomStyleFileName](../../aspose.cells.gridweb/mainweb/customstylefilename) { get; set; } | Obtiene o establece el nombre del archivo de estilo personalizado. |
| [DefaultFontName](../../aspose.cells.gridweb/mainweb/defaultfontname) { get; set; } | Obtiene o establece el nombre de fuente predeterminado del control. |
| [DefaultFontSize](../../aspose.cells.gridweb/mainweb/defaultfontsize) { get; set; } | Obtiene o establece el tamaño de fuente predeterminado del control. |
| [DefaultGridLineColor](../../aspose.cells.gridweb/mainweb/defaultgridlinecolor) { get; set; } | Obtiene o establece el color de la línea de cuadrícula predeterminada. |
| [DisplayCellTip](../../aspose.cells.gridweb/mainweb/displaycelltip) { get; set; } |  |
| [EditMode](../../aspose.cells.gridweb/mainweb/editmode) { get; set; } | Obtiene o establece el modo de edición del control. |
| [EnableAJAX](../../aspose.cells.gridweb/mainweb/enableajax) { get; set; } |  |
| [EnableAsync](../../aspose.cells.gridweb/mainweb/enableasync) { get; set; } | Obtiene o establece si carga los datos de las celdas de forma asíncrona, se sugiere solicitar una hoja con más de 10000 celdas. |
| [EnableClientColumnOperations](../../aspose.cells.gridweb/mainweb/enableclientcolumnoperations) { get; set; } | Obtiene o establece si habilitar las operaciones de columna del lado del cliente. |
| [EnableClientFreeze](../../aspose.cells.gridweb/mainweb/enableclientfreeze) { get; set; } | Obtiene o establece si habilitar las operaciones de congelación del lado del cliente. |
| [EnableClientMergeOperations](../../aspose.cells.gridweb/mainweb/enableclientmergeoperations) { get; set; } | Obtiene o establece si habilitar las operaciones de fusión del lado del cliente. |
| [EnableClientResizeColumnRow](../../aspose.cells.gridweb/mainweb/enableclientresizecolumnrow) { get; set; } | Obtiene o establece si habilitar la fila y la columna de cambio de tamaño del lado del cliente. |
| [EnableClientRowOperations](../../aspose.cells.gridweb/mainweb/enableclientrowoperations) { get; set; } | Obtiene o establece si habilitar las operaciones de fila del lado del cliente. |
| [EnableDoubleClickEvent](../../aspose.cells.gridweb/mainweb/enabledoubleclickevent) { get; set; } | Obtiene o establece si habilitar el evento de doble clic del lado del cliente. |
| [EnableMetalLightEffect](../../aspose.cells.gridweb/mainweb/enablemetallighteffect) { get; set; } | Obtiene o establece si se aplica el efecto de luz metálica. |
| [EnablePaging](../../aspose.cells.gridweb/mainweb/enablepaging) { get; set; } | Obtiene o establece si habilitar el modo de paginación del control. |
| [EnableStyleDialogbox](../../aspose.cells.gridweb/mainweb/enablestyledialogbox) { get; set; } | Obtiene o establece si habilitar el cuadro de diálogo de estilo del lado del cliente. |
| [FilteredPaging](../../aspose.cells.gridweb/mainweb/filteredpaging) { get; set; } | Obtiene o establece si habilitar la paginación después de filtrar los datos, tendrá efecto cuando EnablePaging sea verdadero. |
| [ForceValidation](../../aspose.cells.gridweb/mainweb/forcevalidation) { get; set; } | Obtiene o establece si se debe forzar la validación del lado del cliente. |
| [FrameTableStyle](../../aspose.cells.gridweb/mainweb/frametablestyle) { get; set; } | Obtiene o establece el estilo de marco del control. |
| [GoonDefaultSaveOperation](../../aspose.cells.gridweb/mainweb/goondefaultsaveoperation) { get; set; } | Obtiene o establece si GridWeb realizará la operación de guardado predeterminada, el valor predeterminado es verdadero. |
| [HeaderBarHeight](../../aspose.cells.gridweb/mainweb/headerbarheight) { get; set; } | Obtiene o establece la altura (System.Web.UI.WebControl.Unit) de la barra de encabezado superior del control. |
| [HeaderBarStyle](../../aspose.cells.gridweb/mainweb/headerbarstyle) { get; set; } | Obtiene o establece el estilo de la barra de encabezado. |
| [HeaderBarTableStyle](../../aspose.cells.gridweb/mainweb/headerbartablestyle) { get; set; } | Obtiene o establece el estilo de la barra de encabezado del control. |
| [HeaderBarWidth](../../aspose.cells.gridweb/mainweb/headerbarwidth) { get; set; } | Obtiene o establece el ancho (System.Web.UI.WebControl.Unit) o la barra de encabezado izquierda del control. |
| override [Height](../../aspose.cells.gridweb/mainweb/height) { get; set; } | Obtiene o establece la altura (System.Web.UI.WebControl.Unit) del control. |
| [IsCalculateFormula](../../aspose.cells.gridweb/mainweb/iscalculateformula) { get; set; } | Obtiene o establece si se calcula la fórmula después de cambiar el valor de la celda o después de importar el archivo. El valor predeterminado es verdadero. |
| [IsPostBack](../../aspose.cells.gridweb/mainweb/ispostback) { get; } | Obtiene un valor que indica si gridweb se está cargando en respuesta a una devolución de datos del cliente, o si se está cargando y accediendo por primera vez. |
| [LinksTable](../../aspose.cells.gridweb/mainweb/linkstable) { get; } |  |
| [MaxColumn](../../aspose.cells.gridweb/mainweb/maxcolumn) { get; set; } | Obtiene o establece el índice máximo de la columna de visualización (basado en cero) de la hoja web. El control usa el valor mayor de MaxColumn y la columna máxima de datos de la hoja. |
| [MaxRow](../../aspose.cells.gridweb/mainweb/maxrow) { get; set; } | Obtiene o establece el índice máximo de fila de visualización (basado en cero) de la hoja web. El control usa el mayor valor de MaxRow y la fila máxima de datos de la hoja. |
| [Message](../../aspose.cells.gridweb/mainweb/message) { get; set; } |  |
| [MinColumn](../../aspose.cells.gridweb/mainweb/mincolumn) { get; set; } |  |
| [MinRow](../../aspose.cells.gridweb/mainweb/minrow) { get; set; } | Obtiene o establece el índice mínimo de fila de visualización (basado en cero) de la hoja web. El control usa el valor más pequeño de MinRow y la fila mínima de los datos de la hoja. |
| [ModifiedCells](../../aspose.cells.gridweb/mainweb/modifiedcells) { get; } | Obtiene la colección de celdas que modificó el cliente. |
| [NeedRenderGroupRows](../../aspose.cells.gridweb/mainweb/needrendergrouprows) { get; set; } | Obtiene o establece si mostrar filas de grupo . |
| [NoHScroll](../../aspose.cells.gridweb/mainweb/nohscroll) { get; set; } | Obtiene o establece un valor que indica si la barra de desplazamiento horizontal está oculta. |
| [NoScroll](../../aspose.cells.gridweb/mainweb/noscroll) { get; set; } |  |
| [NoVScroll](../../aspose.cells.gridweb/mainweb/novscroll) { get; set; } | Obtiene o establece un valor que indica si la barra de desplazamiento vertical está oculta. |
| [OnAjaxCallFinishedClientFunction](../../aspose.cells.gridweb/mainweb/onajaxcallfinishedclientfunction) { get; set; } | Obtiene o establece el nombre de la función del lado del cliente que se llamará cuando finalice ajaxcall. La función del cliente debe declararse así: función GridAjaxcallFinished() { alert(this.id+"llamada ajax finalizada"); } Nota: puede usar el puntero "este" en la función del cliente para señalar el control de cuadrícula que activa el evento. |
| [OnCellErrorClientFunction](../../aspose.cells.gridweb/mainweb/oncellerrorclientfunction) { get; set; } | Obtiene o establece el nombre de la función del lado del cliente que se llamará cuando falle la validación de una celda. La función del cliente debe declararse así: función MyOnCellError(celda) { alerta(GridWeb1.getCellValueByCell(celda)); } Nota: puede usar el puntero "este" en la función del cliente para señalar el control de cuadrícula que activa el evento. |
| [OnCellSelectedAjaxCallBackClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedajaxcallbackclientfunction) { get; set; } | Obtiene o establece la función del lado del cliente que se llamará cuando se seleccione una celda. La función del cliente debe declararse así: function MyOnSelectCellAjaxCallBack(cell,customerdata) { } Nota: puede usar el puntero "este" en la función del cliente para señalar el control de cuadrícula que activa el evento. |
| [OnCellSelectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedclientfunction) { get; set; } | Obtiene o establece la función del lado del cliente que se llamará cuando se seleccione una celda. La función del cliente debe declararse así: función MyOnSelectCell(celda) { GridWeb1.setCellValueByCell(celda, "prueba"); } Nota: puede usar el puntero "este" en la función del cliente para señalar el control de cuadrícula que activa el evento. |
| [OnCellUnselectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellunselectedclientfunction) { get; set; } | Obtiene o establece la función del lado del cliente que se llamará cuando una celda no esté seleccionada. La función del cliente debe declararse así: función MyOnUnselectCell(celda) { GridWeb1.setCellValueByCell(celda, "prueba"); } Nota: puede usar el puntero "este" en la función del cliente para señalar el control de cuadrícula que activa el evento. |
| [OnCellUpdatedClientFunction](../../aspose.cells.gridweb/mainweb/oncellupdatedclientfunction) { get; set; } | Obtiene o establece el nombre de la función del lado del cliente que se llamará cuando se actualice el valor de una celda. La función del cliente debe declararse así: función MyOnCellUpdated(celda) { alert(this.getCellValueByCell(cell)); } Nota: puede usar el puntero "este" en la función del cliente para señalar el control de cuadrícula que activa el evento. |
| [OnContextMenuShowClientFunction](../../aspose.cells.gridweb/mainweb/oncontextmenushowclientfunction) { get; set; } | Obtiene o establece la función del lado del cliente que se llamará cuando se muestre el menú contextual. La función del cliente debe declararse así: función enContextMenuShow() { var menú = evento.srcElement; menu.setItemVisibility("Borrar", "bloquear"); menu.setItemVisibility("Actualizar", "ninguno"); } Nota: puede usar el puntero "este" en la función del cliente para señalar el control de cuadrícula que activa el evento. |
| [OnDoubleClickCellClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickcellclientfunction) { get; set; } | Obtiene o establece la función del lado del cliente que se llamará cuando se haga doble clic en una celda. La función del cliente debe declararse así: función MyOnDoubleClickCell(celda) { GridWeb1.setCellValueByCell(celda, "prueba"); } Nota: puede usar el puntero "este" en la función del cliente para señalar el control de cuadrícula que activa el evento. |
| [OnDoubleClickRowClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickrowclientfunction) { get; set; } | Obtiene o establece la función del lado del cliente que se llamará cuando se haga doble clic en una fila. La función del cliente debe declararse así: función MyOnRowDoubleClick(fila) { alerta(fila); } Nota: puede usar el puntero "este" en la función del cliente para señalar el control de cuadrícula que activa el evento. |
| [OnGridInitClientFunction](../../aspose.cells.gridweb/mainweb/ongridinitclientfunction) { get; set; } | Obtiene o establece el nombre de la función del lado del cliente que se llamará cuando se inicialice la cuadrícula. La función del cliente debe declararse así: función MyOnGridInit(cuadrícula) { alert("El grid se inicializa: " + grid.id); } Nota: puede usar el puntero "este" en la función del cliente para señalar el control de cuadrícula que activa el evento. |
| [OnlyAuto](../../aspose.cells.gridweb/mainweb/onlyauto) { get; set; } | Obtiene o establece si solo se ajustan las filas cuya altura no está personalizada, el valor predeterminado es false |
| [OnPageChangeClientFunction](../../aspose.cells.gridweb/mainweb/onpagechangeclientfunction) { get; set; } | Obtiene o configura la función del lado del cliente para que se llame después de cambiar el índice de la página. Solo tiene efecto cuando EnablePaging es verdadero. La función del cliente debe declararse así: función MyOnPageChange(índice) { console.log("la página actual es:"+índice); } Nota: puede usar el puntero "este" en la función del cliente para señalar el control de cuadrícula que activa el evento. |
| [OnPageSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onpagesubmitclientfunction) { get; set; } | Obtiene o establece la función del cliente que se llamará antes de enviar la página en el lado del cliente. |
| [OnShapeSelectedClientFunction](../../aspose.cells.gridweb/mainweb/onshapeselectedclientfunction) { get; set; } | Obtiene o establece la función del lado del cliente que se llamará cuando se seleccione una forma. La función del cliente debe declararse así: función MyOnSelectShape(forma) { var nombre=forma.getAttribute("nombrevalor") var text=shape.getAttribute("textvalue") var valor=forma.getAttribute("valor de control") var tipo=forma.getAttribute("msotype") } Nota: puede usar el puntero "este" en la función del cliente para señalar el control de cuadrícula que activa el evento. |
| [OnSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onsubmitclientfunction) { get; set; } | Obtiene o establece la función del cliente que se llamará antes de que el control se envíe al lado del cliente. La función del cliente debe declararse así: function MyOnSubmit(arg, cancelEdit) { devolver verdadero;} El argumento es el argumento de envío, contiene el comando que se publicará en el servidor. CancelEdit es un valor booleano que indica si el control ha descartado la entrada del usuario antes de enviar. El control continuará enviando si la función devuelve verdadero.  Nota: puede usar el puntero "este" en la función del cliente para señalar el control de cuadrícula que activa el evento. |
| [PageSize](../../aspose.cells.gridweb/mainweb/pagesize) { get; set; } | Obtiene o establece el tamaño de página en modo paginación. |
| [PicturesTable](../../aspose.cells.gridweb/mainweb/picturestable) { get; } |  |
| [PresetStyle](../../aspose.cells.gridweb/mainweb/presetstyle) { get; set; } | Obtiene o establece el estilo preestablecido. |
| [RefreshValidation](../../aspose.cells.gridweb/mainweb/refreshvalidation) { get; set; } | Obtiene o establece si actualizar el valor de validación después de que cambie el valor de la celda. |
| [RenderHiddenRow](../../aspose.cells.gridweb/mainweb/renderhiddenrow) { get; set; } | Obtiene o establece si la fila oculta se representa en GridControl, el valor predeterminado es falso. si necesita mostrar la fila oculta más tarde, debe configurarlo como verdadero |
| [ScrollBarArrowColor](../../aspose.cells.gridweb/mainweb/scrollbararrowcolor) { get; set; } | Especifica el color del botón de flecha de la barra de desplazamiento. |
| [ScrollBarBaseColor](../../aspose.cells.gridweb/mainweb/scrollbarbasecolor) { get; set; } | Especifica el color de la barra de desplazamiento del control. |
| [SelectCellBgColor](../../aspose.cells.gridweb/mainweb/selectcellbgcolor) { get; set; } | Especifica el color de fondo de las celdas seleccionadas en el rango de selección múltiple. |
| [SelectCellColor](../../aspose.cells.gridweb/mainweb/selectcellcolor) { get; set; } | Especifica el color de las celdas seleccionadas en el rango de selección múltiple. |
| [SessionLoaded](../../aspose.cells.gridweb/mainweb/sessionloaded) { get; set; } |  |
| [SessionMode](../../aspose.cells.gridweb/mainweb/sessionmode) { get; set; } | Obtiene o establece el modo de sesión de la cuadrícula. Hay 4 tipos de modo de sesión: 1. Sesión (predeterminado): use la sesión del sistema para almacenar datos de la hoja. Generalmente, asp.net usa el estado de sesión de InProc. La cuadrícula también admite el estado de la sesión de proceso de "StateServer" state y el estado de la sesión de SQLServer. 2. ViewState: use el estado de vista de la página para almacenar datos de la hoja. 3. Personalizado: use los eventos LoadCustomData y SheetDataUpdated para almacenar/recuperar datos de hojas. 4. Archivo: almacenar/recuperar datos de la hoja en SessionStorePath. |
| [SessionSaved](../../aspose.cells.gridweb/mainweb/sessionsaved) { get; set; } |  |
| [SessionStorePath](../../aspose.cells.gridweb/mainweb/sessionstorepath) { get; set; } | Obtiene o establece la ruta del almacenamiento de caché de sesión cuando el modo de sesión es Archivo o ViewState, etc: gridweb.SessionStorePath="c:/mytempdir/session"; luego almacenará los datos de la sesión en c:/mytempdir/session |
| [Settings](../../aspose.cells.gridweb/mainweb/settings) { get; set; } | Representa la configuración del libro. |
| [ShapesTable](../../aspose.cells.gridweb/mainweb/shapestable) { get; } |  |
| [ShowAddButton](../../aspose.cells.gridweb/mainweb/showaddbutton) { get; set; } | Obtiene o establece si mostrar el botón Agregar hoja de cálculo. |
| [ShowBottomBar](../../aspose.cells.gridweb/mainweb/showbottombar) { get; set; } |  |
| [ShowCellEditBox](../../aspose.cells.gridweb/mainweb/showcelleditbox) { get; set; } | si Gridweb muestra la barra de herramientas del cuadro de edición como en MS-EXCEL. Si está habilitado, se mostrará un cuadro de edición para la celda actual en Gridweb. si habilitamos esta función, debemos importar la biblioteca jquery js en sus archivos aspx para admitir esta nueva función. toda la última versión de jquery está bien. etc. |
| [ShowCommandBarAtTop](../../aspose.cells.gridweb/mainweb/showcommandbarattop) { get; set; } | Especifica si mostrar la barra de comandos (incluye la barra de comandos y la barra de pestañas) en la parte superior del control. |
| [ShowContextMenu](../../aspose.cells.gridweb/mainweb/showcontextmenu) { get; set; } |  |
| [ShowDefaultGridLine](../../aspose.cells.gridweb/mainweb/showdefaultgridline) { get; set; } | Obtiene o establece si mostrar las líneas de cuadrícula predeterminadas de las celdas. |
| [ShowHeaderBar](../../aspose.cells.gridweb/mainweb/showheaderbar) { get; set; } |  |
| [ShowLoading](../../aspose.cells.gridweb/mainweb/showloading) { get; set; } | Especifica si mostrar un cuadro de diálogo de carga durante la devolución al servidor. |
| [ShowLoadingPosition](../../aspose.cells.gridweb/mainweb/showloadingposition) { get; set; } | Especifica la posición superior izquierda (en px) para mostrar el cuadro de diálogo de carga mientras se envía al servidor, etc. 100,200 significa que la posición superior izquierda del cuadro de diálogo de carga está en 100px,200px . |
| [ShowSaveButton](../../aspose.cells.gridweb/mainweb/showsavebutton) { get; set; } | Obtiene o establece si mostrar el botón Guardar. |
| [ShowSubmitButton](../../aspose.cells.gridweb/mainweb/showsubmitbutton) { get; set; } | Obtiene o establece si mostrar el botón de envío. |
| [ShowTabBar](../../aspose.cells.gridweb/mainweb/showtabbar) { get; set; } |  |
| [ShowTabNavigation](../../aspose.cells.gridweb/mainweb/showtabnavigation) { get; set; } | Obtiene o establece si se muestra el botón de navegación de pestañas, el valor predeterminado es verdadero. |
| [ShowUndoButton](../../aspose.cells.gridweb/mainweb/showundobutton) { get; set; } | Obtiene o establece si mostrar el botón de deshacer. |
| [SpanWrap](../../aspose.cells.gridweb/mainweb/spanwrap) { get; set; } | Especifica si se ajusta el contenido en el intervalo de celdas. El valor predeterminado es verdadero. |
| [TabStyle](../../aspose.cells.gridweb/mainweb/tabstyle) { get; set; } | Obtiene o establece el estilo de la barra de pestañas. |
| [UseClientPageHeight](../../aspose.cells.gridweb/mainweb/useclientpageheight) { get; set; } | Obtiene o establece si gridweb usa la altura de la página del cliente como altura de control, adecuado para cuando se establece Height="100%", el valor predeterminado es false |
| [ValidationsTable](../../aspose.cells.gridweb/mainweb/validationstable) { get; } |  |
| [ViewPanelScrollLeft](../../aspose.cells.gridweb/mainweb/viewpanelscrollleft) { get; set; } | Obtiene o establece la posición de la barra de desplazamiento del panel de visualización de la cuadrícula. |
| [ViewPanelScrollTop](../../aspose.cells.gridweb/mainweb/viewpanelscrolltop) { get; set; } | Obtiene o establece la posición de la barra de desplazamiento del panel de visualización de la cuadrícula. |
| [ViewTableStyle](../../aspose.cells.gridweb/mainweb/viewtablestyle) { get; set; } | Obtiene o establece el estilo del panel de vista de datos. |
| [WebWorksheets](../../aspose.cells.gridweb/mainweb/webworksheets) { get; } |  |
| override [Width](../../aspose.cells.gridweb/mainweb/width) { get; set; } | Obtiene o establece el ancho (System.Web.UI.WebControl.Unit) del control. |
| [WorkSheets](../../aspose.cells.gridweb/mainweb/worksheets) { get; } |  |
| [XhtmlMode](../../aspose.cells.gridweb/mainweb/xhtmlmode) { get; set; } |  |
| static [PictureCachePath](../../aspose.cells.gridweb/mainweb/picturecachepath) { get; set; } | Obtiene o establece la ruta de almacenamiento de imágenes para el libro de trabajo, todas las formas, las imágenes se almacenarán en este directorio, la ruta predeterminada es acwcache en el directorio base de la aplicación actual los usuarios deben implementar un servicio de programación para limpiar los archivos que están fuera de tiempo de sesión. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CalculateFormula](../../aspose.cells.gridweb/mainweb/calculateformula)() | Calcula el resultado de fórmulas. |
| override [DataBind](../../aspose.cells.gridweb/mainweb/databind)() | Vincula el control y todos sus controles secundarios a su fuente de datos. |
| override [Dispose](../../aspose.cells.gridweb/mainweb/dispose)() |  |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile#importexcelfile)(Stream) | Importaciones desde un flujo de archivo de Excel, incluido el flujo de archivo de disco o el flujo de memoria. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile#importexcelfile_1)(string) | Importaciones desde un archivo excel. |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile#loadcsvfile)(Stream) | Carga datos desde un flujo de archivo CSV. |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile#loadcsvfile_1)(string) | Carga datos desde un archivo CSV. |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile#loadhtmlfile)(Stream) | Carga datos desde un flujo de archivos HTML. |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile#loadhtmlfile_1)(string) | Carga datos desde un archivo HTML. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile#loadspreadsheetmlfile)(Stream) | Carga datos de un flujo de archivo SpreadSheetML. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile#loadspreadsheetmlfile_1)(string) | Carga datos desde un archivo SpreadSheetML. |
| [RefreshChartShape](../../aspose.cells.gridweb/mainweb/refreshchartshape)() | actualizar toda la imagen del gráfico para la hoja de trabajo activa . |
| override [RenderBeginTag](../../aspose.cells.gridweb/mainweb/renderbegintag)(HtmlTextWriter) |  |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile#savecsvfile)(Stream) | Guarda los datos en un flujo de archivo CSV. |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile#savecsvfile_1)(string) | Guarda los datos en un archivo CSV. |
| [SaveCustomStyleFile](../../aspose.cells.gridweb/mainweb/savecustomstylefile)(string) | Guarda los datos de estilo actuales del control en un archivo xml. Puede usarse para crear su archivo de estilo personalizado. |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile#savehtmlfile)(Stream) | Guarda los datos en un flujo de archivos HTML. |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile#savehtmlfile_1)(string) | Guarda los datos en un archivo HTML. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile#savespreadsheetmlfile)(Stream) | Guarda datos en un flujo de archivo SpreadSheetML. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile#savespreadsheetmlfile_1)(string) | Guarda los datos en un archivo SpreadSheetML. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile#savetoexcelfile)(Stream) | Guarda las hojas de trabajo en un archivo de Excel. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile#savetoexcelfile_3)(string) | Guarda las hojas de cálculo en un archivo de Excel con formato Excel 2003. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile#savetoexcelfile_1)(Stream, GridSaveFormat) | Guarda las hojas de trabajo en un archivo de Excel. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile#savetoexcelfile_2)(Stream, GridSaveOptions) | Guarda las hojas de trabajo en un archivo de Excel. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile#savetoexcelfile_4)(string, GridSaveFormat) | Guarda las hojas de trabajo en un archivo de Excel. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile#savetoexcelfile_5)(string, GridSaveOptions) | Guarda las hojas de trabajo en un archivo de Excel. |
| [SetCustomStyle](../../aspose.cells.gridweb/mainweb/setcustomstyle)(Stream) | establece el archivo de estilo personalizado de la secuencia, incluida la secuencia de archivos de disco o la secuencia de memoria. |

### Ver también

* class [ExtWebControl](../extwebcontrol)
* espacio de nombres [Aspose.Cells.GridWeb](../../aspose.cells.gridweb)
* asamblea [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
