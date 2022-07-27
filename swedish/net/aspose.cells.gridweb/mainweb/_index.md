---
title: MainWeb
second_title: Aspose.Cells för .NET API-referens
description: Förälderklass för GridWeb-kontroll. Endast intern användning.
type: docs
weight: 850
url: /sv/net/aspose.cells.gridweb/mainweb/
---
## MainWeb class

Förälderklass för GridWeb-kontroll. Endast intern användning.

```csharp
public class MainWeb : ExtWebControl, INamingContainer, IPostBackDataHandler, 
    IPostBackEventHandler, ISerializable
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [MainWeb](mainweb)() | Default_Constructor |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [ActiveCell](../../aspose.cells.gridweb/mainweb/activecell) { get; set; } | Hämtar eller ställer in den aktiva cellen i det aktuella arket. Ändrad till att vara skrivbar sedan version 1.9.0.1. |
| [ActiveCellBgColor](../../aspose.cells.gridweb/mainweb/activecellbgcolor) { get; set; } | Anger bakgrundsfärgen för den aktiva cellen. |
| [ActiveCellColor](../../aspose.cells.gridweb/mainweb/activecellcolor) { get; set; } | Anger färgen på den aktiva cellen. |
| [ActiveHeaderBgColor](../../aspose.cells.gridweb/mainweb/activeheaderbgcolor) { get; set; } | Anger bakgrundsfärgen för den aktiva rad-/kolumnhuvudet. |
| [ActiveHeaderColor](../../aspose.cells.gridweb/mainweb/activeheadercolor) { get; set; } | Anger färgen på den aktiva rad-/kolumnhuvudet. |
| [ActiveSheet](../../aspose.cells.gridweb/mainweb/activesheet) { get; } | Hämtar det aktiva arket |
| [ActiveSheetIndex](../../aspose.cells.gridweb/mainweb/activesheetindex) { get; set; } | Hämtar eller ställer in det aktiva arkindexet. Lika med WebWorksheets.ActiveSheetIndex. |
| [ActiveTabStyle](../../aspose.cells.gridweb/mainweb/activetabstyle) { get; set; } | Anger stilen för den aktiva fliken. |
| [ACWClientPath](../../aspose.cells.gridweb/mainweb/acwclientpath) { get; set; } | Hämtar eller ställer in webbsökvägen för kontrollens skript-/bildfiler. Till exempel: "http://localhost/acw_client". Du kan också ställa in detta värde i filen web.config. Lägg till det här avsnittet i avsnittet &lt;konfiguration&gt;: &lt;appinställningar&gt;&lt;add key="aspose.cells.gridweb.acw_client_path" value="/acw_client/" /&gt;&lt;/appSettings&gt; |
| [ACWLanguageFileUrl](../../aspose.cells.gridweb/mainweb/acwlanguagefileurl) { get; set; } | Hämtar eller ställer in webbadressen till kontrollens språkfil. Till exempel: "/acw_client/lang_en.js". Som standard används en inbyggd engelsk fil. |
| [AutoRefreshChart](../../aspose.cells.gridweb/mainweb/autorefreshchart) { get; set; } | Hämtar eller ställer in om diagrambilden uppdateras medan cellvärdet uppdateras. standardvärdet är true |
| [BottomTableStyle](../../aspose.cells.gridweb/mainweb/bottomtablestyle) { get; set; } | Hämtar eller ställer in stilen för kontrollens nedre stapel. |
| [CurrentPageIndex](../../aspose.cells.gridweb/mainweb/currentpageindex) { get; set; } |  |
| [CustomCalculationEngine](../../aspose.cells.gridweb/mainweb/customcalculationengine) { get; set; } | Representerar användarens anpassade beräkningsmotor för att utöka standardberäkningsmotorn för Aspose.Cells. |
| [CustomCommandButtons](../../aspose.cells.gridweb/mainweb/customcommandbuttons) { get; } |  |
| [CustomStyleFileName](../../aspose.cells.gridweb/mainweb/customstylefilename) { get; set; } | Hämtar eller ställer in filnamnet för den anpassade stilen. |
| [DefaultFontName](../../aspose.cells.gridweb/mainweb/defaultfontname) { get; set; } | Hämtar eller ställer in kontrollens standardteckensnittsnamn. |
| [DefaultFontSize](../../aspose.cells.gridweb/mainweb/defaultfontsize) { get; set; } | Hämtar eller ställer in kontrollens standardteckensnittsstorlek. |
| [DefaultGridLineColor](../../aspose.cells.gridweb/mainweb/defaultgridlinecolor) { get; set; } | Hämtar eller ställer in standardrutnätslinjens färg. |
| [DisplayCellTip](../../aspose.cells.gridweb/mainweb/displaycelltip) { get; set; } |  |
| [EditMode](../../aspose.cells.gridweb/mainweb/editmode) { get; set; } | Hämtar eller ställer in kontrollens redigeringsläge. |
| [EnableAJAX](../../aspose.cells.gridweb/mainweb/enableajax) { get; set; } |  |
| [EnableAsync](../../aspose.cells.gridweb/mainweb/enableasync) { get; set; } | Hämtar eller ställer in om belastningscellsdata på asynkront sätt, föreslår att ansöka om ett ark med mer än 10000 celler. |
| [EnableClientColumnOperations](../../aspose.cells.gridweb/mainweb/enableclientcolumnoperations) { get; set; } | Hämtar eller ställer in om kolumnoperationer på klientsidan ska aktiveras. |
| [EnableClientFreeze](../../aspose.cells.gridweb/mainweb/enableclientfreeze) { get; set; } | Hämtar eller ställer in om frysning på klientsidan ska aktiveras. |
| [EnableClientMergeOperations](../../aspose.cells.gridweb/mainweb/enableclientmergeoperations) { get; set; } | Hämtar eller ställer in om fusionsoperationer på klientsidan ska aktiveras. |
| [EnableClientResizeColumnRow](../../aspose.cells.gridweb/mainweb/enableclientresizecolumnrow) { get; set; } | Hämtar eller ställer in om du vill aktivera kolumn och rad för att ändra storlek på klientsidan. |
| [EnableClientRowOperations](../../aspose.cells.gridweb/mainweb/enableclientrowoperations) { get; set; } | Hämtar eller ställer in om radoperationer på klientsidan ska aktiveras. |
| [EnableDoubleClickEvent](../../aspose.cells.gridweb/mainweb/enabledoubleclickevent) { get; set; } | Hämtar eller ställer in om dubbelklickshändelse ska aktiveras på kundsidan. |
| [EnableMetalLightEffect](../../aspose.cells.gridweb/mainweb/enablemetallighteffect) { get; set; } | Får eller ställer in om metallljuseffekt ska tillämpas. |
| [EnablePaging](../../aspose.cells.gridweb/mainweb/enablepaging) { get; set; } | Hämtar eller ställer in om kontrollens personsökningsläge ska aktiveras. |
| [EnableStyleDialogbox](../../aspose.cells.gridweb/mainweb/enablestyledialogbox) { get; set; } | Hämtar eller ställer in om dialogrutan stil på klientsidan ska aktiveras. |
| [FilteredPaging](../../aspose.cells.gridweb/mainweb/filteredpaging) { get; set; } | Hämtar eller ställer in om sökningen ska aktiveras efter att data filtrerats, kommer att gälla när EnablePaging är sant. |
| [ForceValidation](../../aspose.cells.gridweb/mainweb/forcevalidation) { get; set; } | Hämtar eller ställer in om validering på kundsidan ska tvingas fram. |
| [FrameTableStyle](../../aspose.cells.gridweb/mainweb/frametablestyle) { get; set; } | Hämtar eller ställer in ramstilen för kontrollen. |
| [GoonDefaultSaveOperation](../../aspose.cells.gridweb/mainweb/goondefaultsaveoperation) { get; set; } | Hämtar eller ställer in om GridWeb ska utföra standardsparningsoperationen, standardvärdet är sant. |
| [HeaderBarHeight](../../aspose.cells.gridweb/mainweb/headerbarheight) { get; set; } | Hämtar eller ställer in höjden (System.Web.UI.WebControl.Unit ) på kontrollens övre rubrikfält. |
| [HeaderBarStyle](../../aspose.cells.gridweb/mainweb/headerbarstyle) { get; set; } | Hämtar eller ställer in rubrikfältets stil. |
| [HeaderBarTableStyle](../../aspose.cells.gridweb/mainweb/headerbartablestyle) { get; set; } | Hämtar eller ställer in huvudfältsstilen för kontrollen. |
| [HeaderBarWidth](../../aspose.cells.gridweb/mainweb/headerbarwidth) { get; set; } | Hämtar eller ställer in width( System.Web.UI.WebControl.Unit ) eller kontrollens vänstra sidhuvud. |
| override [Height](../../aspose.cells.gridweb/mainweb/height) { get; set; } | Hämtar eller ställer in höjden (System.Web.UI.WebControl.Unit) för kontrollen. |
| [IsCalculateFormula](../../aspose.cells.gridweb/mainweb/iscalculateformula) { get; set; } | Hämtar eller ställer in om formeln ska beräknas efter cellvärdeändringar eller efter import av fil. Standardvärdet är sant. |
| [IsPostBack](../../aspose.cells.gridweb/mainweb/ispostback) { get; } | Får ett värde som indikerar om gridweb laddas som svar på en kundreklamation, eller om den laddas och nås för första gången. |
| [LinksTable](../../aspose.cells.gridweb/mainweb/linkstable) { get; } |  |
| [MaxColumn](../../aspose.cells.gridweb/mainweb/maxcolumn) { get; set; } | Hämtar eller ställer in det maximala visningskolumnindexet (nollbaserat) för webbarket. Kontrollen använder det större värdet av MaxColumn och arkdatas maxkolumn. |
| [MaxRow](../../aspose.cells.gridweb/mainweb/maxrow) { get; set; } | Hämtar eller ställer in det maximala visningsradindexet (nollbaserat) för webbarket. Kontrollen använder det större värdet av MaxRow och arkdatas maxrad. |
| [Message](../../aspose.cells.gridweb/mainweb/message) { get; set; } |  |
| [MinColumn](../../aspose.cells.gridweb/mainweb/mincolumn) { get; set; } |  |
| [MinRow](../../aspose.cells.gridweb/mainweb/minrow) { get; set; } | Hämtar eller ställer in det lägsta visningsradindexet (nollbaserat) för webbarket. Kontrollen använder det mindre värdet av MinRow och arkdatas minsta rad. |
| [ModifiedCells](../../aspose.cells.gridweb/mainweb/modifiedcells) { get; } | Hämtar samlingen av cellerna som modifierats av klienten. |
| [NeedRenderGroupRows](../../aspose.cells.gridweb/mainweb/needrendergrouprows) { get; set; } | Hämtar eller ställer in om grupprader ska visas . |
| [NoHScroll](../../aspose.cells.gridweb/mainweb/nohscroll) { get; set; } | Hämtar eller ställer in ett värde som anger om den horisontella rullningslisten är dold. |
| [NoScroll](../../aspose.cells.gridweb/mainweb/noscroll) { get; set; } |  |
| [NoVScroll](../../aspose.cells.gridweb/mainweb/novscroll) { get; set; } | Hämtar eller ställer in ett värde som anger om den vertikala rullningslisten är dold. |
| [OnAjaxCallFinishedClientFunction](../../aspose.cells.gridweb/mainweb/onajaxcallfinishedclientfunction) { get; set; } | Hämtar eller ställer in namnet på klientsidans funktion som ska anropas när ajaxcall avslutats. Klientfunktionen ska deklareras så här: funktion GridAjaxcallFinished() { alert(this.id+" ajaxcall avslutat "); } Obs: Du kan använda "den här"-pekaren i klientfunktionen för att peka på rutnätskontrollen som utlöser händelsen. |
| [OnCellErrorClientFunction](../../aspose.cells.gridweb/mainweb/oncellerrorclientfunction) { get; set; } | Hämtar eller ställer in klientsidans funktionsnamn som ska anropas när en cells validering misslyckas. Klientfunktionen ska deklareras så här: function MyOnCellError(cell) { alert(GridWeb1.getCellValueByCell(cell)); } Obs: Du kan använda "den här"-pekaren i klientfunktionen för att peka på rutnätskontrollen som utlöser händelsen. |
| [OnCellSelectedAjaxCallBackClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedajaxcallbackclientfunction) { get; set; } | Hämtar eller ställer in klientsidans funktion så att den anropas när en cell väljs. Klientfunktionen ska deklareras så här: function MyOnSelectCellAjaxCallBack(cell,kunddata) { } Obs: Du kan använda "den här"-pekaren i klientfunktionen för att peka på rutnätskontrollen som utlöser händelsen. |
| [OnCellSelectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedclientfunction) { get; set; } | Hämtar eller ställer in klientsidans funktion så att den anropas när en cell väljs. Klientfunktionen ska deklareras så här: funktion MyOnSelectCell(cell) { GridWeb1.setCellValueByCell(cell, "test"); } Obs: Du kan använda "den här"-pekaren i klientfunktionen för att peka på rutnätskontrollen som utlöser händelsen. |
| [OnCellUnselectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellunselectedclientfunction) { get; set; } | Hämtar eller ställer in klientsidans funktion så att den anropas när en cell är avmarkerad. Klientfunktionen ska deklareras så här: function MyOnUnselectCell(cell) { GridWeb1.setCellValueByCell(cell, "test"); } Obs: Du kan använda "den här"-pekaren i klientfunktionen för att peka på rutnätskontrollen som utlöser händelsen. |
| [OnCellUpdatedClientFunction](../../aspose.cells.gridweb/mainweb/oncellupdatedclientfunction) { get; set; } | Hämtar eller ställer in klientsidans funktionsnamn som ska anropas när en cells värde uppdateras. Klientfunktionen ska deklareras så här: funktion MyOnCellUpdated(cell) { alert(this.getCellValueByCell(cell)); } Obs: Du kan använda "den här"-pekaren i klientfunktionen för att peka på rutnätskontrollen som utlöser händelsen. |
| [OnContextMenuShowClientFunction](../../aspose.cells.gridweb/mainweb/oncontextmenushowclientfunction) { get; set; } | Hämtar eller ställer in klientsidans funktion så att den ska anropas när snabbmenyn visas. Klientfunktionen ska deklareras så här: funktion på ContextMenuShow() { var menu = event.srcElement; menu.setItemVisibility("Ta bort", "blockera"); menu.setItemVisibility("Uppdatering", "ingen"); } Obs: Du kan använda "den här"-pekaren i klientfunktionen för att peka på rutnätskontrollen som utlöser händelsen. |
| [OnDoubleClickCellClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickcellclientfunction) { get; set; } | Hämtar eller ställer in klientsidans funktion så att den anropas när en cell dubbelklickas. Klientfunktionen ska deklareras så här: funktion MyOnDoubleClickCell(cell) { GridWeb1.setCellValueByCell(cell, "test"); } Obs: Du kan använda "den här"-pekaren i klientfunktionen för att peka på rutnätskontrollen som utlöser händelsen. |
| [OnDoubleClickRowClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickrowclientfunction) { get; set; } | Hämtar eller ställer in klientsidans funktion så att den anropas när en rad dubbelklickas. Klientfunktionen ska deklareras så här: funktion MyOnRowDoubleClick(rad) { alert(rad); } Obs: Du kan använda "den här"-pekaren i klientfunktionen för att peka på rutnätskontrollen som utlöser händelsen. |
| [OnGridInitClientFunction](../../aspose.cells.gridweb/mainweb/ongridinitclientfunction) { get; set; } | Hämtar eller ställer in namnet på klientsidans funktion som ska anropas när rutnätet initieras. Klientfunktionen ska deklareras så här: function MyOnGridInit(grid) { alert("Gridet är initierat: " + grid.id); } Obs: Du kan använda "den här"-pekaren i klientfunktionen för att peka på rutnätskontrollen som utlöser händelsen. |
| [OnlyAuto](../../aspose.cells.gridweb/mainweb/onlyauto) { get; set; } | Hämtar eller ställer in om bara passar raderna vars höjd inte är anpassad, standardvärdet är false |
| [OnPageChangeClientFunction](../../aspose.cells.gridweb/mainweb/onpagechangeclientfunction) { get; set; } | Hämtar eller ställer in klientsidans funktion så att den anropas efter att sidindex har ändrats. träder endast i kraft när EnablePaging är sant. Klientfunktionen ska deklareras så här: function MyOnPageChange(index) { console.log("nuvarande sida är:"+index); } Obs: Du kan använda "den här"-pekaren i klientfunktionen för att peka på rutnätskontrollen som utlöser händelsen. |
| [OnPageSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onpagesubmitclientfunction) { get; set; } | Hämtar eller ställer in klientfunktionen så att den anropas innan sidan skickas på klientsidan. |
| [OnShapeSelectedClientFunction](../../aspose.cells.gridweb/mainweb/onshapeselectedclientfunction) { get; set; } | Hämtar eller ställer in klientsidans funktion som ska anropas när en form väljs. Klientfunktionen ska deklareras så här: funktion MyOnSelectShape(form) { var name=shape.getAttribute("namnvärde") var text=shape.getAttribute("textvalue") var value=shape.getAttribute("kontrollvärde") var type=shape.getAttribute("msotype") } Obs: Du kan använda "den här"-pekaren i klientfunktionen för att peka på rutnätskontrollen som utlöser händelsen. |
| [OnSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onsubmitclientfunction) { get; set; } | Hämtar eller ställer in klientfunktionen som ska anropas innan kontrollen skickas på klientsidan. Klientfunktionen ska deklareras så här: function MyOnSubmit(arg, cancelEdit) { returnera sant;} Arg är submit-argumentet, innehåller kommandot som ska skickas till servern. CancelEdit är booleskt värde indikerar om kontrollen har förkastat användarinmatningen innan submit. Kontrollen kommer att fortsätta skicka om funktionen returnerar true.  Obs: Du kan använda "den här"-pekaren i klientfunktionen för att peka på rutnätskontrollen som utlöser händelsen. |
| [PageSize](../../aspose.cells.gridweb/mainweb/pagesize) { get; set; } | Hämtar eller ställer in sidstorleken i personsökningsläge. |
| [PicturesTable](../../aspose.cells.gridweb/mainweb/picturestable) { get; } |  |
| [PresetStyle](../../aspose.cells.gridweb/mainweb/presetstyle) { get; set; } | Hämtar eller ställer in den förinställda stilen. |
| [RefreshValidation](../../aspose.cells.gridweb/mainweb/refreshvalidation) { get; set; } | Hämtar eller ställer in om valideringsvärdet ska uppdateras efter cellvärdeändringar. |
| [RenderHiddenRow](../../aspose.cells.gridweb/mainweb/renderhiddenrow) { get; set; } | Hämtar eller ställer in om den dolda raden ska renderas i GridControl, standardvärdet är false. om du behöver visa den dolda raden senare, ska du ställa in den som true |
| [ScrollBarArrowColor](../../aspose.cells.gridweb/mainweb/scrollbararrowcolor) { get; set; } | Anger färgen på rullningslistens pilknapp. |
| [ScrollBarBaseColor](../../aspose.cells.gridweb/mainweb/scrollbarbasecolor) { get; set; } | Anger färgen på kontrollens rullningslist. |
| [SelectCellBgColor](../../aspose.cells.gridweb/mainweb/selectcellbgcolor) { get; set; } | Anger bakgrundsfärgen för de markerade cellerna i flervalsområdet. |
| [SelectCellColor](../../aspose.cells.gridweb/mainweb/selectcellcolor) { get; set; } | Anger färgen på de markerade cellerna i flervalsområdet. |
| [SessionLoaded](../../aspose.cells.gridweb/mainweb/sessionloaded) { get; set; } |  |
| [SessionMode](../../aspose.cells.gridweb/mainweb/sessionmode) { get; set; } | Hämtar eller ställer in sessionsläget för rutnätet. Det finns fyra typer av sessionsläge: 1. Session (standard): Använd systemsession för att lagra arkdata. Vanligtvis använder asp.net InProc-sessionstillstånd. Rutnätet stöder också "StateServer" ut process session state och SQLServer session state. 2. ViewState: Använd sidans viewstate för att lagra arkdata. 3. Custom: Använd LoadCustomData och SheetDataUpdated-händelser för att lagra/återställa arkdata. 4. Fil: lagra/återställ arkdata i SessionStorePath. |
| [SessionSaved](../../aspose.cells.gridweb/mainweb/sessionsaved) { get; set; } |  |
| [SessionStorePath](../../aspose.cells.gridweb/mainweb/sessionstorepath) { get; set; } | Hämtar eller ställer in sessionscachelagringssökvägen när sessionsläget är File eller ViewState, etc: gridweb.SessionStorePath="c:/mytempdir/session"; så kommer den att lagra sessionsdata i c:/mytempdir/session |
| [Settings](../../aspose.cells.gridweb/mainweb/settings) { get; set; } | Representerar arbetsboksinställningarna. |
| [ShapesTable](../../aspose.cells.gridweb/mainweb/shapestable) { get; } |  |
| [ShowAddButton](../../aspose.cells.gridweb/mainweb/showaddbutton) { get; set; } | Hämtar eller ställer in om knappen Lägg till kalkylblad ska visas. |
| [ShowBottomBar](../../aspose.cells.gridweb/mainweb/showbottombar) { get; set; } |  |
| [ShowCellEditBox](../../aspose.cells.gridweb/mainweb/showcelleditbox) { get; set; } | om Gridweb visar redigeringsrutans verktygsfält som i MS-EXCEL. Om aktivera, kommer en redigeringsruta för aktuell cell att visas i Gridweb. om vi aktiverar den här funktionen måste vi importera jquery js-biblioteket i dina aspx-filer för att stödja denna nya funktion. all den senaste jquery-versionen är ok. etc. |
| [ShowCommandBarAtTop](../../aspose.cells.gridweb/mainweb/showcommandbarattop) { get; set; } | Anger om kommandofältet (inkluderar kommandofält och flikfält) ska visas överst på kontrollen. |
| [ShowContextMenu](../../aspose.cells.gridweb/mainweb/showcontextmenu) { get; set; } |  |
| [ShowDefaultGridLine](../../aspose.cells.gridweb/mainweb/showdefaultgridline) { get; set; } | Hämtar eller ställer in om standardrutnätslinjerna för cellerna ska visas. |
| [ShowHeaderBar](../../aspose.cells.gridweb/mainweb/showheaderbar) { get; set; } |  |
| [ShowLoading](../../aspose.cells.gridweb/mainweb/showloading) { get; set; } | Anger om en laddningsdialogruta ska visas vid postbackning till servern. |
| [ShowLoadingPosition](../../aspose.cells.gridweb/mainweb/showloadingposition) { get; set; } | Anger den vänstra, översta positionen (i px) för att visa laddningsdialogrutan vid postbackning till servern, etc. 100 200 betyder laddningsdialogrutans vänstra, övre position är 100px,200px . |
| [ShowSaveButton](../../aspose.cells.gridweb/mainweb/showsavebutton) { get; set; } | Hämtar eller ställer in om sparaknappen ska visas. |
| [ShowSubmitButton](../../aspose.cells.gridweb/mainweb/showsubmitbutton) { get; set; } | Hämtar eller ställer in om knappen Skicka ska visas. |
| [ShowTabBar](../../aspose.cells.gridweb/mainweb/showtabbar) { get; set; } |  |
| [ShowTabNavigation](../../aspose.cells.gridweb/mainweb/showtabnavigation) { get; set; } | Hämtar eller ställer in om fliknavigeringsknappen visas, standardvärdet är sant. |
| [ShowUndoButton](../../aspose.cells.gridweb/mainweb/showundobutton) { get; set; } | Hämtar eller ställer in om ångra-knappen ska visas. |
| [SpanWrap](../../aspose.cells.gridweb/mainweb/spanwrap) { get; set; } | Anger om innehåll ska radbrytas i cellomfånget. standardvärdet är sant. |
| [TabStyle](../../aspose.cells.gridweb/mainweb/tabstyle) { get; set; } | Hämtar eller ställer in stilen för flikfältet. |
| [UseClientPageHeight](../../aspose.cells.gridweb/mainweb/useclientpageheight) { get; set; } | Hämtar eller ställer in om gridweb använder klientsidans höjd som kontrollhöjd, lämplig för när inställd Height="100%", standardvärdet är false |
| [ValidationsTable](../../aspose.cells.gridweb/mainweb/validationstable) { get; } |  |
| [ViewPanelScrollLeft](../../aspose.cells.gridweb/mainweb/viewpanelscrollleft) { get; set; } | Hämtar eller ställer in positionen för rullningslisten i rutnätets vypanel. |
| [ViewPanelScrollTop](../../aspose.cells.gridweb/mainweb/viewpanelscrolltop) { get; set; } | Hämtar eller ställer in positionen för rullningslisten i rutnätets vypanel. |
| [ViewTableStyle](../../aspose.cells.gridweb/mainweb/viewtablestyle) { get; set; } | Hämtar eller ställer in datavypanelens stil. |
| [WebWorksheets](../../aspose.cells.gridweb/mainweb/webworksheets) { get; } |  |
| override [Width](../../aspose.cells.gridweb/mainweb/width) { get; set; } | Hämtar eller ställer in bredden (System.Web.UI.WebControl.Unit ) för kontrollen. |
| [WorkSheets](../../aspose.cells.gridweb/mainweb/worksheets) { get; } |  |
| [XhtmlMode](../../aspose.cells.gridweb/mainweb/xhtmlmode) { get; set; } |  |
| static [PictureCachePath](../../aspose.cells.gridweb/mainweb/picturecachepath) { get; set; } | Hämtar eller ställer in bildlagringssökvägen för arbetsboken, alla former, bilderna kommer att lagras i den här katalogen, standardsökvägen är acwcache under nuvarande applikation Base Directory användare behöver implementera en schematjänst för att rensa filerna som är ute av sessionstid. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [CalculateFormula](../../aspose.cells.gridweb/mainweb/calculateformula)() | Beräknar resultatet av formler. |
| override [DataBind](../../aspose.cells.gridweb/mainweb/databind)() | Bind kontrollen och alla dess underordnade kontroller till dess datakälla. |
| override [Dispose](../../aspose.cells.gridweb/mainweb/dispose)() |  |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile#importexcelfile)(Stream) | Importerar från en Excel-filström, inklusive diskfilström eller minnesström. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile#importexcelfile_1)(string) | Importerar från en excel-fil. |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile#loadcsvfile)(Stream) | Laddar data från en CSV-filström. |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile#loadcsvfile_1)(string) | Laddar data från en CSV-fil. |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile#loadhtmlfile)(Stream) | Laddar data från en HTML-filström. |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile#loadhtmlfile_1)(string) | Laddar data från en HTML-fil. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile#loadspreadsheetmlfile)(Stream) | Laddar data från en SpreadSheetML-filström. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile#loadspreadsheetmlfile_1)(string) | Laddar data från en SpreadSheetML-fil. |
| [RefreshChartShape](../../aspose.cells.gridweb/mainweb/refreshchartshape)() | uppdatera alla diagrambilder för det aktiva kalkylbladet . |
| override [RenderBeginTag](../../aspose.cells.gridweb/mainweb/renderbegintag)(HtmlTextWriter) |  |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile#savecsvfile)(Stream) | Sparar data till en CSV-filström. |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile#savecsvfile_1)(string) | Sparar data till en CSV-fil. |
| [SaveCustomStyleFile](../../aspose.cells.gridweb/mainweb/savecustomstylefile)(string) | Sparar aktuell stildata för kontrollen till en xml-fil. Kan användas för att skapa din anpassade stilfil. |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile#savehtmlfile)(Stream) | Sparar data till en HTML-filström. |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile#savehtmlfile_1)(string) | Sparar data till en HTML-fil. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile#savespreadsheetmlfile)(Stream) | Sparar data till en SpreadSheetML-filström. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile#savespreadsheetmlfile_1)(string) | Sparar data till en SpreadSheetML-fil. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile#savetoexcelfile)(Stream) | Sparar kalkylbladen i en excel-fil. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile#savetoexcelfile_3)(string) | Sparar kalkylbladen till en excel-fil med Excel 2003-format. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile#savetoexcelfile_1)(Stream, GridSaveFormat) | Sparar kalkylbladen i en excel-fil. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile#savetoexcelfile_2)(Stream, GridSaveOptions) | Sparar kalkylbladen i en excel-fil. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile#savetoexcelfile_4)(string, GridSaveFormat) | Sparar kalkylbladen i en excel-fil. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile#savetoexcelfile_5)(string, GridSaveOptions) | Sparar kalkylbladen i en excel-fil. |
| [SetCustomStyle](../../aspose.cells.gridweb/mainweb/setcustomstyle)(Stream) | ställer in den anpassade stilfilen från stream inklusive diskfilström eller minnesström. |

### Se även

* class [ExtWebControl](../extwebcontrol)
* namnutrymme [Aspose.Cells.GridWeb](../../aspose.cells.gridweb)
* hopsättning [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
