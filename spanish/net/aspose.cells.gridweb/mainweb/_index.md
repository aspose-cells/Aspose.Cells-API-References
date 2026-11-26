---
title: "Clase MainWeb"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridWeb.MainWeb. Clase padre del control GridWeb. Solo uso interno"
type: docs
url: /es/net/aspose.cells.gridweb/mainweb/
---
## MainWeb class

Clase padre del control GridWeb. Solo para uso interno.

```csharp
public class MainWeb : ExtWebControl, INamingContainer, IPostBackDataHandler, 
    IPostBackEventHandler, ISerializable
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [MainWeb](mainweb/)() | El constructor predeterminado del control MainWeb. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ActiveCell](../../aspose.cells.gridweb/mainweb/activecell/) { get; set; } | Obtiene o establece la celda activa de la hoja actual. Cambiado a escribible desde la versión 1.9.0.1. |
| [ActiveCellBgColor](../../aspose.cells.gridweb/mainweb/activecellbgcolor/) { get; set; } | Especifica el color de fondo de la celda activa. |
| [ActiveCellColor](../../aspose.cells.gridweb/mainweb/activecellcolor/) { get; set; } | Especifica el color de la celda activa. |
| [ActiveHeaderBgColor](../../aspose.cells.gridweb/mainweb/activeheaderbgcolor/) { get; set; } | Especifica el color de fondo del encabezado de fila/columna activo. |
| [ActiveHeaderColor](../../aspose.cells.gridweb/mainweb/activeheadercolor/) { get; set; } | Especifica el color del encabezado de fila/columna activo. |
| [ActiveSheet](../../aspose.cells.gridweb/mainweb/activesheet/) { get; } | Obtiene la hoja activa |
| [ActiveSheetIndex](../../aspose.cells.gridweb/mainweb/activesheetindex/) { get; set; } | Obtiene o establece el índice de la hoja activa. Igual a WebWorksheets.ActiveSheetIndex. |
| [ActiveTabStyle](../../aspose.cells.gridweb/mainweb/activetabstyle/) { get; set; } | Especifica el estilo de la pestaña activa. |
| [ACWClientPath](../../aspose.cells.gridweb/mainweb/acwclientpath/) { get; set; } | Obtiene o establece la ruta web de los archivos de script/imagen del control. Por ejemplo: "http://localhost/acw_client". También puede establecer este valor en el archivo web.config. Añada esta sección a la sección `<configuration>`:`<appSettings>``<add key=\"aspose.cells.gridweb.acw_client_path\" value=\"/acw_client/\" />``</appSettings>` |
| [ACWLanguageFileUrl](../../aspose.cells.gridweb/mainweb/acwlanguagefileurl/) { get; set; } | Obtiene o establece la URL web del archivo de idioma del control. Por ejemplo: \"/acw_client/lang_en.js\". Por defecto, se utiliza un archivo de inglés incorporado. |
| [AutoRefreshChart](../../aspose.cells.gridweb/mainweb/autorefreshchart/) { get; set; } | Obtiene o establece si la imagen del gráfico se actualiza al actualizar el valor de la celda. El valor predeterminado es true. |
| [BottomTableStyle](../../aspose.cells.gridweb/mainweb/bottomtablestyle/) { get; set; } | Obtiene o establece el estilo de la barra inferior del control. |
| [CurrentPageIndex](../../aspose.cells.gridweb/mainweb/currentpageindex/) { get; set; } | Obtiene o establece el índice de página actual en modo de paginación. |
| [CustomCalculationEngine](../../aspose.cells.gridweb/mainweb/customcalculationengine/) { get; set; } | Representa el motor de cálculo personalizado del usuario para ampliar el motor de cálculo predeterminado de Aspose.Cells. |
| [CustomCommandButtons](../../aspose.cells.gridweb/mainweb/customcommandbuttons/) { get; } | Obtiene la colección de botones de comando personalizados |
| [CustomStyleFileName](../../aspose.cells.gridweb/mainweb/customstylefilename/) { get; set; } | Obtiene o establece el nombre del archivo de estilo personalizado. |
| [DefaultFontName](../../aspose.cells.gridweb/mainweb/defaultfontname/) { get; set; } | Obtiene o establece el nombre de fuente predeterminado del control. |
| [DefaultFontSize](../../aspose.cells.gridweb/mainweb/defaultfontsize/) { get; set; } | Obtiene o establece el tamaño de fuente predeterminado del control. |
| [DefaultGridLineColor](../../aspose.cells.gridweb/mainweb/defaultgridlinecolor/) { get; set; } | Obtiene o establece el color de la línea de cuadrícula predeterminada. |
| [DisplayCellTip](../../aspose.cells.gridweb/mainweb/displaycelltip/) { get; set; } | Obtiene o establece si se muestran consejos. El valor predeterminado es verdadero. |
| [EditMode](../../aspose.cells.gridweb/mainweb/editmode/) { get; set; } | Obtiene o establece el modo de edición del control. |
| [EnableAJAX](../../aspose.cells.gridweb/mainweb/enableajax/) { get; set; } | Obtiene o establece si se usa llamada AJAX. El valor predeterminado es verdadero. |
| [EnableAsync](../../aspose.cells.gridweb/mainweb/enableasync/) { get; set; } | Obtiene o establece si se cargan los datos de celdas de forma asíncrona, se sugiere aplicarlo para una hoja con más de 10000 celdas. |
| [EnableClientColumnOperations](../../aspose.cells.gridweb/mainweb/enableclientcolumnoperations/) { get; set; } | Obtiene o establece si se habilitan las operaciones de columna del lado del cliente. |
| [EnableClientFreeze](../../aspose.cells.gridweb/mainweb/enableclientfreeze/) { get; set; } | Obtiene o establece si se habilitan las operaciones de congelación del lado del cliente. |
| [EnableClientMergeOperations](../../aspose.cells.gridweb/mainweb/enableclientmergeoperations/) { get; set; } | Obtiene o establece si se habilitan las operaciones de fusión del lado del cliente. |
| [EnableClientResizeColumnRow](../../aspose.cells.gridweb/mainweb/enableclientresizecolumnrow/) { get; set; } | Obtiene o establece si se habilita el redimensionamiento de columnas y filas del lado del cliente. |
| [EnableClientRowOperations](../../aspose.cells.gridweb/mainweb/enableclientrowoperations/) { get; set; } | Obtiene o establece si se habilitan las operaciones de fila del lado del cliente. |
| [EnableDoubleClickEvent](../../aspose.cells.gridweb/mainweb/enabledoubleclickevent/) { get; set; } | Obtiene o establece si se habilita el evento de doble clic del lado del cliente. |
| [EnableMetalLightEffect](../../aspose.cells.gridweb/mainweb/enablemetallighteffect/) { get; set; } | Obtiene o establece si se aplica el efecto de luz metálica. |
| [EnablePaging](../../aspose.cells.gridweb/mainweb/enablepaging/) { get; set; } | Obtiene o establece si se habilita el modo de paginación del control. |
| [EnableStyleDialogbox](../../aspose.cells.gridweb/mainweb/enablestyledialogbox/) { get; set; } | Obtiene o establece si se habilita el cuadro de diálogo de estilo del lado del cliente. |
| [FilteredPaging](../../aspose.cells.gridweb/mainweb/filteredpaging/) { get; set; } | Obtiene o establece si se habilita la paginación después de filtrar los datos; tendrá efecto cuando EnablePaging sea verdadero. |
| [ForceValidation](../../aspose.cells.gridweb/mainweb/forcevalidation/) { get; set; } | Obtiene o establece si se fuerza la validación del lado del cliente. |
| [FrameTableStyle](../../aspose.cells.gridweb/mainweb/frametablestyle/) { get; set; } | Obtiene o establece el estilo de marco del control. |
| [GoonDefaultSaveOperation](../../aspose.cells.gridweb/mainweb/goondefaultsaveoperation/) { get; set; } | Obtiene o establece si GridWeb realizará la operación de guardado predeterminada, el valor predeterminado es verdadero. |
| [HeaderBarHeight](../../aspose.cells.gridweb/mainweb/headerbarheight/) { get; set; } | Obtiene o establece la altura (System.Web.UI.WebControl.Unit) de la barra de encabezado superior del control. |
| [HeaderBarStyle](../../aspose.cells.gridweb/mainweb/headerbarstyle/) { get; set; } | Obtiene o establece el estilo de la barra de encabezado. |
| [HeaderBarTableStyle](../../aspose.cells.gridweb/mainweb/headerbartablestyle/) { get; set; } | Obtiene o establece el estilo de la barra de encabezado del control. |
| [HeaderBarWidth](../../aspose.cells.gridweb/mainweb/headerbarwidth/) { get; set; } | Obtiene o establece el ancho( System.Web.UI.WebControl.Unit ) o la barra de encabezado izquierda del control. |
| override [Height](../../aspose.cells.gridweb/mainweb/height/) { get; set; } | Obtiene o establece la altura( System.Web.UI.WebControl.Unit ) del control. |
| [IgnoreStyleWithNoData](../../aspose.cells.gridweb/mainweb/ignorestylewithnodata/) { get; set; } | Obtiene o establece si GridWeb ignora la visualización de filas o columnas que no contienen valores de celda pero están estilizadas. Si se establece en true, el rendimiento será mejor. El valor predeterminado es false, lo que significa que si la última fila/columna consecutiva no tiene valores de celda pero está estilizada, aún se mostrará. Esta opción solo es válida cuando EnableAsync es false. Esta opción no tiene efecto cuando EnableAsync es true, lo que significa que GridWeb mostrará todas las filas/columnas con estilo. |
| [IsCalculateFormula](../../aspose.cells.gridweb/mainweb/iscalculateformula/) { get; set; } | Obtiene o establece si se debe calcular la fórmula después de que cambie el valor de la celda o después de importar el archivo. El valor predeterminado es true. |
| [IsPostBack](../../aspose.cells.gridweb/mainweb/ispostback/) { get; } | Obtiene un valor que indica si gridweb se está cargando en respuesta a un postback del cliente, o si se está cargando y accediendo por primera vez. |
| [LoadOptions](../../aspose.cells.gridweb/mainweb/loadoptions/) { get; set; } | Representa las opciones de carga para GridWeb. |
| [MaxColumn](../../aspose.cells.gridweb/mainweb/maxcolumn/) { get; set; } | Obtiene o establece el índice máximo de columna a mostrar (basado en cero) de la hoja web. El control utiliza el valor mayor entre MaxColumn y la columna máxima de los datos de la hoja. |
| [MaxRow](../../aspose.cells.gridweb/mainweb/maxrow/) { get; set; } | Obtiene o establece el índice máximo de fila a mostrar (basado en cero) de la hoja web. El control utiliza el valor mayor entre MaxRow y la fila máxima de los datos de la hoja. |
| [Message](../../aspose.cells.gridweb/mainweb/message/) { get; set; } | Obtiene o establece el mensaje para la cuadrícula. |
| [MinColumn](../../aspose.cells.gridweb/mainweb/mincolumn/) { get; set; } | Obtiene o establece el índice mínimo de columna a mostrar (basado en cero) de la hoja web. El control utiliza el valor menor entre MinColumn y la columna mínima de los datos de la hoja. |
| [MinRow](../../aspose.cells.gridweb/mainweb/minrow/) { get; set; } | Obtiene o establece el índice mínimo de fila a mostrar (basado en cero) de la hoja web. El control utiliza el valor menor entre MinRow y la fila mínima de los datos de la hoja. |
| [ModifiedCells](../../aspose.cells.gridweb/mainweb/modifiedcells/) { get; } | Obtiene la colección de celdas modificadas por el cliente. |
| [NeedRenderGroupRows](../../aspose.cells.gridweb/mainweb/needrendergrouprows/) { get; set; } | Obtiene o establece si se muestran los grouprows . |
| [NoHScroll](../../aspose.cells.gridweb/mainweb/nohscroll/) { get; set; } | Obtiene o establece un valor que indica si la barra de desplazamiento horizontal está oculta. |
| [NoScroll](../../aspose.cells.gridweb/mainweb/noscroll/) { get; set; } | Obtiene o establece si se muestra la barra de desplazamiento . |
| [NoVScroll](../../aspose.cells.gridweb/mainweb/novscroll/) { get; set; } | Obtiene o establece un valor que indica si la barra de desplazamiento vertical está oculta. |
| [OnAjaxCallFinishedClientFunction](../../aspose.cells.gridweb/mainweb/onajaxcallfinishedclientfunction/) { get; set; } | Obtiene o establece el nombre de la función del lado del cliente que se llamará cuando la llamada ajax haya finalizado. La función del cliente debe declararse así: function GridAjaxcallFinished() { alert(this.id+" ajaxcall finished "); }Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de la cuadrícula que dispara el evento. |
| [OnCellErrorClientFunction](../../aspose.cells.gridweb/mainweb/oncellerrorclientfunction/) { get; set; } | Obtiene o establece el nombre de la función del lado del cliente que se llamará cuando falle la validación de una celda. La función del cliente debe declararse así: function MyOnCellError(cell) { alert(this.getCellValueByCell(cell)); }Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de la cuadrícula que dispara el evento. |
| [OnCellSelectedAjaxCallBackClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedajaxcallbackclientfunction/) { get; set; } | Obtiene o establece la función del lado del cliente que se llamará cuando se seleccione una celda. La función del cliente debe declararse así: function MyOnSelectCellAjaxCallBack(cell,customerdata) { }Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de la cuadrícula que dispara el evento. |
| [OnCellSelectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedclientfunction/) { get; set; } | Obtiene o establece la función del lado del cliente que se llamará cuando se seleccione una celda. La función del cliente debe declararse así: function MyOnSelectCell(cell) { GridWeb1.setCellValueByCell(cell, "test"); }Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de la cuadrícula que dispara el evento. |
| [OnCellUnselectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellunselectedclientfunction/) { get; set; } | Obtiene o establece la función del lado del cliente que se llamará cuando se deseleccione una celda. La función del cliente debe declararse así: function MyOnUnselectCell(cell) { this.setCellValueByCell(cell, "test"); }Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de la cuadrícula que dispara el evento. |
| [OnCellUpdatedClientFunction](../../aspose.cells.gridweb/mainweb/oncellupdatedclientfunction/) { get; set; } | Obtiene o establece el nombre de la función del lado del cliente que se llamará cuando se actualice el valor de una celda. La función del cliente debe declararse así: function MyOnCellUpdated(cell) { alert(this.getCellValueByCell(cell)); }Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de la cuadrícula que dispara el evento. |
| [OnContextMenuShowClientFunction](../../aspose.cells.gridweb/mainweb/oncontextmenushowclientfunction/) { get; set; } | Obtiene o establece la función del lado del cliente que se llamará cuando se muestre el menú contextual. La función del cliente debe declararse así: function onContextMenuShow() { var menu = event.srcElement; menu.setItemVisibility("Delete", "block"); menu.setItemVisibility("Update", "none"); }Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento. |
| [OnDoubleClickCellClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickcellclientfunction/) { get; set; } | Obtiene o establece la función del lado del cliente que se llamará cuando una celda se haga doble clic. La función del cliente debe declararse así: function MyOnDoubleClickCell(cell) { this.setCellValueByCell(cell, "test"); }Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento. |
| [OnDoubleClickRowClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickrowclientfunction/) { get; set; } | Obtiene o establece la función del lado del cliente que se llamará cuando una fila se haga doble clic. La función del cliente debe declararse así: function MyOnRowDoubleClick(row) { alert(row); }Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento. |
| [OnGridInitClientFunction](../../aspose.cells.gridweb/mainweb/ongridinitclientfunction/) { get; set; } | Obtiene o establece el nombre de la función del lado del cliente que se llamará cuando la cuadrícula se inicialice. La función del cliente debe declararse así: function MyOnGridInit(grid) { alert("The grid is initialized: " + grid.id); }Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento. |
| [OnlyAuto](../../aspose.cells.gridweb/mainweb/onlyauto/) { get; set; } | Obtiene o establece si solo se ajustan las filas cuya altura no está personalizada, el valor predeterminado es false |
| [OnPageChangeClientFunction](../../aspose.cells.gridweb/mainweb/onpagechangeclientfunction/) { get; set; } | Obtiene o establece la función del lado del cliente que se llamará después de cambiar el índice de página. Solo tiene efecto cuando EnablePaging es true. La función del cliente debe declararse así: function MyOnPageChange(index) { console.log("current page is:"+index); }Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento. |
| [OnPageSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onpagesubmitclientfunction/) { get; set; } | Obtiene o establece la función del cliente que se llamará antes de que la página se envíe del lado del cliente. |
| [OnShapeSelectedClientFunction](../../aspose.cells.gridweb/mainweb/onshapeselectedclientfunction/) { get; set; } | Obtiene o establece la función del lado del cliente que se llamará cuando se seleccione una forma. La función del cliente debe declararse así: function MyOnSelectShape(shape) { var name=shape.getAttribute("namevalue") var text=shape.getAttribute("textvalue") var value=shape.getAttribute("controlvalue") var type=shape.getAttribute("msotype") }Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento. |
| [OnSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onsubmitclientfunction/) { get; set; } | Obtiene o establece la función del cliente que se llamará antes de que el control se envíe del lado del cliente. La función del cliente debe declararse así: function MyOnSubmit(arg, cancelEdit) { return true;} El parámetro arg es el argumento de envío, contiene el comando que se enviará al servidor. cancelEdit es un valor booleano que indica si el control ha descartado la entrada del usuario antes del envío. El control continuará enviando si la función devuelve true. Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento. |
| [PageSize](../../aspose.cells.gridweb/mainweb/pagesize/) { get; set; } | Obtiene o establece el tamaño de página en modo de paginación. |
| [PresetStyle](../../aspose.cells.gridweb/mainweb/presetstyle/) { get; set; } | Obtiene o establece el estilo predefinido. |
| [RefreshValidation](../../aspose.cells.gridweb/mainweb/refreshvalidation/) { get; set; } | Obtiene o establece si se actualiza el valor de validación después de que cambie el valor de la celda. |
| [RenderHiddenRow](../../aspose.cells.gridweb/mainweb/renderhiddenrow/) { get; set; } | Obtiene o establece si la fila oculta se renderiza en GridControl, el valor predeterminado es false. Si necesita volver a mostrar la fila oculta más tarde, debe establecerlo en true. |
| [RowHeightForCSV](../../aspose.cells.gridweb/mainweb/rowheightforcsv/) { get; set; } | Obtenga o establezca el valor de la altura de fila en puntos para el archivo csv, el valor predeterminado es 14.5. |
| [ScrollBarArrowColor](../../aspose.cells.gridweb/mainweb/scrollbararrowcolor/) { get; set; } | Especifica el color del botón de flecha de la barra de desplazamiento. |
| [ScrollBarBaseColor](../../aspose.cells.gridweb/mainweb/scrollbarbasecolor/) { get; set; } | Especifica el color de la barra de desplazamiento del control. |
| [SelectCellBgColor](../../aspose.cells.gridweb/mainweb/selectcellbgcolor/) { get; set; } | Especifica el color de fondo de las celdas seleccionadas en el rango de selección múltiple. |
| [SelectCellColor](../../aspose.cells.gridweb/mainweb/selectcellcolor/) { get; set; } | Especifica el color de las celdas seleccionadas en el rango de selección múltiple. |
| [SessionMode](../../aspose.cells.gridweb/mainweb/sessionmode/) { get; set; } | Obtiene o establece el modo de sesión de la cuadrícula. |
| [SessionStorePath](../../aspose.cells.gridweb/mainweb/sessionstorepath/) { get; set; } | Obtiene o establece la ruta de almacenamiento de caché de sesión cuando el modo de sesión es File o ViewState, etc.: gridweb.SessionStorePath="c:/mytempdir/session"; entonces almacenará los datos de sesión en c:/mytempdir/session |
| [Settings](../../aspose.cells.gridweb/mainweb/settings/) { get; set; } | Representa la configuración del libro de trabajo. |
| [ShowAddButton](../../aspose.cells.gridweb/mainweb/showaddbutton/) { get; set; } | Obtiene o establece si se muestra el botón de agregar hoja de cálculo. |
| [ShowBottomBar](../../aspose.cells.gridweb/mainweb/showbottombar/) { get; set; } | Especifica si se muestra la barra de comandos (incluye barra de comandos y barra de pestañas) en la parte inferior del control. |
| [ShowCellEditBox](../../aspose.cells.gridweb/mainweb/showcelleditbox/) { get; set; } | Indica si Gridweb muestra la barra de herramientas de cuadro de edición como en MS-EXCEL. Si está habilitado, se mostrará un cuadro de edición para la celda actual en Gridweb. Si habilitamos esta función, necesitamos importar la biblioteca jquery js en sus archivos aspx para soportar esta nueva característica. Cualquier versión reciente de jquery está bien, etc. |
| [ShowCommandBarAtTop](../../aspose.cells.gridweb/mainweb/showcommandbarattop/) { get; set; } | Especifica si se muestra la barra de comandos (incluye barra de comandos y barra de pestañas) en la parte superior del control. |
| [ShowContextMenu](../../aspose.cells.gridweb/mainweb/showcontextmenu/) { get; set; } | Obtiene o establece si se muestra el menú contextual. El valor predeterminado es verdadero. |
| [ShowDefaultGridLine](../../aspose.cells.gridweb/mainweb/showdefaultgridline/) { get; set; } | Obtiene o establece si se muestran las líneas de cuadrícula predeterminadas de las celdas. |
| [ShowHeaderBar](../../aspose.cells.gridweb/mainweb/showheaderbar/) { get; set; } | Obtiene o establece si se muestra la barra de encabezado |
| [ShowLoading](../../aspose.cells.gridweb/mainweb/showloading/) { get; set; } | Especifica si se muestra un cuadro de diálogo de carga mientras se realiza el postback al servidor. |
| [ShowLoadingPosition](../../aspose.cells.gridweb/mainweb/showloadingposition/) { get; set; } | Especifica la posición izquierda, superior (en px) para mostrar el cuadro de diálogo de carga durante el postback al servidor, etc. 100,200 indica que la posición izquierda y superior del cuadro de diálogo de carga es 100px,200px. |
| [ShowSaveButton](../../aspose.cells.gridweb/mainweb/showsavebutton/) { get; set; } | Obtiene o establece si se muestra el botón de guardar. |
| [ShowSubmitButton](../../aspose.cells.gridweb/mainweb/showsubmitbutton/) { get; set; } | Obtiene o establece si se muestra el botón de enviar. |
| [ShowTabBar](../../aspose.cells.gridweb/mainweb/showtabbar/) { get; set; } | Obtiene o establece si se muestra la barra de pestañas. |
| [ShowTabNavigation](../../aspose.cells.gridweb/mainweb/showtabnavigation/) { get; set; } | Obtiene o establece si el botón de navegación de pestañas se muestra, el valor predeterminado es verdadero. |
| [ShowUndoButton](../../aspose.cells.gridweb/mainweb/showundobutton/) { get; set; } | Obtiene o establece si se muestra el botón de deshacer. |
| [SpanWrap](../../aspose.cells.gridweb/mainweb/spanwrap/) { get; set; } | Especifica si se ajusta el contenido en el rango de celdas. El valor predeterminado es verdadero. |
| [TabStyle](../../aspose.cells.gridweb/mainweb/tabstyle/) { get; set; } | Obtiene o establece el estilo de la barra de pestañas. |
| [UseClientPageHeight](../../aspose.cells.gridweb/mainweb/useclientpageheight/) { get; set; } | Obtiene o establece si gridweb usa la altura de la página del cliente como altura del control, adecuado cuando se establece Height="100%", el valor predeterminado es falso. |
| [ViewPanelScrollLeft](../../aspose.cells.gridweb/mainweb/viewpanelscrollleft/) { get; set; } | Obtiene o establece la posición de la barra de desplazamiento del panel de vista de la cuadrícula. |
| [ViewPanelScrollTop](../../aspose.cells.gridweb/mainweb/viewpanelscrolltop/) { get; set; } | Obtiene o establece la posición de la barra de desplazamiento del panel de vista de la cuadrícula. |
| [ViewTableStyle](../../aspose.cells.gridweb/mainweb/viewtablestyle/) { get; set; } | Obtiene o establece el estilo del panel de vista de datos. |
| [WebWorksheets](../../aspose.cells.gridweb/mainweb/webworksheets/) { get; } |  |
| override [Width](../../aspose.cells.gridweb/mainweb/width/) { get; set; } | Obtiene o establece el ancho (System.Web.UI.WebControl.Unit) del control. |
| [WorkSheets](../../aspose.cells.gridweb/mainweb/worksheets/) { get; } | Obtiene o establece la colección de hojas de cálculo. |
| [XhtmlMode](../../aspose.cells.gridweb/mainweb/xhtmlmode/) { get; set; } | Obtiene o establece si se usa el estilo XHTML, el valor predeterminado es verdadero. |
| static [DPI](../../aspose.cells.gridweb/mainweb/dpi/) { get; set; } | Obtiene / establece el DPI de la máquina. |
| static [PictureCachePath](../../aspose.cells.gridweb/mainweb/picturecachepath/) { get; set; } | Obtiene o establece la ruta de almacenamiento de imágenes para el libro de trabajo, todas las formas e imágenes se almacenarán en este directorio, la ruta predeterminada es acwcache bajo el Directorio Base de la aplicación actual; los usuarios deben implementar un servicio programado para limpiar los archivos que estén fuera del tiempo de sesión. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CalculateFormula](../../aspose.cells.gridweb/mainweb/calculateformula/)() | Calcula el resultado de las fórmulas. |
| override [DataBind](../../aspose.cells.gridweb/mainweb/databind/)() | Vincula el control y todos sus controles secundarios a su origen de datos. |
| override [Dispose](../../aspose.cells.gridweb/mainweb/dispose/)() |  |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile)(Stream) | Importa desde un flujo de archivo Excel, incluyendo flujo de archivo en disco o flujo de memoria. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile_2)(string) | Importa desde un archivo Excel. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile_1)(Stream, string) | Importa desde un flujo de archivo Excel, incluyendo flujo de archivo en disco o flujo de memoria. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile_3)(string, string) | Importa desde un archivo Excel. |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile/#loadcsvfile)(Stream) | Carga datos desde un flujo de archivo CSV. |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile/#loadcsvfile_1)(string) | Carga datos desde un archivo CSV. |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile/#loadhtmlfile)(Stream) | Carga datos desde un flujo de archivo HTML. |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile/#loadhtmlfile_1)(string) | Carga datos desde un archivo HTML. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile/#loadspreadsheetmlfile)(Stream) | Carga datos desde un flujo de archivo SpreadSheetML. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile/#loadspreadsheetmlfile_1)(string) | Carga datos desde un archivo SpreadSheetML. |
| [RefreshChartShape](../../aspose.cells.gridweb/mainweb/refreshchartshape/)() | Actualiza todas las imágenes de los gráficos para la hoja de cálculo activa. |
| override [RenderBeginTag](../../aspose.cells.gridweb/mainweb/renderbegintag/)(HtmlTextWriter) |  |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile/#savecsvfile)(Stream) | Guarda datos en un flujo de archivo CSV. |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile/#savecsvfile_1)(string) | Guarda datos en un archivo CSV. |
| [SaveCustomStyleFile](../../aspose.cells.gridweb/mainweb/savecustomstylefile/)(string) | Guarda los datos de estilo actuales del control en un archivo xml. Puede usarse para crear su archivo de estilo personalizado. |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile/#savehtmlfile)(Stream) | Guarda datos en un flujo de archivo HTML. |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile/#savehtmlfile_1)(string) | Guarda datos en un archivo HTML. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile/#savespreadsheetmlfile)(Stream) | Guarda datos en un flujo de archivo SpreadSheetML. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile/#savespreadsheetmlfile_1)(string) | Guarda datos en un archivo SpreadSheetML. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile)(Stream) | Guarda las hojas de cálculo en un archivo Excel. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_3)(string) | Guarda las hojas de cálculo en un archivo Excel con formato Excel 2003. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_1)(Stream, GridSaveFormat) | Guarda las hojas de cálculo en un archivo Excel. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_2)(Stream, GridSaveOptions) | Guarda las hojas de cálculo en un archivo Excel. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_4)(string, GridSaveFormat) | Guarda las hojas de cálculo en un archivo Excel. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_5)(string, GridSaveOptions) | Guarda las hojas de cálculo en un archivo Excel. |
| [SetCustomStyle](../../aspose.cells.gridweb/mainweb/setcustomstyle/)(Stream) | Establece el archivo de estilo personalizado desde un flujo, incluyendo flujo de archivo en disco o flujo de memoria. |

