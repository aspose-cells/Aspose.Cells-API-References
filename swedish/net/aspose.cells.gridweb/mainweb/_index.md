---
title: "Klass MainWeb"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridWeb.MainWeb-klass. Föräldraklass till GridWeb-kontrollen. Endast för internt bruk"
type: docs
url: /sv/net/aspose.cells.gridweb/mainweb/
---
## MainWeb class

Föräldraklass för GridWeb-kontrollen. Endast för internt bruk.

```csharp
public class MainWeb : ExtWebControl, INamingContainer, IPostBackDataHandler, 
    IPostBackEventHandler, ISerializable
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [MainWeb](mainweb/)() | standardkonstruktorn för MainWeb-kontrollen. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ActiveCell](../../aspose.cells.gridweb/mainweb/activecell/) { get; set; } | Hämtar eller anger den aktiva cellen i det aktuella bladet. Ändrad till skrivbar sedan version 1.9.0.1. |
| [ActiveCellBgColor](../../aspose.cells.gridweb/mainweb/activecellbgcolor/) { get; set; } | Anger bakgrundsfärgen för den aktiva cellen. |
| [ActiveCellColor](../../aspose.cells.gridweb/mainweb/activecellcolor/) { get; set; } | Anger färgen på den aktiva cellen. |
| [ActiveHeaderBgColor](../../aspose.cells.gridweb/mainweb/activeheaderbgcolor/) { get; set; } | Anger bakgrundsfärgen för den aktiva rad-/kolumnrubriken. |
| [ActiveHeaderColor](../../aspose.cells.gridweb/mainweb/activeheadercolor/) { get; set; } | Anger färgen på den aktiva rad-/kolumnrubriken. |
| [ActiveSheet](../../aspose.cells.gridweb/mainweb/activesheet/) { get; } | Hämtar det aktiva bladet |
| [ActiveSheetIndex](../../aspose.cells.gridweb/mainweb/activesheetindex/) { get; set; } | Hämtar eller anger index för det aktiva bladet. Motsvarar WebWorksheets.ActiveSheetIndex. |
| [ActiveTabStyle](../../aspose.cells.gridweb/mainweb/activetabstyle/) { get; set; } | Anger stilen för den aktiva fliken. |
| [ACWClientPath](../../aspose.cells.gridweb/mainweb/acwclientpath/) { get; set; } | Hämtar eller anger webbadressen för skript-/bildfilerna för kontrollen. Till exempel: "http://localhost/acw_client". Du kan också ange detta värde i web.config-filen. Lägg till detta avsnitt i `<configuration>`-sektionen:`<appSettings>```<add key=\"aspose.cells.gridweb.acw_client_path\" value=\"/acw_client/\" />``</appSettings>` |
| [ACWLanguageFileUrl](../../aspose.cells.gridweb/mainweb/acwlanguagefileurl/) { get; set; } | Hämtar eller anger webbadressen för språkfilen för kontrollen. Till exempel: "/acw_client/lang_en.js". Som standard används en inbyggd engelsk fil. |
| [AutoRefreshChart](../../aspose.cells.gridweb/mainweb/autorefreshchart/) { get; set; } | Hämtar eller anger om diagrambilden uppdateras när cellvärdet uppdateras. Standardvärdet är true. |
| [BottomTableStyle](../../aspose.cells.gridweb/mainweb/bottomtablestyle/) { get; set; } | Hämtar eller anger stilen för kontrollens nedre stapel. |
| [CurrentPageIndex](../../aspose.cells.gridweb/mainweb/currentpageindex/) { get; set; } | Hämtar eller anger det aktuella sidindexet i pagineringsläge. |
| [CustomCalculationEngine](../../aspose.cells.gridweb/mainweb/customcalculationengine/) { get; set; } | Representerar användarens anpassade beräkningsmotor för att utöka standardberäkningsmotorn i Aspose.Cells. |
| [CustomCommandButtons](../../aspose.cells.gridweb/mainweb/customcommandbuttons/) { get; } | Hämtar den anpassade samlingen av kommandoknappar |
| [CustomStyleFileName](../../aspose.cells.gridweb/mainweb/customstylefilename/) { get; set; } | Hämtar eller anger filnamnet för den anpassade stilen. |
| [DefaultFontName](../../aspose.cells.gridweb/mainweb/defaultfontname/) { get; set; } | Hämtar eller anger kontrollens standardteckensnittnamn. |
| [DefaultFontSize](../../aspose.cells.gridweb/mainweb/defaultfontsize/) { get; set; } | Hämtar eller anger kontrollens standardteckenstorlek. |
| [DefaultGridLineColor](../../aspose.cells.gridweb/mainweb/defaultgridlinecolor/) { get; set; } | Hämtar eller anger standardfärgen för rutnätslinjer. |
| [DisplayCellTip](../../aspose.cells.gridweb/mainweb/displaycelltip/) { get; set; } | Hämtar eller anger om tips ska visas. Standardvärdet är true. |
| [EditMode](../../aspose.cells.gridweb/mainweb/editmode/) { get; set; } | Hämtar eller anger kontrollens redigeringsläge. |
| [EnableAJAX](../../aspose.cells.gridweb/mainweb/enableajax/) { get; set; } | Hämtar eller anger om AJAX-anrop ska användas. Standardvärdet är true. |
| [EnableAsync](../../aspose.cells.gridweb/mainweb/enableasync/) { get; set; } | Hämtar eller anger om celldata ska laddas asynkront, rekommenderas för ett blad med mer än 10 000 celler. |
| [EnableClientColumnOperations](../../aspose.cells.gridweb/mainweb/enableclientcolumnoperations/) { get; set; } | Hämtar eller anger om kolumnoperationer på klientsidan ska aktiveras. |
| [EnableClientFreeze](../../aspose.cells.gridweb/mainweb/enableclientfreeze/) { get; set; } | Hämtar eller anger om frysoperationer på klientsidan ska aktiveras. |
| [EnableClientMergeOperations](../../aspose.cells.gridweb/mainweb/enableclientmergeoperations/) { get; set; } | Hämtar eller anger om sammanslagningsoperationer på klientsidan ska aktiveras. |
| [EnableClientResizeColumnRow](../../aspose.cells.gridweb/mainweb/enableclientresizecolumnrow/) { get; set; } | Hämtar eller anger om ändring av storlek på kolumner och rader på klientsidan ska aktiveras. |
| [EnableClientRowOperations](../../aspose.cells.gridweb/mainweb/enableclientrowoperations/) { get; set; } | Hämtar eller anger om radoperationer på klientsidan ska aktiveras. |
| [EnableDoubleClickEvent](../../aspose.cells.gridweb/mainweb/enabledoubleclickevent/) { get; set; } | Hämtar eller anger om dubbelklickshändelse på kundsidan ska aktiveras. |
| [EnableMetalLightEffect](../../aspose.cells.gridweb/mainweb/enablemetallighteffect/) { get; set; } | Hämtar eller anger om metallljuseffekt ska tillämpas. |
| [EnablePaging](../../aspose.cells.gridweb/mainweb/enablepaging/) { get; set; } | Hämtar eller anger om kontrollens pagineringsläge ska aktiveras. |
| [EnableStyleDialogbox](../../aspose.cells.gridweb/mainweb/enablestyledialogbox/) { get; set; } | Hämtar eller anger om stil‑dialogrutan på klientsidan ska aktiveras. |
| [FilteredPaging](../../aspose.cells.gridweb/mainweb/filteredpaging/) { get; set; } | Hämtar eller anger om paginering ska aktiveras efter att data filtrerats, gäller när EnablePaging är true. |
| [ForceValidation](../../aspose.cells.gridweb/mainweb/forcevalidation/) { get; set; } | Hämtar eller anger om validering på kundsidan ska tvingas. |
| [FrameTableStyle](../../aspose.cells.gridweb/mainweb/frametablestyle/) { get; set; } | Hämtar eller anger ramstilen för kontrollen. |
| [GoonDefaultSaveOperation](../../aspose.cells.gridweb/mainweb/goondefaultsaveoperation/) { get; set; } | Hämtar eller anger om GridWeb ska utföra standard‑sparåtgärden, standardvärdet är true. |
| [HeaderBarHeight](../../aspose.cells.gridweb/mainweb/headerbarheight/) { get; set; } | Hämtar eller anger höjden (System.Web.UI.WebControl.Unit) för kontrollens övre rubrikrad. |
| [HeaderBarStyle](../../aspose.cells.gridweb/mainweb/headerbarstyle/) { get; set; } | Hämtar eller anger stil för rubrikraden. |
| [HeaderBarTableStyle](../../aspose.cells.gridweb/mainweb/headerbartablestyle/) { get; set; } | Hämtar eller anger rubrikradens stil för kontrollen. |
| [HeaderBarWidth](../../aspose.cells.gridweb/mainweb/headerbarwidth/) { get; set; } | Hämtar eller anger bredden (System.Web.UI.WebControl.Unit) för kontrollens vänstra rubrikrad. |
| override [Height](../../aspose.cells.gridweb/mainweb/height/) { get; set; } | Hämtar eller anger höjden (System.Web.UI.WebControl.Unit) för kontrollen. |
| [IgnoreStyleWithNoData](../../aspose.cells.gridweb/mainweb/ignorestylewithnodata/) { get; set; } | Hämtar eller anger om GridWeb ignorerar att visa rader eller kolumner som inte innehåller cellvärden men ändå är formaterade. Om den sätts till true blir prestandan bättre. Standardvärdet är false, vilket betyder att om den sista på varandra följande raden/kolumnen saknar cellvärden men är formaterad, kommer den fortfarande att visas. Detta alternativ är endast giltigt när EnableAsync är false. Detta alternativ har ingen effekt när EnableAsync är true, vilket betyder att GridWeb kommer att visa alla rader/kolumner med stil. |
| [IsCalculateFormula](../../aspose.cells.gridweb/mainweb/iscalculateformula/) { get; set; } | Hämtar eller anger om formel ska beräknas efter att cellvärdet ändras eller efter import av fil. Standardvärdet är true. |
| [IsPostBack](../../aspose.cells.gridweb/mainweb/ispostback/) { get; } | Hämtar ett värde som indikerar om GridWeb laddas som svar på en klient‑postback, eller om den laddas och nås för första gången. |
| [LoadOptions](../../aspose.cells.gridweb/mainweb/loadoptions/) { get; set; } | Representerar laddningsalternativen för GridWeb. |
| [MaxColumn](../../aspose.cells.gridweb/mainweb/maxcolumn/) { get; set; } | Hämtar eller anger det maximala visningskolumnindexet (nollbaserat) för webblarket. Kontrollen använder det större värdet av MaxColumn och bladdata's maximala kolumn. |
| [MaxRow](../../aspose.cells.gridweb/mainweb/maxrow/) { get; set; } | Hämtar eller anger det maximala visningsradindexet (nollbaserat) för webblarket. Kontrollen använder det större värdet av MaxRow och bladdata's maximala rad. |
| [Message](../../aspose.cells.gridweb/mainweb/message/) { get; set; } | Hämtar eller anger meddelandet för rutnätet. |
| [MinColumn](../../aspose.cells.gridweb/mainweb/mincolumn/) { get; set; } | Hämtar eller anger det minsta visningskolumnindexet (nollbaserat) för webblarket. Kontrollen använder det mindre värdet av MinColumn och bladdata's minsta kolumn. |
| [MinRow](../../aspose.cells.gridweb/mainweb/minrow/) { get; set; } | Hämtar eller anger det minsta visningsradindexet (nollbaserat) för webblarket. Kontrollen använder det mindre värdet av MinRow och bladdata's minsta rad. |
| [ModifiedCells](../../aspose.cells.gridweb/mainweb/modifiedcells/) { get; } | Hämtar samlingen av celler som har modifierats av klienten. |
| [NeedRenderGroupRows](../../aspose.cells.gridweb/mainweb/needrendergrouprows/) { get; set; } | Hämtar eller anger om grouprows ska visas. |
| [NoHScroll](../../aspose.cells.gridweb/mainweb/nohscroll/) { get; set; } | Hämtar eller anger ett värde som indikerar om den horisontella rullningslisten är dold. |
| [NoScroll](../../aspose.cells.gridweb/mainweb/noscroll/) { get; set; } | Hämtar eller anger om rullningslisten ska visas. |
| [NoVScroll](../../aspose.cells.gridweb/mainweb/novscroll/) { get; set; } | Hämtar eller anger ett värde som indikerar om den vertikala rullningslisten är dold. |
| [OnAjaxCallFinishedClientFunction](../../aspose.cells.gridweb/mainweb/onajaxcallfinishedclientfunction/) { get; set; } | Hämtar eller anger namnet på klientsidans funktion som ska anropas när ajax‑anropet är färdigt. Klientfunktionen bör deklareras så här: function GridAjaxcallFinished() { alert(this.id+" ajaxcall finished "); } Obs: Du kan använda "this"‑pekaren i klientfunktionen för att referera till rutnätskontrollen som utlöser händelsen. |
| [OnCellErrorClientFunction](../../aspose.cells.gridweb/mainweb/oncellerrorclientfunction/) { get; set; } | Hämtar eller anger namnet på klientsidans funktion som ska anropas när en cells validering misslyckas. Klientfunktionen bör deklareras så här: function MyOnCellError(cell) { alert(this.getCellValueByCell(cell)); } Obs: Du kan använda "this"‑pekaren i klientfunktionen för att referera till rutnätskontrollen som utlöser händelsen. |
| [OnCellSelectedAjaxCallBackClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedajaxcallbackclientfunction/) { get; set; } | Hämtar eller anger klientsidans funktion som ska anropas när en cell väljs. Klientfunktionen bör deklareras så här: function MyOnSelectCellAjaxCallBack(cell,customerdata) { } Obs: Du kan använda "this"‑pekaren i klientfunktionen för att referera till rutnätskontrollen som utlöser händelsen. |
| [OnCellSelectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedclientfunction/) { get; set; } | Hämtar eller anger den klientsidiga funktionen som ska anropas när en cell är markerad. Klientfunktionen bör deklareras så här: function MyOnSelectCell(cell) { GridWeb1.setCellValueByCell(cell, "test"); }Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på gridkontrollen som utlöser händelsen. |
| [OnCellUnselectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellunselectedclientfunction/) { get; set; } | Hämtar eller anger den klientsidiga funktionen som ska anropas när en cell avmarkerats. Klientfunktionen bör deklareras så här: function MyOnUnselectCell(cell) { this.setCellValueByCell(cell, "test"); }Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på gridkontrollen som utlöser händelsen. |
| [OnCellUpdatedClientFunction](../../aspose.cells.gridweb/mainweb/oncellupdatedclientfunction/) { get; set; } | Hämtar eller anger namnet på den klientsidiga funktionen som ska anropas när en cells värde uppdateras. Klientfunktionen bör deklareras så här: function MyOnCellUpdated(cell) { alert(this.getCellValueByCell(cell)); }Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på gridkontrollen som utlöser händelsen. |
| [OnContextMenuShowClientFunction](../../aspose.cells.gridweb/mainweb/oncontextmenushowclientfunction/) { get; set; } | Hämtar eller anger den klientsidiga funktionen som ska anropas när snabbmenyn ska visas. Klientfunktionen bör deklareras så här: function onContextMenuShow() { var menu = event.srcElement; menu.setItemVisibility("Delete", "block"); menu.setItemVisibility("Update", "none"); }Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på gridkontrollen som utlöser händelsen. |
| [OnDoubleClickCellClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickcellclientfunction/) { get; set; } | Hämtar eller anger den klientsidiga funktionen som ska anropas när en cell dubbelklickas. Klientfunktionen bör deklareras så här: function MyOnDoubleClickCell(cell) { this.setCellValueByCell(cell, "test"); }Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på gridkontrollen som utlöser händelsen. |
| [OnDoubleClickRowClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickrowclientfunction/) { get; set; } | Hämtar eller anger den klientsidiga funktionen som ska anropas när en rad dubbelklickas. Klientfunktionen bör deklareras så här: function MyOnRowDoubleClick(row) { alert(row); }Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på gridkontrollen som utlöser händelsen. |
| [OnGridInitClientFunction](../../aspose.cells.gridweb/mainweb/ongridinitclientfunction/) { get; set; } | Hämtar eller anger namnet på den klientsidiga funktionen som ska anropas när griden initieras. Klientfunktionen bör deklareras så här: function MyOnGridInit(grid) { alert("The grid is initialized: " + grid.id); }Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på gridkontrollen som utlöser händelsen. |
| [OnlyAuto](../../aspose.cells.gridweb/mainweb/onlyauto/) { get; set; } | Hämtar eller anger om endast rader vars höjd inte är anpassad ska anpassas, standardvärdet är false |
| [OnPageChangeClientFunction](../../aspose.cells.gridweb/mainweb/onpagechangeclientfunction/) { get; set; } | Hämtar eller anger den klientsidiga funktionen som ska anropas efter sidindexändring. Gäller endast när EnablePaging är true. Klientfunktionen bör deklareras så här: function MyOnPageChange(index) { console.log("current page is:"+index); }Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på gridkontrollen som utlöser händelsen. |
| [OnPageSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onpagesubmitclientfunction/) { get; set; } | Hämtar eller anger klientfunktionen som ska anropas innan sidan skickas in på klientsidan. |
| [OnShapeSelectedClientFunction](../../aspose.cells.gridweb/mainweb/onshapeselectedclientfunction/) { get; set; } | Hämtar eller anger klientsidans funktion som ska anropas när en form väljs. Klientfunktionen bör deklareras så här: function MyOnSelectShape(shape) { var name=shape.getAttribute(\"namevalue\") var text=shape.getAttribute(\"textvalue\") var value=shape.getAttribute(\"controlvalue\") var type=shape.getAttribute(\"msotype\") }Obs: Du kan använda \"this\"-pekaren i klientfunktionen för att peka på grid‑kontrollen som utlöser händelsen. |
| [OnSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onsubmitclientfunction/) { get; set; } | Hämtar eller anger klientfunktionen som ska anropas innan kontrollen skickas in på klientsidan. Klientfunktionen bör deklareras så här: function MyOnSubmit(arg, cancelEdit) { return true;} Arg är inlämningsargumentet och innehåller kommandot som ska postas till servern. cancelEdit är ett booleskt värde som indikerar om kontrollen har förkastat användarens inmatning innan inlämning. Kontrollen fortsätter att skicka om funktionen returnerar true. Obs: Du kan använda \"this\"-pekaren i klientfunktionen för att peka på grid‑kontrollen som utlöser händelsen. |
| [PageSize](../../aspose.cells.gridweb/mainweb/pagesize/) { get; set; } | Hämtar eller anger sidstorleken i pagineringsläge. |
| [PresetStyle](../../aspose.cells.gridweb/mainweb/presetstyle/) { get; set; } | Hämtar eller anger den förinställda stilen. |
| [RefreshValidation](../../aspose.cells.gridweb/mainweb/refreshvalidation/) { get; set; } | Hämtar eller anger om valideringsvärdet ska uppdateras efter att cellvärdet ändras. |
| [RenderHiddenRow](../../aspose.cells.gridweb/mainweb/renderhiddenrow/) { get; set; } | Hämtar eller anger om den dolda raden renderas i GridControl, standardvärdet är false. Om du senare behöver visa den dolda raden ska du sätta den till true. |
| [RowHeightForCSV](../../aspose.cells.gridweb/mainweb/rowheightforcsv/) { get; set; } | Hämta eller ange radens höjd i punkter för CSV‑fil, standardvärdet är 14,5. |
| [ScrollBarArrowColor](../../aspose.cells.gridweb/mainweb/scrollbararrowcolor/) { get; set; } | Anger färgen på rullningslistens pilknapp. |
| [ScrollBarBaseColor](../../aspose.cells.gridweb/mainweb/scrollbarbasecolor/) { get; set; } | Anger färgen på kontrollens rullningslist. |
| [SelectCellBgColor](../../aspose.cells.gridweb/mainweb/selectcellbgcolor/) { get; set; } | Anger bakgrundsfärgen för de markerade cellerna i ett flervalsområde. |
| [SelectCellColor](../../aspose.cells.gridweb/mainweb/selectcellcolor/) { get; set; } | Anger färgen på de markerade cellerna i ett flervalsområde. |
| [SessionMode](../../aspose.cells.gridweb/mainweb/sessionmode/) { get; set; } | Hämtar eller anger sessionsläget för rutnätet. |
| [SessionStorePath](../../aspose.cells.gridweb/mainweb/sessionstorepath/) { get; set; } | Hämtar eller anger sökvägen för sessionscachelagring när sessionsläget är File eller ViewState, etc: gridweb.SessionStorePath=\"c:/mytempdir/session\"; då lagras sessionsdata i c:/mytempdir/session. |
| [Settings](../../aspose.cells.gridweb/mainweb/settings/) { get; set; } | Representerar arbetsbokens inställningar. |
| [ShowAddButton](../../aspose.cells.gridweb/mainweb/showaddbutton/) { get; set; } | Hämtar eller anger om knappen för att lägga till kalkylblad ska visas. |
| [ShowBottomBar](../../aspose.cells.gridweb/mainweb/showbottombar/) { get; set; } | Anger om kommandoraden (inklusive kommandorad och flikrad) ska visas längst ner i kontrollen. |
| [ShowCellEditBox](../../aspose.cells.gridweb/mainweb/showcelleditbox/) { get; set; } | Om Gridweb visar verktygsfältet för redigeringsrutan som i MS‑EXCEL. Om det är aktiverat visas en redigeringsruta för den aktuella cellen i Gridweb. När vi aktiverar denna funktion måste du importera jQuery‑js‑biblioteket i dina .aspx‑filer för att stödja den nya funktionen. Alla senaste jQuery‑versioner fungerar. |
| [ShowCommandBarAtTop](../../aspose.cells.gridweb/mainweb/showcommandbarattop/) { get; set; } | Anger om kommandoraden (inklusive kommandorad och flikrad) ska visas högst upp i kontrollen. |
| [ShowContextMenu](../../aspose.cells.gridweb/mainweb/showcontextmenu/) { get; set; } | Hämtar eller anger om snabbmenyn ska visas. Standardvärdet är true. |
| [ShowDefaultGridLine](../../aspose.cells.gridweb/mainweb/showdefaultgridline/) { get; set; } | Hämtar eller anger om cellernas standardrutnätslinjer ska visas. |
| [ShowHeaderBar](../../aspose.cells.gridweb/mainweb/showheaderbar/) { get; set; } | Hämtar eller anger om rubrikraden ska visas |
| [ShowLoading](../../aspose.cells.gridweb/mainweb/showloading/) { get; set; } | Anger om en laddningsdialogruta ska visas under postback till servern. |
| [ShowLoadingPosition](../../aspose.cells.gridweb/mainweb/showloadingposition/) { get; set; } | Anger den vänstra och övre positionen (i px) för att visa laddningsdialogrutan under postback till servern, etc. 100,200 betyder att laddningsdialogrutans vänstra och övre position är 100 px, 200 px. |
| [ShowSaveButton](../../aspose.cells.gridweb/mainweb/showsavebutton/) { get; set; } | Hämtar eller anger om spara‑knappen ska visas. |
| [ShowSubmitButton](../../aspose.cells.gridweb/mainweb/showsubmitbutton/) { get; set; } | Hämtar eller anger om skicka‑knappen ska visas. |
| [ShowTabBar](../../aspose.cells.gridweb/mainweb/showtabbar/) { get; set; } | Hämtar eller anger om flikraden ska visas. |
| [ShowTabNavigation](../../aspose.cells.gridweb/mainweb/showtabnavigation/) { get; set; } | Hämtar eller anger om fliknavigationsknappen ska visas, standardvärdet är true. |
| [ShowUndoButton](../../aspose.cells.gridweb/mainweb/showundobutton/) { get; set; } | Hämtar eller anger om ångra‑knappen ska visas. |
| [SpanWrap](../../aspose.cells.gridweb/mainweb/spanwrap/) { get; set; } | Anger om innehållet ska radbrytas i cellspannet. Standardvärdet är true. |
| [TabStyle](../../aspose.cells.gridweb/mainweb/tabstyle/) { get; set; } | Hämtar eller anger stilen för flikfältet. |
| [UseClientPageHeight](../../aspose.cells.gridweb/mainweb/useclientpageheight/) { get; set; } | Hämtar eller anger om GridWeb använder klientens sidhöjd som kontrollhöjd, lämpligt när Height="100%" är satt, standardvärdet är false. |
| [ViewPanelScrollLeft](../../aspose.cells.gridweb/mainweb/viewpanelscrollleft/) { get; set; } | Hämtar eller anger positionen för rullningslisten i rutnätets visningspanel. |
| [ViewPanelScrollTop](../../aspose.cells.gridweb/mainweb/viewpanelscrolltop/) { get; set; } | Hämtar eller anger positionen för rullningslisten i rutnätets visningspanel. |
| [ViewTableStyle](../../aspose.cells.gridweb/mainweb/viewtablestyle/) { get; set; } | Hämtar eller anger stilen för datavisningspanelen. |
| [WebWorksheets](../../aspose.cells.gridweb/mainweb/webworksheets/) { get; } |  |
| override [Width](../../aspose.cells.gridweb/mainweb/width/) { get; set; } | Hämtar eller anger bredden (System.Web.UI.WebControl.Unit) för kontrollen. |
| [WorkSheets](../../aspose.cells.gridweb/mainweb/worksheets/) { get; } | Hämtar eller anger samlingen av kalkylblad. |
| [XhtmlMode](../../aspose.cells.gridweb/mainweb/xhtmlmode/) { get; set; } | Hämtar eller anger om XHTML-stil ska användas, standardvärdet är true. |
| static [DPI](../../aspose.cells.gridweb/mainweb/dpi/) { get; set; } | Hämtar / anger DPI för maskinen. |
| static [PictureCachePath](../../aspose.cells.gridweb/mainweb/picturecachepath/) { get; set; } | Hämtar eller anger bildlagringssökvägen för arbetsboken, alla former och bilder lagras i denna katalog, standardvägen är acwcache under den aktuella applikationens baskatalog. Användare måste implementera en schemalagd tjänst för att rensa filer som har gått utanför sessionstiden. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [CalculateFormula](../../aspose.cells.gridweb/mainweb/calculateformula/)() | Beräknar resultatet av formler. |
| override [DataBind](../../aspose.cells.gridweb/mainweb/databind/)() | Bind kontrollen och alla dess underkontroller till dess datakälla. |
| override [Dispose](../../aspose.cells.gridweb/mainweb/dispose/)() |  |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile)(Stream) | Importerar från en Excel-filström, inklusive filström från disk eller minnesström. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile_2)(string) | Importerar från en Excel-fil. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile_1)(Stream, string) | Importerar från en Excel-filström, inklusive filström från disk eller minnesström. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile_3)(string, string) | Importerar från en Excel-fil. |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile/#loadcsvfile)(Stream) | Läser in data från en CSV-filström. |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile/#loadcsvfile_1)(string) | Läser in data från en CSV-fil. |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile/#loadhtmlfile)(Stream) | Läser in data från en HTML-filström. |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile/#loadhtmlfile_1)(string) | Läser in data från en HTML-fil. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile/#loadspreadsheetmlfile)(Stream) | Läser in data från en SpreadSheetML-filström. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile/#loadspreadsheetmlfile_1)(string) | Läser in data från en SpreadSheetML-fil. |
| [RefreshChartShape](../../aspose.cells.gridweb/mainweb/refreshchartshape/)() | Uppdatera alla diagrambilder för det aktiva kalkylbladet. |
| override [RenderBeginTag](../../aspose.cells.gridweb/mainweb/renderbegintag/)(HtmlTextWriter) |  |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile/#savecsvfile)(Stream) | Sparar data till en CSV-filström. |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile/#savecsvfile_1)(string) | Sparar data till en CSV-fil. |
| [SaveCustomStyleFile](../../aspose.cells.gridweb/mainweb/savecustomstylefile/)(string) | Sparar aktuell stildata för kontrollen till en XML-fil. Kan användas för att skapa din anpassade stilfil. |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile/#savehtmlfile)(Stream) | Sparar data till en HTML-filström. |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile/#savehtmlfile_1)(string) | Sparar data till en HTML-fil. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile/#savespreadsheetmlfile)(Stream) | Sparar data till en SpreadSheetML-filström. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile/#savespreadsheetmlfile_1)(string) | Sparar data till en SpreadSheetML-fil. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile)(Stream) | Sparar arbetsbladen till en excel-fil. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_3)(string) | Sparar arbetsbladen till en excel-fil i Excel 2003-format. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_1)(Stream, GridSaveFormat) | Sparar arbetsbladen till en excel-fil. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_2)(Stream, GridSaveOptions) | Sparar arbetsbladen till en excel-fil. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_4)(string, GridSaveFormat) | Sparar arbetsbladen till en excel-fil. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_5)(string, GridSaveOptions) | Sparar arbetsbladen till en excel-fil. |
| [SetCustomStyle](../../aspose.cells.gridweb/mainweb/setcustomstyle/)(Stream) | Anger den anpassade stilfilen från en ström, inklusive filströmmar på disk eller minnesströmmar. |

