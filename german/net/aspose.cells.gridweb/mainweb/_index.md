---
title: MainWeb
second_title: Aspose.Cells für .NET-API-Referenz
description: Übergeordnete Klasse des GridWeb-Steuerelements. Nur zur internen Verwendung.
type: docs
weight: 850
url: /de/net/aspose.cells.gridweb/mainweb/
---
## MainWeb class

Übergeordnete Klasse des GridWeb-Steuerelements. Nur zur internen Verwendung.

```csharp
public class MainWeb : ExtWebControl, INamingContainer, IPostBackDataHandler, 
    IPostBackEventHandler, ISerializable
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [MainWeb](mainweb)() | Default_Constructor |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ActiveCell](../../aspose.cells.gridweb/mainweb/activecell) { get; set; } | Ruft die aktive Zelle des aktuellen Blatts ab oder setzt sie. Seit Version 1.9.0.1 schreibbar geändert. |
| [ActiveCellBgColor](../../aspose.cells.gridweb/mainweb/activecellbgcolor) { get; set; } | Gibt die Hintergrundfarbe der aktiven Zelle an. |
| [ActiveCellColor](../../aspose.cells.gridweb/mainweb/activecellcolor) { get; set; } | Gibt die Farbe der aktiven Zelle an. |
| [ActiveHeaderBgColor](../../aspose.cells.gridweb/mainweb/activeheaderbgcolor) { get; set; } | Gibt die Hintergrundfarbe der aktiven Zeilen-/Spaltenüberschrift an. |
| [ActiveHeaderColor](../../aspose.cells.gridweb/mainweb/activeheadercolor) { get; set; } | Gibt die Farbe der aktiven Zeilen-/Spaltenüberschrift an. |
| [ActiveSheet](../../aspose.cells.gridweb/mainweb/activesheet) { get; } | Ruft das aktive Blatt ab |
| [ActiveSheetIndex](../../aspose.cells.gridweb/mainweb/activesheetindex) { get; set; } | Ruft den Index des aktiven Blatts ab oder legt ihn fest. Entspricht dem WebWorksheets.ActiveSheetIndex. |
| [ActiveTabStyle](../../aspose.cells.gridweb/mainweb/activetabstyle) { get; set; } | Gibt den Stil der aktiven Registerkarte an. |
| [ACWClientPath](../../aspose.cells.gridweb/mainweb/acwclientpath) { get; set; } | Ruft den Webpfad der Skript-/Bilddateien des Steuerelements ab oder setzt ihn. Beispiel: "http://localhost/acw_client". Sie können diesen Wert auch in der Datei web.config festlegen. Fügen Sie diesen Abschnitt zum Abschnitt &lt;configuration&gt; hinzu: &lt;App-Einstellungen&gt;&lt;add key="aspose.cells.gridweb.acw_client_path" value="/acw_client/" /&gt;&lt;/appEinstellungen&gt; |
| [ACWLanguageFileUrl](../../aspose.cells.gridweb/mainweb/acwlanguagefileurl) { get; set; } | Ruft die Web-URL der Sprachdatei des Steuerelements ab oder setzt sie. Beispiel: "/acw_client/lang_en.js". Standardmäßig wird eine eingebaute englische Datei verwendet. |
| [AutoRefreshChart](../../aspose.cells.gridweb/mainweb/autorefreshchart) { get; set; } | Ruft ab oder legt fest, ob das Diagrammbild aktualisiert wird, während der Zellenwert aktualisiert wird. Der Standardwert ist true |
| [BottomTableStyle](../../aspose.cells.gridweb/mainweb/bottomtablestyle) { get; set; } | Ruft den Stil der unteren Leiste des Steuerelements ab oder legt ihn fest. |
| [CurrentPageIndex](../../aspose.cells.gridweb/mainweb/currentpageindex) { get; set; } |  |
| [CustomCalculationEngine](../../aspose.cells.gridweb/mainweb/customcalculationengine) { get; set; } | Stellt das benutzerdefinierte Berechnungsmodul des Benutzers dar, um das standardmäßige Berechnungsmodul von Aspose.Cells zu erweitern. |
| [CustomCommandButtons](../../aspose.cells.gridweb/mainweb/customcommandbuttons) { get; } |  |
| [CustomStyleFileName](../../aspose.cells.gridweb/mainweb/customstylefilename) { get; set; } | Ruft den Namen der benutzerdefinierten Stildatei ab oder legt ihn fest. |
| [DefaultFontName](../../aspose.cells.gridweb/mainweb/defaultfontname) { get; set; } | Ruft den Standardschriftnamen des Steuerelements ab oder legt ihn fest. |
| [DefaultFontSize](../../aspose.cells.gridweb/mainweb/defaultfontsize) { get; set; } | Ruft die Standardschriftgröße des Steuerelements ab oder legt sie fest. |
| [DefaultGridLineColor](../../aspose.cells.gridweb/mainweb/defaultgridlinecolor) { get; set; } | Ruft die Farbe der Standardrasterlinie ab oder legt sie fest. |
| [DisplayCellTip](../../aspose.cells.gridweb/mainweb/displaycelltip) { get; set; } |  |
| [EditMode](../../aspose.cells.gridweb/mainweb/editmode) { get; set; } | Ruft den Bearbeitungsmodus des Steuerelements ab oder legt ihn fest. |
| [EnableAJAX](../../aspose.cells.gridweb/mainweb/enableajax) { get; set; } |  |
| [EnableAsync](../../aspose.cells.gridweb/mainweb/enableasync) { get; set; } | Ruft ab oder legt fest, ob Wägezellendaten asynchron übertragen werden, schlagen Sie vor, ein Blatt mit mehr als 10000 Zellen zu beantragen. |
| [EnableClientColumnOperations](../../aspose.cells.gridweb/mainweb/enableclientcolumnoperations) { get; set; } | Ruft ab oder legt fest, ob die clientseitigen Spaltenoperationen aktiviert werden sollen. |
| [EnableClientFreeze](../../aspose.cells.gridweb/mainweb/enableclientfreeze) { get; set; } | Ruft ab oder legt fest, ob die clientseitigen Sperrvorgänge aktiviert werden sollen. |
| [EnableClientMergeOperations](../../aspose.cells.gridweb/mainweb/enableclientmergeoperations) { get; set; } | Ruft ab oder legt fest, ob die clientseitigen Zusammenführungsvorgänge aktiviert werden sollen. |
| [EnableClientResizeColumnRow](../../aspose.cells.gridweb/mainweb/enableclientresizecolumnrow) { get; set; } | Ruft ab oder legt fest, ob die clientseitige Größenänderung von Spalte und Zeile aktiviert werden soll. |
| [EnableClientRowOperations](../../aspose.cells.gridweb/mainweb/enableclientrowoperations) { get; set; } | Ruft ab oder legt fest, ob die clientseitigen Zeilenoperationen aktiviert werden sollen. |
| [EnableDoubleClickEvent](../../aspose.cells.gridweb/mainweb/enabledoubleclickevent) { get; set; } | Ruft ab oder legt fest, ob das kundenseitige Doppelklickereignis aktiviert werden soll. |
| [EnableMetalLightEffect](../../aspose.cells.gridweb/mainweb/enablemetallighteffect) { get; set; } | Ruft ab oder legt fest, ob Metalllichteffekte angewendet werden sollen. |
| [EnablePaging](../../aspose.cells.gridweb/mainweb/enablepaging) { get; set; } | Ruft ab oder legt fest, ob der Paging-Modus des Steuerelements aktiviert werden soll. |
| [EnableStyleDialogbox](../../aspose.cells.gridweb/mainweb/enablestyledialogbox) { get; set; } | Ruft ab oder legt fest, ob das clientseitige Stildialogfeld aktiviert werden soll. |
| [FilteredPaging](../../aspose.cells.gridweb/mainweb/filteredpaging) { get; set; } | Ruft ab oder legt fest, ob das Paging nach gefilterten Daten aktiviert werden soll, wird wirksam, wenn EnablePaging wahr ist. |
| [ForceValidation](../../aspose.cells.gridweb/mainweb/forcevalidation) { get; set; } | Ruft ab oder legt fest, ob die kundenseitige Validierung erzwungen werden soll. |
| [FrameTableStyle](../../aspose.cells.gridweb/mainweb/frametablestyle) { get; set; } | Ruft den Rahmenstil des Steuerelements ab oder legt ihn fest. |
| [GoonDefaultSaveOperation](../../aspose.cells.gridweb/mainweb/goondefaultsaveoperation) { get; set; } | Ruft ab oder legt fest, ob GridWeb den Standardspeichervorgang durchführt, der Standardwert ist true. |
| [HeaderBarHeight](../../aspose.cells.gridweb/mainweb/headerbarheight) { get; set; } | Ruft die Höhe ( System.Web.UI.WebControl.Unit ) der oberen Kopfleiste des Steuerelements ab oder legt sie fest. |
| [HeaderBarStyle](../../aspose.cells.gridweb/mainweb/headerbarstyle) { get; set; } | Ruft den Stil der Kopfleiste ab oder legt ihn fest. |
| [HeaderBarTableStyle](../../aspose.cells.gridweb/mainweb/headerbartablestyle) { get; set; } | Ruft den Kopfleistenstil des Steuerelements ab oder legt ihn fest. |
| [HeaderBarWidth](../../aspose.cells.gridweb/mainweb/headerbarwidth) { get; set; } | Ruft die Breite ( System.Web.UI.WebControl.Unit ) oder die linke Kopfzeile des Steuerelements ab oder legt sie fest. |
| override [Height](../../aspose.cells.gridweb/mainweb/height) { get; set; } | Ruft die Höhe ( System.Web.UI.WebControl.Unit ) des Steuerelements ab oder legt sie fest. |
| [IsCalculateFormula](../../aspose.cells.gridweb/mainweb/iscalculateformula) { get; set; } | Ruft ab oder legt fest, ob die Formel nach Zellwertänderungen oder nach dem Import einer Datei berechnet werden soll. Der Standardwert ist true. |
| [IsPostBack](../../aspose.cells.gridweb/mainweb/ispostback) { get; } | Ruft einen Wert ab, der angibt, ob Gridweb als Antwort auf ein Client-Postback geladen wird, oder ob es geladen und zum ersten Mal aufgerufen wird. |
| [LinksTable](../../aspose.cells.gridweb/mainweb/linkstable) { get; } |  |
| [MaxColumn](../../aspose.cells.gridweb/mainweb/maxcolumn) { get; set; } | Ruft den maximalen Anzeigespaltenindex (nullbasiert) des Webblatts ab oder legt diesen fest. Das Steuerelement verwendet den größeren Wert von MaxColumn und der maximalen Spalte von Blattdaten. |
| [MaxRow](../../aspose.cells.gridweb/mainweb/maxrow) { get; set; } | Ruft den maximalen Anzeigezeilenindex (nullbasiert) des Webblatts ab oder legt diesen fest. Das Steuerelement verwendet den größeren Wert von MaxRow und der maximalen Zeile der Blattdaten. |
| [Message](../../aspose.cells.gridweb/mainweb/message) { get; set; } |  |
| [MinColumn](../../aspose.cells.gridweb/mainweb/mincolumn) { get; set; } |  |
| [MinRow](../../aspose.cells.gridweb/mainweb/minrow) { get; set; } | Ruft den minimalen Anzeigezeilenindex (nullbasiert) des Webblatts ab oder legt diesen fest. Das Steuerelement verwendet den kleineren Wert von MinRow und die minimale Zeile der Blattdaten. |
| [ModifiedCells](../../aspose.cells.gridweb/mainweb/modifiedcells) { get; } | Ruft die Sammlung der Zellen ab, die vom Client geändert wurden. |
| [NeedRenderGroupRows](../../aspose.cells.gridweb/mainweb/needrendergrouprows) { get; set; } | Ruft ab oder legt fest, ob Gruppenzeilen angezeigt werden sollen . |
| [NoHScroll](../../aspose.cells.gridweb/mainweb/nohscroll) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob die horizontale Bildlaufleiste ausgeblendet ist. |
| [NoScroll](../../aspose.cells.gridweb/mainweb/noscroll) { get; set; } |  |
| [NoVScroll](../../aspose.cells.gridweb/mainweb/novscroll) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob die vertikale Bildlaufleiste ausgeblendet ist. |
| [OnAjaxCallFinishedClientFunction](../../aspose.cells.gridweb/mainweb/onajaxcallfinishedclientfunction) { get; set; } | Erhält oder setzt den Namen der clientseitigen Funktion, die aufgerufen werden soll, wenn Ajaxcall beendet ist. Die Client-Funktion sollte wie folgt deklariert werden: -Funktion GridAjaxcallFinished() { alert(this.id+" ajaxcall beendet "); } Hinweis: Sie können den "this"-Zeiger in der Client-Funktion verwenden, um auf das Grid-Steuerelement zu zeigen, das das Ereignis auslöst. |
| [OnCellErrorClientFunction](../../aspose.cells.gridweb/mainweb/oncellerrorclientfunction) { get; set; } | Ruft den clientseitigen Funktionsnamen ab oder legt ihn fest, der aufgerufen werden soll, wenn die Validierung einer Zelle fehlschlägt. Die Clientfunktion sollte wie folgt deklariert werden: Funktion MyOnCellError(Zelle) { alert(GridWeb1.getCellValueByCell(cell)); } Hinweis: Sie können den "this"-Zeiger in der Client-Funktion verwenden, um auf das Grid-Steuerelement zu zeigen, das das Ereignis auslöst. |
| [OnCellSelectedAjaxCallBackClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedajaxcallbackclientfunction) { get; set; } | Ruft die Client-seitige Funktion ab oder legt sie fest, die aufgerufen werden soll, wenn eine Zelle ausgewählt wird. Die Client-Funktion sollte wie folgt deklariert werden: Funktion MyOnSelectCellAjaxCallBack(cell,customerdata) { } Hinweis: Sie können den "this"-Zeiger in der Client-Funktion verwenden, um auf das Grid-Steuerelement zu zeigen, das das Ereignis auslöst. |
| [OnCellSelectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedclientfunction) { get; set; } | Ruft die Client-seitige Funktion ab oder legt sie fest, die aufgerufen werden soll, wenn eine Zelle ausgewählt wird. Die Client-Funktion sollte wie folgt deklariert werden: Funktion MyOnSelectCell(Zelle) { GridWeb1.setCellValueByCell(cell, "test"); } Hinweis: Sie können den "this"-Zeiger in der Client-Funktion verwenden, um auf das Grid-Steuerelement zu zeigen, das das Ereignis auslöst. |
| [OnCellUnselectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellunselectedclientfunction) { get; set; } | Ruft die Client-seitige Funktion ab oder legt sie fest, die aufgerufen werden soll, wenn eine Zelle nicht ausgewählt ist. Die Client-Funktion sollte wie folgt deklariert werden: Funktion MyOnUnselectCell(Zelle) { GridWeb1.setCellValueByCell(cell, "test"); } Hinweis: Sie können den "this"-Zeiger in der Client-Funktion verwenden, um auf das Grid-Steuerelement zu zeigen, das das Ereignis auslöst. |
| [OnCellUpdatedClientFunction](../../aspose.cells.gridweb/mainweb/oncellupdatedclientfunction) { get; set; } | Ruft den Namen der clientseitigen Funktion ab oder legt ihn fest, der aufgerufen werden soll, wenn der Wert einer Zelle aktualisiert wird. Die Clientfunktion sollte wie folgt deklariert werden: Funktion MyOnCellUpdated(Zelle) { alert(this.getCellValueByCell(cell)); } Hinweis: Sie können den "this"-Zeiger in der Client-Funktion verwenden, um auf das Grid-Steuerelement zu zeigen, das das Ereignis auslöst. |
| [OnContextMenuShowClientFunction](../../aspose.cells.gridweb/mainweb/oncontextmenushowclientfunction) { get; set; } | Ruft die Client-seitige Funktion ab oder legt sie fest, die aufgerufen werden soll, wenn das Kontextmenü angezeigt wird. Die Client-Funktion sollte wie folgt deklariert werden: Funktion onContextMenuShow() { var menu = event.srcElement; menu.setItemVisibility("Löschen", "blockieren"); menu.setItemVisibility("Update", "none"); } Hinweis: Sie können den "this"-Zeiger in der Client-Funktion verwenden, um auf das Grid-Steuerelement zu zeigen, das das Ereignis auslöst. |
| [OnDoubleClickCellClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickcellclientfunction) { get; set; } | Ruft die Client-seitige Funktion ab oder legt sie fest, die aufgerufen werden soll, wenn auf eine Zelle doppelgeklickt wird. Die Client-Funktion sollte wie folgt deklariert werden: Funktion MyOnDoubleClickCell(Zelle) { GridWeb1.setCellValueByCell(cell, "test"); } Hinweis: Sie können den "this"-Zeiger in der Client-Funktion verwenden, um auf das Grid-Steuerelement zu zeigen, das das Ereignis auslöst. |
| [OnDoubleClickRowClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickrowclientfunction) { get; set; } | Ruft die Client-seitige Funktion ab oder legt sie fest, die aufgerufen werden soll, wenn auf eine Zeile doppelgeklickt wird. Die Client-Funktion sollte wie folgt deklariert werden: Funktion MyOnRowDoubleClick(Zeile) { Warnung (Zeile); } Hinweis: Sie können den "this"-Zeiger in der Client-Funktion verwenden, um auf das Grid-Steuerelement zu zeigen, das das Ereignis auslöst. |
| [OnGridInitClientFunction](../../aspose.cells.gridweb/mainweb/ongridinitclientfunction) { get; set; } | Erhält oder setzt den Namen der clientseitigen Funktion, die aufgerufen werden soll, wenn das Grid initialisiert wird. Die Client-Funktion sollte wie folgt deklariert werden: Funktion MyOnGridInit(Gitter) { alert("Das Raster wird initialisiert: " + grid.id); } Hinweis: Sie können den "this"-Zeiger in der Client-Funktion verwenden, um auf das Grid-Steuerelement zu zeigen, das das Ereignis auslöst. |
| [OnlyAuto](../../aspose.cells.gridweb/mainweb/onlyauto) { get; set; } | Ruft ab oder legt fest, ob nur die Zeilen passen, deren Höhe nicht angepasst ist, der Standardwert ist false |
| [OnPageChangeClientFunction](../../aspose.cells.gridweb/mainweb/onpagechangeclientfunction) { get; set; } | Ruft die clientseitige Funktion ab oder legt sie fest, die nach dem Ändern des Seitenindex aufgerufen werden soll. Nur wirksam, wenn EnablePaging wahr ist. Die Client-Funktion sollte wie folgt deklariert werden: Funktion MyOnPageChange(Index) { console.log("aktuelle Seite ist:"+index); } Hinweis: Sie können den "this"-Zeiger in der Client-Funktion verwenden, um auf das Grid-Steuerelement zu zeigen, das das Ereignis auslöst. |
| [OnPageSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onpagesubmitclientfunction) { get; set; } | Ruft die Clientfunktion ab oder legt sie fest, die aufgerufen werden soll, bevor die Seite auf der Clientseite übermittelt wird. |
| [OnShapeSelectedClientFunction](../../aspose.cells.gridweb/mainweb/onshapeselectedclientfunction) { get; set; } | Ruft die Client-seitige Funktion ab oder legt sie fest, die aufgerufen werden soll, wenn eine Form ausgewählt wird. Die Client-Funktion sollte wie folgt deklariert werden: Funktion MyOnSelectShape(Form) { var name=shape.getAttribute("namevalue") var text=shape.getAttribute("Textwert") var value=shape.getAttribute("controlvalue") var type=shape.getAttribute("msotype") } Hinweis: Sie können den "this"-Zeiger in der Client-Funktion verwenden, um auf das Grid-Steuerelement zu zeigen, das das Ereignis auslöst. |
| [OnSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onsubmitclientfunction) { get; set; } | Ruft die Client-Funktion ab oder legt sie fest, die aufgerufen werden soll, bevor das Steuerelement auf der Client-Seite übermittelt wird. Die Client-Funktion sollte wie folgt deklariert werden: -Funktion MyOnSubmit(arg, cancelEdit) { gib true zurück;} Das arg ist das Submit-Argument und enthält den Befehl, der an den Server gesendet werden soll. Der CancelEdit ist ein boolescher Wert, der angibt, ob das Steuerelement die Benutzereingabe vor dem Submit verworfen hat. Das Steuerelement wird mit dem Senden fortfahren, wenn die Funktion wahr zurückgibt.  Hinweis: Sie können den "this"-Zeiger in der Client-Funktion verwenden, um auf das Grid-Steuerelement zu zeigen, das das Ereignis auslöst. |
| [PageSize](../../aspose.cells.gridweb/mainweb/pagesize) { get; set; } | Ruft die Seitengröße im Paging-Modus ab oder legt sie fest. |
| [PicturesTable](../../aspose.cells.gridweb/mainweb/picturestable) { get; } |  |
| [PresetStyle](../../aspose.cells.gridweb/mainweb/presetstyle) { get; set; } | Ruft den voreingestellten Stil ab oder legt ihn fest. |
| [RefreshValidation](../../aspose.cells.gridweb/mainweb/refreshvalidation) { get; set; } | Ruft ab oder legt fest, ob der Validierungswert nach Änderungen des Zellenwerts aktualisiert werden soll. |
| [RenderHiddenRow](../../aspose.cells.gridweb/mainweb/renderhiddenrow) { get; set; } | Ruft ab oder legt fest, ob die ausgeblendete Zeile in GridControl gerendert wird, der Standardwert ist „false“. Wenn Sie die ausgeblendete Zeile später wieder einblenden müssen, müssen Sie sie auf „true“ setzen |
| [ScrollBarArrowColor](../../aspose.cells.gridweb/mainweb/scrollbararrowcolor) { get; set; } | Gibt die Farbe der Pfeilschaltfläche der Bildlaufleiste an. |
| [ScrollBarBaseColor](../../aspose.cells.gridweb/mainweb/scrollbarbasecolor) { get; set; } | Gibt die Farbe der Bildlaufleiste des Steuerelements an. |
| [SelectCellBgColor](../../aspose.cells.gridweb/mainweb/selectcellbgcolor) { get; set; } | Gibt die Hintergrundfarbe der ausgewählten Zellen im Mehrfachauswahlbereich an. |
| [SelectCellColor](../../aspose.cells.gridweb/mainweb/selectcellcolor) { get; set; } | Gibt die Farbe der ausgewählten Zellen im Mehrfachauswahlbereich an. |
| [SessionLoaded](../../aspose.cells.gridweb/mainweb/sessionloaded) { get; set; } |  |
| [SessionMode](../../aspose.cells.gridweb/mainweb/sessionmode) { get; set; } | Ruft den Sitzungsmodus des Rasters ab oder legt ihn fest. Es gibt 4 Arten von Sitzungsmodi: 1. Sitzung (Standard): Systemsitzung zum Speichern von Blattdaten verwenden. Im Allgemeinen verwendet asp.net den InProc-Sitzungsstatus. Das Grid unterstützt auch „StateServer“-Out-Prozesssitzungsstatus und SQLServer-Sitzungsstatus. 2. ViewState: Verwenden Sie den Viewstate der Seite, um Blattdaten zu speichern. 3. Benutzerdefiniert: Verwenden Sie LoadCustomData- und SheetDataUpdated-Ereignisse zum Speichern/Wiederherstellen von Blattdaten. 4. Datei: Blattdaten in SessionStorePath speichern/wiederherstellen. |
| [SessionSaved](../../aspose.cells.gridweb/mainweb/sessionsaved) { get; set; } |  |
| [SessionStorePath](../../aspose.cells.gridweb/mainweb/sessionstorepath) { get; set; } | Ruft den Sitzungs-Cache-Speicherpfad ab oder legt ihn fest, wenn der Sitzungsmodus File oder ViewState ist, usw.: gridweb.SessionStorePath="c:/mytempdir/session"; dann werden Sitzungsdaten in c:/mytempdir/session gespeichert |
| [Settings](../../aspose.cells.gridweb/mainweb/settings) { get; set; } | Stellt die Arbeitsmappeneinstellungen dar. |
| [ShapesTable](../../aspose.cells.gridweb/mainweb/shapestable) { get; } |  |
| [ShowAddButton](../../aspose.cells.gridweb/mainweb/showaddbutton) { get; set; } | Ruft ab oder legt fest, ob die Schaltfläche „Arbeitsblatt hinzufügen“ angezeigt werden soll. |
| [ShowBottomBar](../../aspose.cells.gridweb/mainweb/showbottombar) { get; set; } |  |
| [ShowCellEditBox](../../aspose.cells.gridweb/mainweb/showcelleditbox) { get; set; } | ob Gridweb Bearbeitungsfeld-Symbolleiste wie in MS-EXCEL anzeigt. Wenn aktiviert, wird ein Bearbeitungsfeld für die aktuelle Zelle in Gridweb angezeigt. Wenn wir diese Funktion aktivieren, müssen wir die jquery js-Bibliothek in Ihre ASPX-Dateien importieren, um diese neue Funktion zu unterstützen. die neueste jquery-version ist in ordnung. usw. |
| [ShowCommandBarAtTop](../../aspose.cells.gridweb/mainweb/showcommandbarattop) { get; set; } | Gibt an, ob die Befehlsleiste (einschließlich Befehlsleiste und Registerkartenleiste) oben im Steuerelement angezeigt werden soll. |
| [ShowContextMenu](../../aspose.cells.gridweb/mainweb/showcontextmenu) { get; set; } |  |
| [ShowDefaultGridLine](../../aspose.cells.gridweb/mainweb/showdefaultgridline) { get; set; } | Ruft ab oder legt fest, ob die Standardgitterlinien der Zellen angezeigt werden sollen. |
| [ShowHeaderBar](../../aspose.cells.gridweb/mainweb/showheaderbar) { get; set; } |  |
| [ShowLoading](../../aspose.cells.gridweb/mainweb/showloading) { get; set; } | Gibt an, ob beim Postback auf den Server ein Ladedialogfeld angezeigt werden soll. |
| [ShowLoadingPosition](../../aspose.cells.gridweb/mainweb/showloadingposition) { get; set; } | Gibt die linke, obere Position (in px) an, um das Ladedialogfeld während des Postbacks zum Server usw. anzuzeigen. 100.200 bedeutet die linke obere Position des Ladedialogfelds bei 100 Pixel, 200 Pixel . |
| [ShowSaveButton](../../aspose.cells.gridweb/mainweb/showsavebutton) { get; set; } | Ruft ab oder legt fest, ob die Speichern-Schaltfläche angezeigt werden soll. |
| [ShowSubmitButton](../../aspose.cells.gridweb/mainweb/showsubmitbutton) { get; set; } | Ruft ab oder legt fest, ob die Senden-Schaltfläche angezeigt werden soll. |
| [ShowTabBar](../../aspose.cells.gridweb/mainweb/showtabbar) { get; set; } |  |
| [ShowTabNavigation](../../aspose.cells.gridweb/mainweb/showtabnavigation) { get; set; } | Ruft ab oder legt fest, ob die Registerkarten-Navigationsschaltfläche angezeigt wird, der Standardwert ist wahr. |
| [ShowUndoButton](../../aspose.cells.gridweb/mainweb/showundobutton) { get; set; } | Ruft ab oder legt fest, ob die Rückgängig-Schaltfläche angezeigt werden soll. |
| [SpanWrap](../../aspose.cells.gridweb/mainweb/spanwrap) { get; set; } | Gibt an, ob Inhalt in der Zellspanne umbrochen werden soll. Der Standardwert ist wahr. |
| [TabStyle](../../aspose.cells.gridweb/mainweb/tabstyle) { get; set; } | Ruft den Stil der Registerkartenleiste ab oder legt ihn fest. |
| [UseClientPageHeight](../../aspose.cells.gridweb/mainweb/useclientpageheight) { get; set; } | Ruft ab oder legt fest, ob Gridweb die Seitenhöhe des Clients als Kontrollhöhe verwendet, geeignet für wenn Höhe = "100 %" gesetzt ist, Standardwert ist false |
| [ValidationsTable](../../aspose.cells.gridweb/mainweb/validationstable) { get; } |  |
| [ViewPanelScrollLeft](../../aspose.cells.gridweb/mainweb/viewpanelscrollleft) { get; set; } | Ruft die Position der Bildlaufleiste des Ansichtsbereichs des Rasters ab oder legt sie fest. |
| [ViewPanelScrollTop](../../aspose.cells.gridweb/mainweb/viewpanelscrolltop) { get; set; } | Ruft die Position der Bildlaufleiste des Ansichtsbereichs des Rasters ab oder legt sie fest. |
| [ViewTableStyle](../../aspose.cells.gridweb/mainweb/viewtablestyle) { get; set; } | Ruft den Stil des Datenansichtsbereichs ab oder legt ihn fest. |
| [WebWorksheets](../../aspose.cells.gridweb/mainweb/webworksheets) { get; } |  |
| override [Width](../../aspose.cells.gridweb/mainweb/width) { get; set; } | Ruft die Breite ( System.Web.UI.WebControl.Unit ) des Steuerelements ab oder legt sie fest. |
| [WorkSheets](../../aspose.cells.gridweb/mainweb/worksheets) { get; } |  |
| [XhtmlMode](../../aspose.cells.gridweb/mainweb/xhtmlmode) { get; set; } |  |
| static [PictureCachePath](../../aspose.cells.gridweb/mainweb/picturecachepath) { get; set; } | Ruft den Bildspeicherpfad für die Arbeitsmappe ab oder legt ihn fest. Alle Formen und Bilder werden in diesem Verzeichnis gespeichert. Der Standardpfad ist acwcache im Basisverzeichnis der aktuellen Anwendung Sitzungszeit. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [CalculateFormula](../../aspose.cells.gridweb/mainweb/calculateformula)() | Berechnet das Ergebnis von Formeln. |
| override [DataBind](../../aspose.cells.gridweb/mainweb/databind)() | Binden Sie das Steuerelement und alle untergeordneten Steuerelemente an seine Datenquelle. |
| override [Dispose](../../aspose.cells.gridweb/mainweb/dispose)() |  |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile#importexcelfile)(Stream) | Importe aus einem Excel-Datei-Stream, einschließlich Disk-Datei-Stream oder Speicher-Stream. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile#importexcelfile_1)(string) | Importiert aus einer Excel-Datei. |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile#loadcsvfile)(Stream) | Lädt Daten aus einem CSV-Dateistream. |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile#loadcsvfile_1)(string) | Lädt Daten aus einer CSV-Datei. |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile#loadhtmlfile)(Stream) | Lädt Daten aus einem HTML-Dateistream. |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile#loadhtmlfile_1)(string) | Lädt Daten aus einer HTML-Datei. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile#loadspreadsheetmlfile)(Stream) | Lädt Daten aus einem SpreadSheetML-Dateistream. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile#loadspreadsheetmlfile_1)(string) | Lädt Daten aus einer SpreadSheetML-Datei. |
| [RefreshChartShape](../../aspose.cells.gridweb/mainweb/refreshchartshape)() | alle Diagrammbilder für das aktive Arbeitsblatt aktualisieren . |
| override [RenderBeginTag](../../aspose.cells.gridweb/mainweb/renderbegintag)(HtmlTextWriter) |  |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile#savecsvfile)(Stream) | Speichert Daten in einem CSV-Dateistream. |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile#savecsvfile_1)(string) | Speichert Daten in einer CSV-Datei. |
| [SaveCustomStyleFile](../../aspose.cells.gridweb/mainweb/savecustomstylefile)(string) | Speichert aktuelle Stildaten des Steuerelements in einer XML-Datei. Kann verwendet werden, um Ihre benutzerdefinierte Stildatei zu erstellen. |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile#savehtmlfile)(Stream) | Speichert Daten in einem HTML-Dateistream. |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile#savehtmlfile_1)(string) | Speichert Daten in einer HTML-Datei. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile#savespreadsheetmlfile)(Stream) | Speichert Daten in einem SpreadSheetML-Dateistream. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile#savespreadsheetmlfile_1)(string) | Speichert Daten in einer SpreadSheetML-Datei. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile#savetoexcelfile)(Stream) | Speichert die Arbeitsblätter in einer Excel-Datei. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile#savetoexcelfile_3)(string) | Speichert die Arbeitsblätter in einer Excel-Datei im Excel 2003-Format. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile#savetoexcelfile_1)(Stream, GridSaveFormat) | Speichert die Arbeitsblätter in einer Excel-Datei. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile#savetoexcelfile_2)(Stream, GridSaveOptions) | Speichert die Arbeitsblätter in einer Excel-Datei. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile#savetoexcelfile_4)(string, GridSaveFormat) | Speichert die Arbeitsblätter in einer Excel-Datei. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile#savetoexcelfile_5)(string, GridSaveOptions) | Speichert die Arbeitsblätter in einer Excel-Datei. |
| [SetCustomStyle](../../aspose.cells.gridweb/mainweb/setcustomstyle)(Stream) | legt die benutzerdefinierte Stildatei aus dem Stream fest, einschließlich des Festplattendatei-Streams oder des Speicherstreams. |

### Siehe auch

* class [ExtWebControl](../extwebcontrol)
* namensraum [Aspose.Cells.GridWeb](../../aspose.cells.gridweb)
* Montage [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
