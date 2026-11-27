---
title: "Klass GridDesktop"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridDesktop.GridDesktop-klass. Aspose GridDesktop-klass representerar ett rotobjekt för att skapa en GridDesktop-kontroll. För att använda denna kontroll drar du helt enkelt den från verktygslådan till ett formulär eller en användarkontroll."
type: docs
url: /sv/net/aspose.cells.griddesktop/griddesktop/
---
## GridDesktop class

Aspose GridDesktop class representerar ett rotobjekt för att skapa en GridDesktop‑kontroll. För att använda denna kontroll, dra den helt enkelt från verktygslådan till ett formulär eller en användarkontroll.

```csharp
public class GridDesktop : UserControl
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [GridDesktop](griddesktop/)() | Aspose GridDesktop-klass |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells.griddesktop/griddesktop/activesheetindex/) { get; set; } | Hämtar eller anger det valda bladindexet. |
| [ActiveSheetNameFont](../../aspose.cells.griddesktop/griddesktop/activesheetnamefont/) { get; set; } | Hämtar eller anger det aktiva bladets teckensnitt i bladfältet. |
| [AlwasysRecalculateAllFormulas](../../aspose.cells.griddesktop/griddesktop/alwasysrecalculateallformulas/) { get; set; } | Hämtar eller anger ett värde som indikerar om vi behöver köra alla formler, som när vi kör alla formler, när en cellvärde uppdateras, och det påverkar andra, och andra påverkar andra, mer och mer, vilket får att hela cellerna måste omberäknas, precis som fjärilseffekten, det kräver många stackoperationer, det ger mycket låg prestanda, som i CELLSNET-41921, detta problem innehåller den fil som kan visa detta scenario, vi bör hellre bara köra alla formler, eftersom när vi kör alla formler kan vi ha viss optimering. |
| [BorderStyle](../../aspose.cells.griddesktop/griddesktop/borderstyle/) { get; set; } | Anger kantstilen för kontrollen. |
| [ColumnHeaderVisible](../../aspose.cells.griddesktop/griddesktop/columnheadervisible/) { get; set; } | Hämtar eller anger ett värde som indikerar om kolumnrubriken är synlig. |
| [CommentDisplayingFont](../../aspose.cells.griddesktop/griddesktop/commentdisplayingfont/) { get; set; } | Hämtar eller anger standardteckensnittet för visning av kommentartext. |
| [ContextMenuManager](../../aspose.cells.griddesktop/griddesktop/contextmenumanager/) { get; } | Hämtar ContextMenuManager-instansen. |
| [DefaultCellFont](../../aspose.cells.griddesktop/griddesktop/defaultcellfont/) { get; set; } | Hämtar eller anger standardteckensnittet för cellen |
| [DefaultCellFontColor](../../aspose.cells.griddesktop/griddesktop/defaultcellfontcolor/) { get; set; } | Hämtar eller anger standardteckensnittsfärgen för cellen. |
| [EnableClipboardCopyPaste](../../aspose.cells.griddesktop/griddesktop/enableclipboardcopypaste/) { get; set; } | Anger om kopiering/klistring ska baseras på urklipp, så att det kan kopiera/klistra med MS-EXCEL. Det kopierar/endast klistrar cellvärdet, det kopierar inte några andra inställningar för cellen som format, kantstil osv. Standardvärdet är falskt. |
| [EnableCopyWithExtension](../../aspose.cells.griddesktop/griddesktop/enablecopywithextension/) { get; set; } | Hämtar eller anger ett värde som indikerar om kopieringsoperationen ska utöka antalet rader eller kolumner. |
| [EnableCopyWithLockedOption](../../aspose.cells.griddesktop/griddesktop/enablecopywithlockedoption/) { get; set; } | Hämtar eller anger ett värde som indikerar om kopieringsoperationen ska kopiera stilens CellLocked-attributvärde för en cell. |
| [EnableUndo](../../aspose.cells.griddesktop/griddesktop/enableundo/) { get; set; } | Hämtar eller anger ett värde som indikerar om Undo-funktionen är aktiverad. Standardvärdet är falskt. |
| [GridMemorySetting](../../aspose.cells.griddesktop/griddesktop/gridmemorysetting/) { get; set; } | Hämtar eller anger minnesalternativ, standardvärdet är GridMemorySetting.Normal |
| [IsHorizontalScrollBarVisible](../../aspose.cells.griddesktop/griddesktop/ishorizontalscrollbarvisible/) { get; set; } | Ställer in synligt tillstånd för Horizontal ScrollBar. |
| [IsVerticalScrollBarVisible](../../aspose.cells.griddesktop/griddesktop/isverticalscrollbarvisible/) { get; set; } | Ställer in synligt tillstånd för Vertical ScrollBar. |
| [Names](../../aspose.cells.griddesktop/griddesktop/names/) { get; } | Hämtar samlingen av alla Name-objekt i kalkylarket. |
| [PageRows](../../aspose.cells.griddesktop/griddesktop/pagerows/) { get; set; } | Ställer in eller hämtar radstorlek för paginering. Det maximala antalet PageRows som stöds är 100000, det maximala sidantalet som stöds är 5000. |
| [PasteType](../../aspose.cells.griddesktop/griddesktop/pastetype/) { get; set; } | Anger vilken klistringstyp som används vid klistringsåtgärd, endast tillgänglig när EnableClipboardCopyPaste är falskt. Standardvärdet är GridPasteType.Default; |
| [R1C1](../../aspose.cells.griddesktop/griddesktop/r1c1/) { get; set; } | Hämtar eller anger ett värde som indikerar om kontrollen använder R1C1-referensstil. |
| [RecalculateFormulas](../../aspose.cells.griddesktop/griddesktop/recalculateformulas/) { get; set; } | Hämtar eller anger ett värde som indikerar om alla cellers formler ska omberäknas när en cells värde ändras. Standardvärdet är true. |
| [RowHeaderVisible](../../aspose.cells.griddesktop/griddesktop/rowheadervisible/) { get; set; } | Hämtar eller anger ett värde som indikerar om radhuvudet är synligt. |
| [SheetNameFont](../../aspose.cells.griddesktop/griddesktop/sheetnamefont/) { get; set; } | Hämtar eller anger standardteckensnittet för visning i bladfältet. |
| [SheetsBarVisible](../../aspose.cells.griddesktop/griddesktop/sheetsbarvisible/) { get; set; } | Hämtar eller anger ett värde som indikerar om bladfältet är synligt. |
| [SheetTabWidth](../../aspose.cells.griddesktop/griddesktop/sheettabwidth/) { get; set; } | Ställer in / Hämtar bredden på Sheet Tab. |
| [ShowContextMenu](../../aspose.cells.griddesktop/griddesktop/showcontextmenu/) { get; set; } | Hämtar eller anger ett värde som indikerar om kontrollen kan visa snabbmenyn. |
| [ShowFormulaWarning](../../aspose.cells.griddesktop/griddesktop/showformulawarning/) { get; set; } | Ställer in/Hämtar om fel- eller varningsmeddelandet ska visas för angivet cellformelvärde, standardvärdet är true. |
| [ShowNumberStoredAsTextSymbol](../../aspose.cells.griddesktop/griddesktop/shownumberstoredastextsymbol/) { get; set; } | Ställer in / Hämtar om triangelsymbolen ska visas för cellen som innehåller en siffra som textformat. |
| [ShowStatus](../../aspose.cells.griddesktop/griddesktop/showstatus/) { get; set; } | Hämtar eller anger ett värde som indikerar om beräkningsstatusen ska visas. Standardvärdet är true. |
| [UndoManager](../../aspose.cells.griddesktop/griddesktop/undomanager/) { get; } | Hämtar UndoManager-instansen. |
| [Worksheets](../../aspose.cells.griddesktop/griddesktop/worksheets/) { get; } | Hämtar Worksheets. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Clear](../../aspose.cells.griddesktop/griddesktop/clear/)() | Rensar GridDesktop-kontrollen. |
| [Copy](../../aspose.cells.griddesktop/griddesktop/copy/)() | Kopierar fokuserat cellinnehåll till urklipp. |
| [Cut](../../aspose.cells.griddesktop/griddesktop/cut/)() | Klipper ut fokuserat cellinnehåll till urklipp. |
| [DoSplit](../../aspose.cells.griddesktop/griddesktop/dosplit/)() | Ställer in delad vy. |
| [EndFormatPainter](../../aspose.cells.griddesktop/griddesktop/endformatpainter/)() | Meddelar GridDesktop att avsluta FormatPainter. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile)(Stream) | Exporterar till en excel‑filström, inklusive disk‑IO‑ström eller minnesström. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile_2)(string) | Exporterar till en excel‑fil. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile_1)(Stream, FileFormatType) | Exporterar till en excel‑filström, inklusive disk‑IO‑ström eller minnesström. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile_3)(string, FileFormatType) | Exporterar till en excel‑fil. |
| [ExportPdfFile](../../aspose.cells.griddesktop/griddesktop/exportpdffile/#exportpdffile)(Stream, GridPdfSaveOptions) | Exporterar till en pdf‑filström, inklusive disk‑IO‑ström eller minnesström. |
| [ExportPdfFile](../../aspose.cells.griddesktop/griddesktop/exportpdffile/#exportpdffile_1)(string, GridPdfSaveOptions) | Exporterar till en pdf‑filström, inklusive disk‑IO‑ström eller minnesström. |
| [GetActiveWorksheet](../../aspose.cells.griddesktop/griddesktop/getactiveworksheet/)() | Hämtar aktuellt aktivt kalkylblad. |
| [getHScrollBar](../../aspose.cells.griddesktop/griddesktop/gethscrollbar/)() | returnera horisontell rullningslist |
| [getVScrollBar](../../aspose.cells.griddesktop/griddesktop/getvscrollbar/)() | returnera vertikal rullningslist |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile)(Stream) | Importerar från en Excel-filström, inklusive filström från disk eller minnesström. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_3)(string) | Importerar från en Excel-fil. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_1)(Stream, bool) | Importerar från en Excel-filström, inklusive filström från disk eller minnesström. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_4)(string, bool) | Importerar från en Excel-fil. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_5)(string, int) | Importerar ett kalkylblad från en excel‑fil. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_2)(Stream, string, string, bool, bool) | Importerar från en Excel-fil. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_6)(string, string, string, bool, bool) | Importerar från en Excel-fil. |
| [Invalidate](../../aspose.cells.griddesktop/griddesktop/invalidate/#invalidate)() | Åsidosätt ogiltigförklaring. |
| [OpenFindReplaceDialog](../../aspose.cells.griddesktop/griddesktop/openfindreplacedialog/)(bool) | Öppnar FindReplace‑dialogen för att hitta eller ersätta celler. |
| [Paste](../../aspose.cells.griddesktop/griddesktop/paste/)() | Klistrar in urklippsinnehåll i den fokuserade cellen. |
| [RefreshControl](../../aspose.cells.griddesktop/griddesktop/refreshcontrol/)() | Uppdatera GridDesktop‑kontrollen. |
| [RunAllFormulas](../../aspose.cells.griddesktop/griddesktop/runallformulas/)() | Kör alla cellers formler. |
| [SetAllScrollBarsVisible](../../aspose.cells.griddesktop/griddesktop/setallscrollbarsvisible/)() | Ställer in alla rullningslister som synliga. |
| [SetCustomResourceManager](../../aspose.cells.griddesktop/griddesktop/setcustomresourcemanager/)(ResourceManager) | Ställ in anpassad resurs‑hanterare för att implementera användardefinierad lokalisering |
| [ShowStyleDialog](../../aspose.cells.griddesktop/griddesktop/showstyledialog/)() | Öppnar en stil‑dialog, för att ange cellstil, teckensnitt, färger etc. |
| [StartFormatPainter](../../aspose.cells.griddesktop/griddesktop/startformatpainter/)(bool) | Meddelar GridDesktop att starta FormatPainter. |
| [UnDoSplit](../../aspose.cells.griddesktop/griddesktop/undosplit/)() | Inaktivera delad vy. |
| static [GetVersion](../../aspose.cells.griddesktop/griddesktop/getversion/)() | Hämta utgivningsversionen. |

## Fält

| Namn | Beskrivning |
| --- | --- |
| [LoadDataFilter](../../aspose.cells.griddesktop/griddesktop/loaddatafilter/) | alternativen för att filtrera data när arbetsboken laddas från mall. |
| [ShowImportMessage](../../aspose.cells.griddesktop/griddesktop/showimportmessage/) | om ett meddelandefönster ska visas när import av filen misslyckas, standardvärdet är true |

## Händelser

| Namn | Beskrivning |
| --- | --- |
| event [AfterDeleteColumns](../../aspose.cells.griddesktop/griddesktop/afterdeletecolumns/) | Uppstår efter att en kolumn har raderats. |
| event [AfterDeleteRows](../../aspose.cells.griddesktop/griddesktop/afterdeleterows/) | Uppstår efter att en rad har raderats. |
| event [AfterInsertColumns](../../aspose.cells.griddesktop/griddesktop/afterinsertcolumns/) | Uppstår efter att en ny kolumn har infogats. |
| event [AfterInsertRows](../../aspose.cells.griddesktop/griddesktop/afterinsertrows/) | Uppstår efter att en ny rad har infogats. |
| event [BeforeCalculate](../../aspose.cells.griddesktop/griddesktop/beforecalculate/) | Uppstår innan formel beräknas i arbetsboken. |
| event [BeforeLoadFile](../../aspose.cells.griddesktop/griddesktop/beforeloadfile/) | Uppstår innan arbetsboken laddas från fil. |
| event [CellButtonClick](../../aspose.cells.griddesktop/griddesktop/cellbuttonclick/) | Uppstår när cellknappen klickas. |
| event [CellCheckedChanged](../../aspose.cells.griddesktop/griddesktop/cellcheckedchanged/) | Uppstår när cellens kryssruta Checked-egenskap ändras. |
| event [CellClick](../../aspose.cells.griddesktop/griddesktop/cellclick/) | Uppstår när gridcellen klickas. |
| event [CellComboBoxCopy](../../aspose.cells.griddesktop/griddesktop/cellcomboboxcopy/) | Uppstår när en grid cell ComboBox kopieras. |
| event [CellDataChanged](../../aspose.cells.griddesktop/griddesktop/celldatachanged/) | Uppstår när gridcellens dataegenskap ändras. |
| event [CellDoubleClick](../../aspose.cells.griddesktop/griddesktop/celldoubleclick/) | Uppstår när gridcellen dubbelklickas. |
| event [CellFormatChanged](../../aspose.cells.griddesktop/griddesktop/cellformatchanged/) | Uppstår när cellformatet ändras via dialogrutan Format Cells. |
| event [CellKeyPressed](../../aspose.cells.griddesktop/griddesktop/cellkeypressed/) | Uppstår när en tangent trycks ned medan en cell har fokus. |
| event [CellSelectedIndexChanged](../../aspose.cells.griddesktop/griddesktop/cellselectedindexchanged/) | Uppstår när cellens combobox SelectedIndex-egenskap har ändrats. |
| event [CellTextBoxChanging](../../aspose.cells.griddesktop/griddesktop/celltextboxchanging/) | Uppstår när tecken skrivs i en gridcell. |
| event [CellValidationFailed](../../aspose.cells.griddesktop/griddesktop/cellvalidationfailed/) | Uppstår när en gridcell misslyckas med validering. |
| event [ColumnHeaderClick](../../aspose.cells.griddesktop/griddesktop/columnheaderclick/) | Uppstår när kolumnrubriken klickas. |
| event [ColumnHeaderDoubleClick](../../aspose.cells.griddesktop/griddesktop/columnheaderdoubleclick/) | Uppstår när kolumnrubriken dubbelklickas. |
| event [CommentDataChanged](../../aspose.cells.griddesktop/griddesktop/commentdatachanged/) | Uppstår när kommentarsdata har ändrats. |
| event [FailLoadFile](../../aspose.cells.griddesktop/griddesktop/failloadfile/) |  |
| event [FinishCalculate](../../aspose.cells.griddesktop/griddesktop/finishcalculate/) | Uppstår efter att formeln beräknats i arbetsboken. |
| event [FinishLoadFile](../../aspose.cells.griddesktop/griddesktop/finishloadfile/) | Uppstår när arbetsboken laddas. |
| event [FocusedCellChanged](../../aspose.cells.griddesktop/griddesktop/focusedcellchanged/) | Uppstår när den fokuserade cellen ändras. |
| event [PictureClick](../../aspose.cells.griddesktop/griddesktop/pictureclick/) | Uppstår när formen klickas. |
| event [RowColumnHiddenChanged](../../aspose.cells.griddesktop/griddesktop/rowcolumnhiddenchanged/) | Uppstår när rad-/kolumnens dolda status ändras. |
| event [RowFilteredEvent](../../aspose.cells.griddesktop/griddesktop/rowfilteredevent/) | Uppstår efter att radfilterobjektet har valts. |
| event [RowHeaderClick](../../aspose.cells.griddesktop/griddesktop/rowheaderclick/) | Uppstår när radrubriken klickas. |
| event [RowHeaderDoubleClick](../../aspose.cells.griddesktop/griddesktop/rowheaderdoubleclick/) | Uppstår när radrubriken dubbelklickas. |
| event [SelectedCellRangeChanged](../../aspose.cells.griddesktop/griddesktop/selectedcellrangechanged/) | Uppstår när det valda cellområdet ändras. |
| event [SelectedSheetIndexChanged](../../aspose.cells.griddesktop/griddesktop/selectedsheetindexchanged/) | Uppstår när SelectedSheetIndex-egenskapen ändras. |
| event [ShapeClick](../../aspose.cells.griddesktop/griddesktop/shapeclick/) | Uppstår när formen klickas. |

### Anmärkningar

Vänligen se .NET SDK-dokumentet för mer information om System.Windows.Forms.UserControl.

### Exempel

```csharp
[C#]
gridDesktop1.Worksheets[0].Cells[0, 0].Value = "2";
gridDesktop1.Worksheets[0].Cells[1, 0].Value = "3";
gridDesktop1.Worksheets[0].Cells[2, 1].Value = "=a1*a2";
gridDesktop1.RunAllFormulas();
gridDesktop1.Invalidate();

[Visual Basic]
gridDesktop1.Worksheets(0).Cells(0, 0).Value = "2"
gridDesktop1.Worksheets(0).Cells(1, 0).Value = "3"
gridDesktop1.Worksheets(0).Cells(2, 1).Value = "=a1*a2"
gridDesktop1.RunAllFormulas()
gridDesktop1.Invalidate()

```

### Se även

* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