## Eventos

| Nombre | Descripción |
| --- | --- |
| event [AfterColumnFilter](../../aspose.cells.gridweb/mainweb/aftercolumnfilter/) | Ocurre después de que la columna se haya filtrado. |
| event [AjaxCallFinished](../../aspose.cells.gridweb/mainweb/ajaxcallfinished/) | Se dispara cuando la actualización ajax del control ha finalizado. (EnableAJAX debe estar configurado en true) |
| event [BeforeColumnFilter](../../aspose.cells.gridweb/mainweb/beforecolumnfilter/) | Ocurre antes de que la columna sea filtrada. |
| event [CellClickOnAjax](../../aspose.cells.gridweb/mainweb/cellclickonajax/) | Ocurre cuando se hace clic en la celda, y es necesario hacer ajaxcallback para este evento. |
| event [CellClientUpdate](../../aspose.cells.gridweb/mainweb/cellclientupdate/) | Ocurre cuando se produce una actualización de celda del cliente. Cuando se dispara este evento, su parámetro e.Argument contiene el nombre del comando. |
| event [CellCommand](../../aspose.cells.gridweb/mainweb/cellcommand/) | Ocurre cuando se hace clic en el hipervínculo de comando de una celda. Cuando se dispara este evento, su parámetro e.Argument contiene el nombre del comando. |
| event [CellDoubleClick](../../aspose.cells.gridweb/mainweb/celldoubleclick/) | Ocurre cuando se hace doble clic en la celda. |
| event [CellError](../../aspose.cells.gridweb/mainweb/cellerror/) | Ocurre cuando hay un error en el valor de entrada de una celda. |
| event [CellModifiedOnAjax](../../aspose.cells.gridweb/mainweb/cellmodifiedonajax/) | Ocurre cuando la celda se modifica en ajaxcall. |
| event [ColumnDeleted](../../aspose.cells.gridweb/mainweb/columndeleted/) | Ocurre cuando el usuario elimina una columna del menú del lado del cliente. |
| event [ColumnDeleting](../../aspose.cells.gridweb/mainweb/columndeleting/) | Ocurre cuando el usuario intenta eliminar una columna del menú del lado del cliente. Puede manejar este evento y establecer el parámetro cancel en True para cancelar la operación de eliminación. |
| event [ColumnDoubleClick](../../aspose.cells.gridweb/mainweb/columndoubleclick/) | Ocurre cuando se hace doble clic en el encabezado de la columna. |
| event [ColumnInserted](../../aspose.cells.gridweb/mainweb/columninserted/) | Ocurre cuando el usuario inserta una columna desde el menú del lado del cliente. |
| event [CustomCommand](../../aspose.cells.gridweb/mainweb/customcommand/) | Ocurre cuando el usuario hace clic en un botón de comando personalizado. |
| event [LoadCustomData](../../aspose.cells.gridweb/mainweb/loadcustomdata/) | Se dispara cuando SessionMode del control está configurado en Custom y necesita cargar los datos de la hoja. Puede manejar este evento en modo Custom Session para cargar los datos de la hoja desde un archivo o base de datos. |
| event [PageIndexChanged](../../aspose.cells.gridweb/mainweb/pageindexchanged/) | Ocurre cuando el índice de página de la hoja del control cambia. |
| event [RowDeleted](../../aspose.cells.gridweb/mainweb/rowdeleted/) | Ocurre cuando el usuario ha eliminado una fila del menú del lado del cliente. |
| event [RowDeleting](../../aspose.cells.gridweb/mainweb/rowdeleting/) | Ocurre cuando el usuario intenta eliminar una fila del menú del lado del cliente. Puede manejar este evento y lanzar una excepción RejectDeleteException para cancelar la operación de eliminación. |
| event [RowDoubleClick](../../aspose.cells.gridweb/mainweb/rowdoubleclick/) | Ocurre cuando se hace doble clic en el encabezado de la fila. |
| event [RowInserted](../../aspose.cells.gridweb/mainweb/rowinserted/) | Ocurre cuando el usuario inserta una fila desde el menú del lado del cliente. |
| event [SaveCommand](../../aspose.cells.gridweb/mainweb/savecommand/) | Ocurre cuando se hace clic en el botón "save". |
| event [SheetAdded](../../aspose.cells.gridweb/mainweb/sheetadded/) | Ocurre cuando el usuario agrega una hoja de cálculo desde el menú de la barra de herramientas. |
| event [SheetDataUpdated](../../aspose.cells.gridweb/mainweb/sheetdataupdated/) | Ocurre cuando el control ha cargado los datos enviados y actualizado los datos de la hoja. |
| event [SheetTabClick](../../aspose.cells.gridweb/mainweb/sheettabclick/) | Ocurre cuando se hace clic en la pestaña de la hoja. |
| event [SubmitCommand](../../aspose.cells.gridweb/mainweb/submitcommand/) | Ocurre cuando se hace clic en el botón "submit". |
| event [UndoCommand](../../aspose.cells.gridweb/mainweb/undocommand/) | Ocurre cuando se hace clic en el botón "deshacer". |

### Ejemplos

```csharp
[C#]
	GridWeb GridWeb1 = new GridWeb();
//realiza tu negocio
```

### Ver también

* class [ExtWebControl](../extwebcontrol/)
* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