## Händelser

| Namn | Beskrivning |
| --- | --- |
| event [AfterColumnFilter](../../aspose.cells.gridweb/mainweb/aftercolumnfilter/) | Inträffar efter att kolumnen har filtrerats. |
| event [AjaxCallFinished](../../aspose.cells.gridweb/mainweb/ajaxcallfinished/) | Utlöses när AJAX-uppdateringen av kontrollen är klar (EnableAJAX ska vara satt till true). |
| event [BeforeColumnFilter](../../aspose.cells.gridweb/mainweb/beforecolumnfilter/) | Inträffar innan kolumnen filtreras. |
| event [CellClickOnAjax](../../aspose.cells.gridweb/mainweb/cellclickonajax/) | Inträffar när cellen klickas, och ett AJAX-återanrop behövs för denna händelse. |
| event [CellClientUpdate](../../aspose.cells.gridweb/mainweb/cellclientupdate/) | Inträffar när en klientcelluppdatering sker. När denna händelse utlöses innehåller dess parameter e.Argument kommandots namn. |
| event [CellCommand](../../aspose.cells.gridweb/mainweb/cellcommand/) | Inträffar när en cells kommandolänk klickas. När denna händelse utlöses innehåller dess parameter e.Argument kommandots namn. |
| event [CellDoubleClick](../../aspose.cells.gridweb/mainweb/celldoubleclick/) | Inträffar när cellen dubbelklickas. |
| event [CellError](../../aspose.cells.gridweb/mainweb/cellerror/) | Inträffar när ett inmatningsvärdesfel i cellen uppstår. |
| event [CellModifiedOnAjax](../../aspose.cells.gridweb/mainweb/cellmodifiedonajax/) | Inträffar när cellen ändras i ett AJAX-anrop. |
| event [ColumnDeleted](../../aspose.cells.gridweb/mainweb/columndeleted/) | Inträffar när användaren tar bort en kolumn från klientmenyn. |
| event [ColumnDeleting](../../aspose.cells.gridweb/mainweb/columndeleting/) | Inträffar när användaren försöker ta bort en kolumn från klientmenyn. Du kan hantera denna händelse och sätta avbrytparametern till True för att avbryta borttagningsoperationen. |
| event [ColumnDoubleClick](../../aspose.cells.gridweb/mainweb/columndoubleclick/) | Uppstår när kolumnrubriken dubbelklickas. |
| event [ColumnInserted](../../aspose.cells.gridweb/mainweb/columninserted/) | Uppstår när användaren infogar en kolumn från klientmenyn. |
| event [CustomCommand](../../aspose.cells.gridweb/mainweb/customcommand/) | Uppstår när användaren klickar på en anpassad kommandoknapp. |
| event [LoadCustomData](../../aspose.cells.gridweb/mainweb/loadcustomdata/) | Utlöses när kontrollens SessionMode är inställd på Custom och behöver ladda bladdata. Du kan hantera denna händelse i Custom Session-läge för att ladda bladdata från fil eller databas. |
| event [PageIndexChanged](../../aspose.cells.gridweb/mainweb/pageindexchanged/) | Uppstår när kontrollens bladsidindex ändrades. |
| event [RowDeleted](../../aspose.cells.gridweb/mainweb/rowdeleted/) | Uppstår när användaren har raderat en rad från klientmenyn. |
| event [RowDeleting](../../aspose.cells.gridweb/mainweb/rowdeleting/) | Uppstår när användaren försöker radera en rad från klientmenyn. Du kan hantera denna händelse och kasta ett RejectDeleteException‑undantag för att avbryta en raderingsoperation. |
| event [RowDoubleClick](../../aspose.cells.gridweb/mainweb/rowdoubleclick/) | Uppstår när radrubriken dubbelklickas. |
| event [RowInserted](../../aspose.cells.gridweb/mainweb/rowinserted/) | Uppstår när användaren infogar en rad från klientmenyn. |
| event [SaveCommand](../../aspose.cells.gridweb/mainweb/savecommand/) | Uppstår när "save"-knappen klickas. |
| event [SheetAdded](../../aspose.cells.gridweb/mainweb/sheetadded/) | Uppstår när användaren lägger till ett arbetsblad från verktygsmenyn. |
| event [SheetDataUpdated](../../aspose.cells.gridweb/mainweb/sheetdataupdated/) | Uppstår när kontrollen har laddat de postade data och uppdaterat bladdata. |
| event [SheetTabClick](../../aspose.cells.gridweb/mainweb/sheettabclick/) | Uppstår när bladfliken klickas. |
| event [SubmitCommand](../../aspose.cells.gridweb/mainweb/submitcommand/) | Uppstår när "submit"-knappen klickas. |
| event [UndoCommand](../../aspose.cells.gridweb/mainweb/undocommand/) | Uppstår när "undo"-knappen klickas. |

### Exempel

```csharp
[C#]
	GridWeb GridWeb1 = new GridWeb();
//utför din verksamhet
```

### Se även

* class [ExtWebControl](../extwebcontrol/)
* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


