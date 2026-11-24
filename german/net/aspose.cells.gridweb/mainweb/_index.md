---
title: "Klasse MainWeb"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridWeb.MainWeb Klasse. Elternklasse des GridWeb-Steuerelements. Nur für den internen Gebrauch."
type: docs
url: /de/net/aspose.cells.gridweb/mainweb/
---
## MainWeb class

Elternklasse des GridWeb-Steuerelements. Nur für den internen Gebrauch.

```csharp
public class MainWeb : ExtWebControl, INamingContainer, IPostBackDataHandler, 
    IPostBackEventHandler, ISerializable
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [MainWeb](mainweb/)() | Der Standardkonstruktor des MainWeb-Steuerelements. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ActiveCell](../../aspose.cells.gridweb/mainweb/activecell/) { get; set; } | Liest oder setzt die aktive Zelle des aktuellen Blatts. Seit Version 1.9.0.1 schreibbar geändert. |
| [ActiveCellBgColor](../../aspose.cells.gridweb/mainweb/activecellbgcolor/) { get; set; } | Gibt die Hintergrundfarbe der aktiven Zelle an. |
| [ActiveCellColor](../../aspose.cells.gridweb/mainweb/activecellcolor/) { get; set; } | Gibt die Farbe der aktiven Zelle an. |
| [ActiveHeaderBgColor](../../aspose.cells.gridweb/mainweb/activeheaderbgcolor/) { get; set; } | Gibt die Hintergrundfarbe der aktiven Zeilen‑/Spaltenüberschrift an. |
| [ActiveHeaderColor](../../aspose.cells.gridweb/mainweb/activeheadercolor/) { get; set; } | Gibt die Farbe der aktiven Zeilen‑/Spaltenüberschrift an. |
| [ActiveSheet](../../aspose.cells.gridweb/mainweb/activesheet/) { get; } | Liest das aktive Blatt |
| [ActiveSheetIndex](../../aspose.cells.gridweb/mainweb/activesheetindex/) { get; set; } | Liest oder setzt den Index des aktiven Blatts. Gleich dem WebWorksheets.ActiveSheetIndex. |
| [ActiveTabStyle](../../aspose.cells.gridweb/mainweb/activetabstyle/) { get; set; } | Gibt den Stil des aktiven Tabs an. |
| [ACWClientPath](../../aspose.cells.gridweb/mainweb/acwclientpath/) { get; set; } | Liest oder setzt den Web-Pfad der Skript-/Bilddateien des Steuerelements. Beispiel: "http://localhost/acw_client". Sie können diesen Wert auch in der web.config-Datei festlegen. Fügen Sie diesen Abschnitt zum `<configuration>`-Abschnitt hinzu:`<appSettings>``<add key="aspose.cells.gridweb.acw_client_path" value="/acw_client/" />``</appSettings>` |
| [ACWLanguageFileUrl](../../aspose.cells.gridweb/mainweb/acwlanguagefileurl/) { get; set; } | Liest oder setzt die Web-URL der Sprachdatei des Steuerelements. Beispiel: "/acw_client/lang_en.js". Standardmäßig wird eine integrierte englische Datei verwendet. |
| [AutoRefreshChart](../../aspose.cells.gridweb/mainweb/autorefreshchart/) { get; set; } | Liest oder setzt, ob das Diagrammbild beim Aktualisieren des Zellenwerts aktualisiert wird. Der Standardwert ist true. |
| [BottomTableStyle](../../aspose.cells.gridweb/mainweb/bottomtablestyle/) { get; set; } | Liest oder setzt den Stil der unteren Leiste des Steuerelements. |
| [CurrentPageIndex](../../aspose.cells.gridweb/mainweb/currentpageindex/) { get; set; } | Liest oder setzt den aktuellen Seitenindex im Paging-Modus. |
| [CustomCalculationEngine](../../aspose.cells.gridweb/mainweb/customcalculationengine/) { get; set; } | Stellt die benutzerdefinierte Berechnungs-Engine des Benutzers dar, um die Standard-Berechnungs-Engine von Aspose.Cells zu erweitern. |
| [CustomCommandButtons](../../aspose.cells.gridweb/mainweb/customcommandbuttons/) { get; } | Liest die benutzerdefinierte Befehls-Schaltflächensammlung |
| [CustomStyleFileName](../../aspose.cells.gridweb/mainweb/customstylefilename/) { get; set; } | Liest oder setzt den Dateinamen des benutzerdefinierten Stils. |
| [DefaultFontName](../../aspose.cells.gridweb/mainweb/defaultfontname/) { get; set; } | Liest oder schreibt den Standard‑Schriftartnamen des Steuerelements. |
| [DefaultFontSize](../../aspose.cells.gridweb/mainweb/defaultfontsize/) { get; set; } | Liest oder setzt die Standard-Schriftgröße des Steuerelements. |
| [DefaultGridLineColor](../../aspose.cells.gridweb/mainweb/defaultgridlinecolor/) { get; set; } | Liest oder setzt die Standardfarbe der Rasterlinien. |
| [DisplayCellTip](../../aspose.cells.gridweb/mainweb/displaycelltip/) { get; set; } | Legt fest, ob Tipps angezeigt werden sollen. Der Standardwert ist true. |
| [EditMode](../../aspose.cells.gridweb/mainweb/editmode/) { get; set; } | Legt den Bearbeitungsmodus der Steuerung fest. |
| [EnableAJAX](../../aspose.cells.gridweb/mainweb/enableajax/) { get; set; } | Legt fest, ob ein AJAX-Aufruf verwendet werden soll. Der Standardwert ist true. |
| [EnableAsync](../../aspose.cells.gridweb/mainweb/enableasync/) { get; set; } | Legt fest, ob Zellen-Daten asynchron geladen werden sollen, empfohlen für ein Blatt mit mehr als 10000 Zellen. |
| [EnableClientColumnOperations](../../aspose.cells.gridweb/mainweb/enableclientcolumnoperations/) { get; set; } | Legt fest, ob clientseitige Spaltenoperationen aktiviert werden sollen. |
| [EnableClientFreeze](../../aspose.cells.gridweb/mainweb/enableclientfreeze/) { get; set; } | Legt fest, ob clientseitige Freeze-Operationen aktiviert werden sollen. |
| [EnableClientMergeOperations](../../aspose.cells.gridweb/mainweb/enableclientmergeoperations/) { get; set; } | Legt fest, ob clientseitige Merge-Operationen aktiviert werden sollen. |
| [EnableClientResizeColumnRow](../../aspose.cells.gridweb/mainweb/enableclientresizecolumnrow/) { get; set; } | Legt fest, ob das clientseitige Ändern der Spalten- und Zeilengröße aktiviert werden soll. |
| [EnableClientRowOperations](../../aspose.cells.gridweb/mainweb/enableclientrowoperations/) { get; set; } | Legt fest, ob clientseitige Zeilenoperationen aktiviert werden sollen. |
| [EnableDoubleClickEvent](../../aspose.cells.gridweb/mainweb/enabledoubleclickevent/) { get; set; } | Legt fest, ob das kundenseitige Doppelklick-Ereignis aktiviert werden soll. |
| [EnableMetalLightEffect](../../aspose.cells.gridweb/mainweb/enablemetallighteffect/) { get; set; } | Legt fest, ob der Metal-Light-Effekt angewendet werden soll. |
| [EnablePaging](../../aspose.cells.gridweb/mainweb/enablepaging/) { get; set; } | Legt fest, ob der Paging-Modus der Steuerung aktiviert werden soll. |
| [EnableStyleDialogbox](../../aspose.cells.gridweb/mainweb/enablestyledialogbox/) { get; set; } | Legt fest, ob das clientseitige Stil-Dialogfeld aktiviert werden soll. |
| [FilteredPaging](../../aspose.cells.gridweb/mainweb/filteredpaging/) { get; set; } | Legt fest, ob das Paging nach Datenfilterung aktiviert wird, wirkt nur, wenn EnablePaging true ist. |
| [ForceValidation](../../aspose.cells.gridweb/mainweb/forcevalidation/) { get; set; } | Legt fest, ob die kundenseitige Validierung erzwungen wird. |
| [FrameTableStyle](../../aspose.cells.gridweb/mainweb/frametablestyle/) { get; set; } | Legt den Rahmenstil der Steuerung fest. |
| [GoonDefaultSaveOperation](../../aspose.cells.gridweb/mainweb/goondefaultsaveoperation/) { get; set; } | Legt fest, ob GridWeb die Standardspeicheroperation ausführt, der Standardwert ist true. |
| [HeaderBarHeight](../../aspose.cells.gridweb/mainweb/headerbarheight/) { get; set; } | Legt die Höhe (System.Web.UI.WebControl.Unit) der oberen Kopfzeile der Steuerung fest. |
| [HeaderBarStyle](../../aspose.cells.gridweb/mainweb/headerbarstyle/) { get; set; } | Legt den Stil der Kopfzeile fest. |
| [HeaderBarTableStyle](../../aspose.cells.gridweb/mainweb/headerbartablestyle/) { get; set; } | Legt den Stil der Kopfzeile der Steuerung fest. |
| [HeaderBarWidth](../../aspose.cells.gridweb/mainweb/headerbarwidth/) { get; set; } | Legt die Breite (System.Web.UI.WebControl.Unit) der linken Kopfzeile der Steuerung fest. |
| override [Height](../../aspose.cells.gridweb/mainweb/height/) { get; set; } | Legt die Höhe (System.Web.UI.WebControl.Unit) der Steuerung fest. |
| [IgnoreStyleWithNoData](../../aspose.cells.gridweb/mainweb/ignorestylewithnodata/) { get; set; } | Legt fest, ob GridWeb das Anzeigen von Zeilen oder Spalten ignoriert, die keine Zellwerte enthalten, aber dennoch formatiert sind. Wenn auf true gesetzt, ist die Leistung besser. Der Standardwert ist false, was bedeutet, dass wir letzte zusammenhängende Zeilen/Spalten ohne Zellwerte, aber mit Formatierung, weiterhin anzeigen. Diese Option ist nur gültig, wenn EnableAsync false ist. Sie hat keine Wirkung, wenn EnableAsync true ist, was bedeutet, dass GridWeb alle Zeilen/Spalten mit Formatierung anzeigt. |
| [IsCalculateFormula](../../aspose.cells.gridweb/mainweb/iscalculateformula/) { get; set; } | Legt fest, ob Formeln nach Änderungen des Zellwerts oder nach dem Import einer Datei berechnet werden sollen. Der Standardwert ist true. |
| [IsPostBack](../../aspose.cells.gridweb/mainweb/ispostback/) { get; } | Gibt einen Wert zurück, der angibt, ob GridWeb als Reaktion auf ein Client-Postback geladen wird oder ob es zum ersten Mal geladen und verwendet wird. |
| [LoadOptions](../../aspose.cells.gridweb/mainweb/loadoptions/) { get; set; } | Stellt die Ladeoptionen für GridWeb dar. |
| [MaxColumn](../../aspose.cells.gridweb/mainweb/maxcolumn/) { get; set; } | Liest oder setzt den maximalen Anzeigespaltenindex(nullbasiert) des Webblatts. Das Steuerelement verwendet den größeren Wert von MaxColumn und dem maximalen Spaltenwert der Blattdaten. |
| [MaxRow](../../aspose.cells.gridweb/mainweb/maxrow/) { get; set; } | Liest oder setzt den maximalen Anzeigereihenindex(nullbasiert) des Webblatts. Das Steuerelement verwendet den größeren Wert von MaxRow und dem maximalen Reihenwert der Blattdaten. |
| [Message](../../aspose.cells.gridweb/mainweb/message/) { get; set; } | Liest oder setzt die Meldung für das Raster. |
| [MinColumn](../../aspose.cells.gridweb/mainweb/mincolumn/) { get; set; } | Liest oder setzt den minimalen Anzeigespaltenindex(nullbasiert) des Webblatts. Das Steuerelement verwendet den kleineren Wert von MinColumn und dem minimalen Spaltenwert der Blattdaten. |
| [MinRow](../../aspose.cells.gridweb/mainweb/minrow/) { get; set; } | Liest oder setzt den minimalen Anzeigereihenindex(nullbasiert) des Webblatts. Das Steuerelement verwendet den kleineren Wert von MinRow und dem minimalen Reihenwert der Blattdaten. |
| [ModifiedCells](../../aspose.cells.gridweb/mainweb/modifiedcells/) { get; } | Liest die Sammlung der Zellen, die vom Client geändert wurden. |
| [NeedRenderGroupRows](../../aspose.cells.gridweb/mainweb/needrendergrouprows/) { get; set; } | Liest oder setzt, ob Gruppenreihen angezeigt werden sollen. |
| [NoHScroll](../../aspose.cells.gridweb/mainweb/nohscroll/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob die horizontale Bildlaufleiste ausgeblendet ist. |
| [NoScroll](../../aspose.cells.gridweb/mainweb/noscroll/) { get; set; } | Liest oder setzt, ob die Bildlaufleiste angezeigt wird. |
| [NoVScroll](../../aspose.cells.gridweb/mainweb/novscroll/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob die vertikale Bildlaufleiste ausgeblendet ist. |
| [OnAjaxCallFinishedClientFunction](../../aspose.cells.gridweb/mainweb/onajaxcallfinishedclientfunction/) { get; set; } | Liest oder setzt den Namen der clientseitigen Funktion, die aufgerufen wird, wenn der Ajax‑Aufruf abgeschlossen ist. Die Client‑Funktion sollte wie folgt deklariert werden: function GridAjaxcallFinished() { alert(this.id+" ajaxcall finished "); } Hinweis: Sie können den \"this\"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst. |
| [OnCellErrorClientFunction](../../aspose.cells.gridweb/mainweb/oncellerrorclientfunction/) { get; set; } | Liest oder setzt den Namen der clientseitigen Funktion, die aufgerufen wird, wenn die Validierung einer Zelle fehlschlägt. Die Client‑Funktion sollte wie folgt deklariert werden: function MyOnCellError(cell) { alert(this.getCellValueByCell(cell)); } Hinweis: Sie können den \"this\"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst. |
| [OnCellSelectedAjaxCallBackClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedajaxcallbackclientfunction/) { get; set; } | Liest oder setzt die clientseitige Funktion, die aufgerufen wird, wenn eine Zelle ausgewählt wird. Die Client‑Funktion sollte wie folgt deklariert werden: function MyOnSelectCellAjaxCallBack(cell,customerdata) { } Hinweis: Sie können den \"this\"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst. |
| [OnCellSelectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedclientfunction/) { get; set; } | Liest oder setzt die clientseitige Funktion, die aufgerufen wird, wenn eine Zelle ausgewählt wird. Die Client‑Funktion sollte wie folgt deklariert werden: function MyOnSelectCell(cell) { GridWeb1.setCellValueByCell(cell, \"test\"); } Hinweis: Sie können den \"this\"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst. |
| [OnCellUnselectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellunselectedclientfunction/) { get; set; } | Liest oder setzt die clientseitige Funktion, die aufgerufen wird, wenn eine Zelle deselektiert wird. Die Client‑Funktion sollte wie folgt deklariert werden: function MyOnUnselectCell(cell) { this.setCellValueByCell(cell, \"test\"); } Hinweis: Sie können den \"this\"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst. |
| [OnCellUpdatedClientFunction](../../aspose.cells.gridweb/mainweb/oncellupdatedclientfunction/) { get; set; } | Liest oder setzt den Namen der clientseitigen Funktion, die aufgerufen wird, wenn der Wert einer Zelle aktualisiert wird. Die Client‑Funktion sollte wie folgt deklariert werden: function MyOnCellUpdated(cell) { alert(this.getCellValueByCell(cell)); } Hinweis: Sie können den \"this\"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst. |
| [OnContextMenuShowClientFunction](../../aspose.cells.gridweb/mainweb/oncontextmenushowclientfunction/) { get; set; } | Legt die clientseitige Funktion fest, die aufgerufen wird, wenn das Kontextmenü angezeigt wird, oder ruft sie ab. Die Clientfunktion sollte wie folgt deklariert werden: function onContextMenuShow() { var menu = event.srcElement; menu.setItemVisibility("Delete", "block"); menu.setItemVisibility("Update", "none"); }Hinweis: Sie können den "this"-Zeiger in der Clientfunktion verwenden, um auf das Grid-Steuerelement zu verweisen, das das Ereignis auslöst. |
| [OnDoubleClickCellClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickcellclientfunction/) { get; set; } | Legt die clientseitige Funktion fest, die aufgerufen wird, wenn eine Zelle doppelt angeklickt wird, oder ruft sie ab. Die Clientfunktion sollte wie folgt deklariert werden: function MyOnDoubleClickCell(cell) { this.setCellValueByCell(cell, "test"); }Hinweis: Sie können den "this"-Zeiger in der Clientfunktion verwenden, um auf das Grid-Steuerelement zu verweisen, das das Ereignis auslöst. |
| [OnDoubleClickRowClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickrowclientfunction/) { get; set; } | Legt die clientseitige Funktion fest, die aufgerufen wird, wenn eine Zeile doppelt angeklickt wird, oder ruft sie ab. Die Clientfunktion sollte wie folgt deklariert werden: function MyOnRowDoubleClick(row) { alert(row); }Hinweis: Sie können den "this"-Zeiger in der Clientfunktion verwenden, um auf das Grid-Steuerelement zu verweisen, das das Ereignis auslöst. |
| [OnGridInitClientFunction](../../aspose.cells.gridweb/mainweb/ongridinitclientfunction/) { get; set; } | Legt den Namen der clientseitigen Funktion fest, die aufgerufen wird, wenn das Grid initialisiert wird, oder ruft ihn ab. Die Clientfunktion sollte wie folgt deklariert werden: function MyOnGridInit(grid) { alert("The grid is initialized: " + grid.id); }Hinweis: Sie können den "this"-Zeiger in der Clientfunktion verwenden, um auf das Grid-Steuerelement zu verweisen, das das Ereignis auslöst. |
| [OnlyAuto](../../aspose.cells.gridweb/mainweb/onlyauto/) { get; set; } | Legt fest, ob nur die Zeilen, deren Höhe nicht benutzerdefiniert ist, angepasst werden; der Standardwert ist false. |
| [OnPageChangeClientFunction](../../aspose.cells.gridweb/mainweb/onpagechangeclientfunction/) { get; set; } | Legt die clientseitige Funktion fest, die nach dem Ändern des Seitenindex aufgerufen wird, oder ruft sie ab. Wirkt nur, wenn EnablePaging true ist. Die Clientfunktion sollte wie folgt deklariert werden: function MyOnPageChange(index) { console.log("current page is:"+index); }Hinweis: Sie können den "this"-Zeiger in der Clientfunktion verwenden, um auf das Grid-Steuerelement zu verweisen, das das Ereignis auslöst. |
| [OnPageSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onpagesubmitclientfunction/) { get; set; } | Legt die Clientfunktion fest, die vor dem Absenden der Seite auf der Clientseite aufgerufen wird, oder ruft sie ab. |
| [OnShapeSelectedClientFunction](../../aspose.cells.gridweb/mainweb/onshapeselectedclientfunction/) { get; set; } | Legt die clientseitige Funktion fest, die aufgerufen wird, wenn eine Form ausgewählt wird, oder ruft sie ab. Die Clientfunktion sollte wie folgt deklariert werden: function MyOnSelectShape(shape) { var name=shape.getAttribute("namevalue") var text=shape.getAttribute("textvalue") var value=shape.getAttribute("controlvalue") var type=shape.getAttribute("msotype") }Hinweis: Sie können den "this"-Zeiger in der Clientfunktion verwenden, um auf das Grid-Steuerelement zu verweisen, das das Ereignis auslöst. |
| [OnSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onsubmitclientfunction/) { get; set; } | Legt die Clientfunktion fest, die vor dem Absenden des Steuerelements auf der Clientseite aufgerufen wird, oder ruft sie ab. Die Clientfunktion sollte wie folgt deklariert werden: function MyOnSubmit(arg, cancelEdit) { return true;} Das Argument arg ist das Übermittlungsargument und enthält den Befehl, der an den Server gesendet wird. cancelEdit ist ein boolescher Wert, der angibt, ob das Steuerelement die Benutzereingabe vor dem Absenden verworfen hat. Das Steuerelement wird weiter senden, wenn die Funktion true zurückgibt. Hinweis: Sie können den "this"-Zeiger in der Clientfunktion verwenden, um auf das Grid-Steuerelement zu verweisen, das das Ereignis auslöst. |
| [PageSize](../../aspose.cells.gridweb/mainweb/pagesize/) { get; set; } | Legt die Seitengröße im Paging-Modus fest, oder ruft sie ab. |
| [PresetStyle](../../aspose.cells.gridweb/mainweb/presetstyle/) { get; set; } | Legt den voreingestellten Stil fest, oder ruft ihn ab. |
| [RefreshValidation](../../aspose.cells.gridweb/mainweb/refreshvalidation/) { get; set; } | Legt fest, ob der Validierungswert nach Änderungen des Zellenwerts aktualisiert werden soll, oder ruft diese Einstellung ab. |
| [RenderHiddenRow](../../aspose.cells.gridweb/mainweb/renderhiddenrow/) { get; set; } | Legt fest, ob die versteckte Zeile in GridControl gerendert wird, der Standardwert ist false. Wenn Sie die versteckte Zeile später wieder einblenden müssen, setzen Sie sie auf true. |
| [RowHeightForCSV](../../aspose.cells.gridweb/mainweb/rowheightforcsv/) { get; set; } | Legt die Zeilenhöhe in Punkten für CSV-Dateien fest, Standardwert ist 14,5. |
| [ScrollBarArrowColor](../../aspose.cells.gridweb/mainweb/scrollbararrowcolor/) { get; set; } | Gibt die Farbe des Pfeilsymbols der Bildlaufleiste an. |
| [ScrollBarBaseColor](../../aspose.cells.gridweb/mainweb/scrollbarbasecolor/) { get; set; } | Gibt die Farbe der Bildlaufleiste des Steuerelements an. |
| [SelectCellBgColor](../../aspose.cells.gridweb/mainweb/selectcellbgcolor/) { get; set; } | Gibt die Hintergrundfarbe der ausgewählten Zellen im Mehrfachauswahlbereich an. |
| [SelectCellColor](../../aspose.cells.gridweb/mainweb/selectcellcolor/) { get; set; } | Gibt die Farbe der ausgewählten Zellen im Mehrfachauswahlbereich an. |
| [SessionMode](../../aspose.cells.gridweb/mainweb/sessionmode/) { get; set; } | Legt den Sitzungsmodus des Rasters fest. |
| [SessionStorePath](../../aspose.cells.gridweb/mainweb/sessionstorepath/) { get; set; } | Legt den Pfad des Sitzungs-Cachespeichers fest, wenn der Sitzungsmodus File oder ViewState ist, usw.: gridweb.SessionStorePath=\"c:/mytempdir/session\"; danach werden Sitzungsdaten in c:/mytempdir/session gespeichert. |
| [Settings](../../aspose.cells.gridweb/mainweb/settings/) { get; set; } | Stellt die Einstellungen der Arbeitsmappe dar. |
| [ShowAddButton](../../aspose.cells.gridweb/mainweb/showaddbutton/) { get; set; } | Legt fest, ob die Schaltfläche zum Hinzufügen eines Arbeitsblatts angezeigt wird. |
| [ShowBottomBar](../../aspose.cells.gridweb/mainweb/showbottombar/) { get; set; } | Gibt an, ob die Befehlsleiste (einschließlich Befehlsleiste und Registerkartenleiste) am unteren Rand des Steuerelements angezeigt wird. |
| [ShowCellEditBox](../../aspose.cells.gridweb/mainweb/showcelleditbox/) { get; set; } | Ob Gridweb die Bearbeitungsfeld‑Symbolleiste wie in MS‑EXCEL anzeigt. Wenn aktiviert, wird ein Bearbeitungsfeld für die aktuelle Zelle in Gridweb angezeigt. Wenn wir diese Funktion aktivieren, müssen wir die jQuery‑JS‑Bibliothek in Ihre .aspx‑Dateien importieren, um diese neue Funktion zu unterstützen. Jede aktuelle jQuery‑Version ist geeignet, usw. |
| [ShowCommandBarAtTop](../../aspose.cells.gridweb/mainweb/showcommandbarattop/) { get; set; } | Gibt an, ob die Befehlsleiste (einschließlich Befehlsleiste und Registerkartenleiste) am oberen Rand des Steuerelements angezeigt wird. |
| [ShowContextMenu](../../aspose.cells.gridweb/mainweb/showcontextmenu/) { get; set; } | Legt fest, ob das Kontextmenü angezeigt wird. Der Standardwert ist true. |
| [ShowDefaultGridLine](../../aspose.cells.gridweb/mainweb/showdefaultgridline/) { get; set; } | Legt fest, ob die Standardgitterlinien der Zellen angezeigt werden. |
| [ShowHeaderBar](../../aspose.cells.gridweb/mainweb/showheaderbar/) { get; set; } | Legt fest, ob die Kopfzeilenleiste angezeigt wird |
| [ShowLoading](../../aspose.cells.gridweb/mainweb/showloading/) { get; set; } | Gibt an, ob während des Postbacks zum Server ein Lade‑Dialogfeld angezeigt wird. |
| [ShowLoadingPosition](../../aspose.cells.gridweb/mainweb/showloadingposition/) { get; set; } | Gibt die linke, obere Position (in px) an, um das Lade‑Dialogfeld während des Postbacks zum Server anzuzeigen, usw. 100,200 bedeutet, dass die linke, obere Position des Lade‑Dialogfelds bei 100 px, 200 px liegt. |
| [ShowSaveButton](../../aspose.cells.gridweb/mainweb/showsavebutton/) { get; set; } | Legt fest, ob die Schaltfläche zum Speichern angezeigt wird. |
| [ShowSubmitButton](../../aspose.cells.gridweb/mainweb/showsubmitbutton/) { get; set; } | Legt fest, ob die Schaltfläche zum Senden angezeigt wird. |
| [ShowTabBar](../../aspose.cells.gridweb/mainweb/showtabbar/) { get; set; } | Legt fest, ob die Registerkartenleiste angezeigt wird. |
| [ShowTabNavigation](../../aspose.cells.gridweb/mainweb/showtabnavigation/) { get; set; } | Legt fest, ob die Registerkarten‑Navigationsschaltfläche angezeigt wird, der Standardwert ist true. |
| [ShowUndoButton](../../aspose.cells.gridweb/mainweb/showundobutton/) { get; set; } | Legt fest, ob die Rückgängig‑Schaltfläche angezeigt wird. |
| [SpanWrap](../../aspose.cells.gridweb/mainweb/spanwrap/) { get; set; } | Gibt an, ob der Inhalt im Zellen‑Span umgebrochen wird. Der Standardwert ist true. |
| [TabStyle](../../aspose.cells.gridweb/mainweb/tabstyle/) { get; set; } | Legt den Stil der Registerkartenleiste fest. |
| [UseClientPageHeight](../../aspose.cells.gridweb/mainweb/useclientpageheight/) { get; set; } | Legt fest, ob Gridweb die Höhe der Client‑Seite als Steuerelementhöhe verwendet, geeignet für den Fall, dass Height=\"100%\" gesetzt ist, Standardwert ist false. |
| [ViewPanelScrollLeft](../../aspose.cells.gridweb/mainweb/viewpanelscrollleft/) { get; set; } | Legt die Position der Bildlaufleiste des Ansichtsbereichs des Rasters fest. |
| [ViewPanelScrollTop](../../aspose.cells.gridweb/mainweb/viewpanelscrolltop/) { get; set; } | Legt die Position der Bildlaufleiste des Ansichtsbereichs des Rasters fest. |
| [ViewTableStyle](../../aspose.cells.gridweb/mainweb/viewtablestyle/) { get; set; } | Legt den Stil des Datenansichtsbereichs fest. |
| [WebWorksheets](../../aspose.cells.gridweb/mainweb/webworksheets/) { get; } |  |
| override [Width](../../aspose.cells.gridweb/mainweb/width/) { get; set; } | Liest oder setzt die Breite( System.Web.UI.WebControl.Unit ) des Steuerelements. |
| [WorkSheets](../../aspose.cells.gridweb/mainweb/worksheets/) { get; } | Liest oder setzt die Sammlung der Arbeitsblätter. |
| [XhtmlMode](../../aspose.cells.gridweb/mainweb/xhtmlmode/) { get; set; } | Liest oder setzt, ob XHTML-Stil verwendet wird, der Standardwert ist true. |
| static [DPI](../../aspose.cells.gridweb/mainweb/dpi/) { get; set; } | Liest /setzt die DPI der Maschine. |
| static [PictureCachePath](../../aspose.cells.gridweb/mainweb/picturecachepath/) { get; set; } | Liest oder setzt den Bildspeicherpfad für die Arbeitsmappe, alle Formen und Bilder werden in diesem Verzeichnis gespeichert, der Standardpfad ist acwcache im Basisverzeichnis der aktuellen Anwendung; Benutzer müssen einen geplanten Dienst implementieren, um Dateien, die außerhalb der Sitzungszeit liegen, zu bereinigen. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [CalculateFormula](../../aspose.cells.gridweb/mainweb/calculateformula/)() | Berechnet das Ergebnis von Formeln. |
| override [DataBind](../../aspose.cells.gridweb/mainweb/databind/)() | Bindet das Steuerelement und alle seine untergeordneten Steuerelemente an dessen Datenquelle. |
| override [Dispose](../../aspose.cells.gridweb/mainweb/dispose/)() |  |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile)(Stream) | Importiert aus einem Excel-Dateistream, einschließlich Dateistream von Festplatte oder Speicherstream. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile_2)(string) | Importiert aus einer Excel-Datei. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile_1)(Stream, string) | Importiert aus einem Excel-Dateistream, einschließlich Dateistream von Festplatte oder Speicherstream. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile_3)(string, string) | Importiert aus einer Excel-Datei. |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile/#loadcsvfile)(Stream) | Lädt Daten aus einem CSV-Datei-Stream. |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile/#loadcsvfile_1)(string) | Lädt Daten aus einer CSV-Datei. |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile/#loadhtmlfile)(Stream) | Lädt Daten aus einem HTML-Datei-Stream. |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile/#loadhtmlfile_1)(string) | Lädt Daten aus einer HTML-Datei. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile/#loadspreadsheetmlfile)(Stream) | Lädt Daten aus einem SpreadSheetML-Datei-Stream. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile/#loadspreadsheetmlfile_1)(string) | Lädt Daten aus einer SpreadSheetML-Datei. |
| [RefreshChartShape](../../aspose.cells.gridweb/mainweb/refreshchartshape/)() | Aktualisiert alle Diagrammbilder für das aktive Arbeitsblatt. |
| override [RenderBeginTag](../../aspose.cells.gridweb/mainweb/renderbegintag/)(HtmlTextWriter) |  |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile/#savecsvfile)(Stream) | Speichert Daten in einen CSV-Datei-Stream. |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile/#savecsvfile_1)(string) | Speichert Daten in einer CSV-Datei. |
| [SaveCustomStyleFile](../../aspose.cells.gridweb/mainweb/savecustomstylefile/)(string) | Speichert die aktuellen Stildaten des Steuerelements in einer XML-Datei. Kann verwendet werden, um Ihre benutzerdefinierte Stildatei zu erstellen. |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile/#savehtmlfile)(Stream) | Speichert Daten in einen HTML-Datei-Stream. |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile/#savehtmlfile_1)(string) | Speichert Daten in einer HTML-Datei. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile/#savespreadsheetmlfile)(Stream) | Speichert Daten in einen SpreadSheetML-Datei-Stream. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile/#savespreadsheetmlfile_1)(string) | Speichert Daten in einer SpreadSheetML-Datei. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile)(Stream) | Speichert die Arbeitsblätter in einer Excel-Datei. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_3)(string) | Speichert die Arbeitsblätter in einer Excel-Datei im Excel‑2003-Format. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_1)(Stream, GridSaveFormat) | Speichert die Arbeitsblätter in einer Excel-Datei. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_2)(Stream, GridSaveOptions) | Speichert die Arbeitsblätter in einer Excel-Datei. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_4)(string, GridSaveFormat) | Speichert die Arbeitsblätter in einer Excel-Datei. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_5)(string, GridSaveOptions) | Speichert die Arbeitsblätter in einer Excel-Datei. |
| [SetCustomStyle](../../aspose.cells.gridweb/mainweb/setcustomstyle/)(Stream) | Setzt die benutzerdefinierte Stildatei aus einem Stream, einschließlich Dateistream oder Memory-Stream. |

## Ereignisse

| Name | Beschreibung |
| --- | --- |
| event [AfterColumnFilter](../../aspose.cells.gridweb/mainweb/aftercolumnfilter/) | Tritt auf, nachdem die Spalte gefiltert wurde. |
| event [AjaxCallFinished](../../aspose.cells.gridweb/mainweb/ajaxcallfinished/) | Wird ausgelöst, wenn das AJAX-Update des Steuerelements abgeschlossen ist. (EnableAJAX muss auf true gesetzt werden) |
| event [BeforeColumnFilter](../../aspose.cells.gridweb/mainweb/beforecolumnfilter/) | Tritt auf, bevor die Spalte gefiltert wird. |
| event [CellClickOnAjax](../../aspose.cells.gridweb/mainweb/cellclickonajax/) | Tritt auf, wenn die Zelle angeklickt wird, und ein Ajax-Callback für dieses Ereignis erforderlich ist. |
| event [CellClientUpdate](../../aspose.cells.gridweb/mainweb/cellclientupdate/) | Tritt auf, wenn ein Client-Zellen-Update erfolgt. Wenn dieses Ereignis ausgelöst wird, enthält sein Parameter e.Argument den Namen des Befehls. |
| event [CellCommand](../../aspose.cells.gridweb/mainweb/cellcommand/) | Tritt auf, wenn der Befehls-Hyperlink einer Zelle angeklickt wird. Wenn dieses Ereignis ausgelöst wird, enthält sein Parameter e.Argument den Namen des Befehls. |
| event [CellDoubleClick](../../aspose.cells.gridweb/mainweb/celldoubleclick/) | Tritt auf, wenn die Zelle doppelt angeklickt wird. |
| event [CellError](../../aspose.cells.gridweb/mainweb/cellerror/) | Tritt auf, wenn ein Eingabewertfehler einer Zelle vorliegt. |
| event [CellModifiedOnAjax](../../aspose.cells.gridweb/mainweb/cellmodifiedonajax/) | Tritt auf, wenn die Zelle in einem Ajax-Aufruf geändert wird. |
| event [ColumnDeleted](../../aspose.cells.gridweb/mainweb/columndeleted/) | Tritt auf, wenn der Benutzer eine Spalte aus dem clientseitigen Menü löscht. |
| event [ColumnDeleting](../../aspose.cells.gridweb/mainweb/columndeleting/) | Tritt auf, wenn der Benutzer versucht, eine Spalte aus dem clientseitigen Menü zu löschen. Sie können dieses Ereignis behandeln und den Abbruchparameter auf True setzen, um den Löschvorgang abzubrechen. |
| event [ColumnDoubleClick](../../aspose.cells.gridweb/mainweb/columndoubleclick/) | Tritt auf, wenn die Spaltenüberschrift doppelt angeklickt wird. |
| event [ColumnInserted](../../aspose.cells.gridweb/mainweb/columninserted/) | Tritt auf, wenn der Benutzer eine Spalte aus dem clientseitigen Menü einfügt. |
| event [CustomCommand](../../aspose.cells.gridweb/mainweb/customcommand/) | Tritt auf, wenn der Benutzer einen benutzerdefinierten Befehlsbutton anklickt. |
| event [LoadCustomData](../../aspose.cells.gridweb/mainweb/loadcustomdata/) | Wird ausgelöst, wenn der SessionMode des Steuerelements auf Custom gesetzt ist und Blattdaten geladen werden müssen. Sie können dieses Ereignis im benutzerdefinierten Sitzungsmodus behandeln, um Blattdaten aus einer Datei oder Datenbank zu laden. |
| event [PageIndexChanged](../../aspose.cells.gridweb/mainweb/pageindexchanged/) | Tritt auf, wenn sich der Blattseitenindex des Steuerelements ändert. |
| event [RowDeleted](../../aspose.cells.gridweb/mainweb/rowdeleted/) | Tritt auf, wenn der Benutzer eine Zeile aus dem clientseitigen Menü gelöscht hat. |
| event [RowDeleting](../../aspose.cells.gridweb/mainweb/rowdeleting/) | Tritt auf, wenn der Benutzer versucht, eine Zeile aus dem clientseitigen Menü zu löschen. Sie können dieses Ereignis behandeln und eine RejectDeleteException-Ausnahme auslösen, um den Löschvorgang abzubrechen. |
| event [RowDoubleClick](../../aspose.cells.gridweb/mainweb/rowdoubleclick/) | Tritt auf, wenn die Zeilenüberschrift doppelt angeklickt wird. |
| event [RowInserted](../../aspose.cells.gridweb/mainweb/rowinserted/) | Tritt auf, wenn der Benutzer eine Zeile aus dem clientseitigen Menü einfügt. |
| event [SaveCommand](../../aspose.cells.gridweb/mainweb/savecommand/) | Tritt auf, wenn die Schaltfläche "save" geklickt wird. |
| event [SheetAdded](../../aspose.cells.gridweb/mainweb/sheetadded/) | Tritt auf, wenn der Benutzer ein Arbeitsblatt aus dem Symbolleistenmenü hinzufügt. |
| event [SheetDataUpdated](../../aspose.cells.gridweb/mainweb/sheetdataupdated/) | Tritt auf, wenn das Steuerelement die gesendeten Daten geladen und die Blattdaten aktualisiert hat. |
| event [SheetTabClick](../../aspose.cells.gridweb/mainweb/sheettabclick/) | Tritt auf, wenn das Blattregister geklickt wird. |
| event [SubmitCommand](../../aspose.cells.gridweb/mainweb/submitcommand/) | Tritt auf, wenn die Schaltfläche "submit" geklickt wird. |
| event [UndoCommand](../../aspose.cells.gridweb/mainweb/undocommand/) | Tritt auf, wenn die Schaltfläche "undo" geklickt wird. |

### Beispiele

```csharp
[C#]
	GridWeb GridWeb1 = new GridWeb();
//Erledigen Sie Ihr Geschäft.
```

### Siehe auch

* class [ExtWebControl](../extwebcontrol/)
* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


