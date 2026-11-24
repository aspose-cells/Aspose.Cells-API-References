---
title: "Klasse GridDesktop"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridDesktop.GridDesktop Klasse. Aspose GridDesktop Klasse stellt ein Root-Objekt dar, um ein GridDesktop-Steuerelement zu erstellen. Um dieses Steuerelement zu verwenden, ziehen Sie es einfach aus Ihrer Toolbox auf ein Formular oder UserControl."
type: docs
url: /de/net/aspose.cells.griddesktop/griddesktop/
---
## GridDesktop class

Aspose GridDesktop Klasse stellt ein Root-Objekt zum Erstellen eines GridDesktop-Steuerelements dar. Um dieses Steuerelement zu verwenden, ziehen Sie es einfach aus Ihrer Toolbox auf ein Formular oder UserControl.

```csharp
public class GridDesktop : UserControl
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [GridDesktop](griddesktop/)() | Aspose GridDesktop Klasse |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells.griddesktop/griddesktop/activesheetindex/) { get; set; } | Liest oder setzt den Index des ausgewählten Blatts. |
| [ActiveSheetNameFont](../../aspose.cells.griddesktop/griddesktop/activesheetnamefont/) { get; set; } | Liest oder setzt die Schriftart der aktiven Blattanzeige in der Blattleiste. |
| [AlwasysRecalculateAllFormulas](../../aspose.cells.griddesktop/griddesktop/alwasysrecalculateallformulas/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob wir alle Formeln ausführen müssen, wie wenn wir alle Formeln ausführen, wenn ein Zellenwert aktualisiert wird und er andere beeinflusst, und andere wiederum weitere beeinflussen, immer mehr, wodurch alle Zellen neu berechnet werden müssen, ähnlich dem Schmetterlingseffekt, es erfordert viele Stack-Operationen, die Leistung wird sehr niedrig, wie in CELLSNET-41921, dieses Problem enthält die Datei, die dieses Szenario zeigt; wir sollten besser einfach alle Formeln ausführen, da wir bei der Ausführung aller Formeln möglicherweise Optimierungen haben. |
| [BorderStyle](../../aspose.cells.griddesktop/griddesktop/borderstyle/) { get; set; } | Gibt den Rahmenstil für das Steuerelement an. |
| [ColumnHeaderVisible](../../aspose.cells.griddesktop/griddesktop/columnheadervisible/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob die Spaltenüberschrift sichtbar ist. |
| [CommentDisplayingFont](../../aspose.cells.griddesktop/griddesktop/commentdisplayingfont/) { get; set; } | Liest oder setzt die standardmäßig angezeigte Schriftart des Kommentartexts. |
| [ContextMenuManager](../../aspose.cells.griddesktop/griddesktop/contextmenumanager/) { get; } | Liest die ContextMenuManager-Instanz. |
| [DefaultCellFont](../../aspose.cells.griddesktop/griddesktop/defaultcellfont/) { get; set; } | Liest oder setzt die Standardschriftart der Zelle |
| [DefaultCellFontColor](../../aspose.cells.griddesktop/griddesktop/defaultcellfontcolor/) { get; set; } | Liest oder setzt die Standard-Schriftfarbe der Zelle. |
| [EnableClipboardCopyPaste](../../aspose.cells.griddesktop/griddesktop/enableclipboardcopypaste/) { get; set; } | Gibt an, ob Kopieren/Einfügen basierend auf der Zwischenablage erfolgen soll, sodass es mit MS-EXCEL kopieren/einfügen kann. Es kopiert/fügt nur den Zellenwert ein, es kopiert keine anderen Zelleneinstellungen wie Format, Rahmenstil usw. Der Standardwert ist false. |
| [EnableCopyWithExtension](../../aspose.cells.griddesktop/griddesktop/enablecopywithextension/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob der Kopiervorgang die Anzahl der Zeilen oder Spalten erweitert. |
| [EnableCopyWithLockedOption](../../aspose.cells.griddesktop/griddesktop/enablecopywithlockedoption/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob der Kopiervorgang den CellLocked-Attributwert des Zellstils kopiert. |
| [EnableUndo](../../aspose.cells.griddesktop/griddesktop/enableundo/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob die Undo‑Funktion aktiviert ist. Der Standardwert ist false. |
| [GridMemorySetting](../../aspose.cells.griddesktop/griddesktop/gridmemorysetting/) { get; set; } | Liest oder setzt die Speicheroption, der Standardwert ist GridMemorySetting.Normal |
| [IsHorizontalScrollBarVisible](../../aspose.cells.griddesktop/griddesktop/ishorizontalscrollbarvisible/) { get; set; } | Setzt die Sichtbarkeit für die horizontale Bildlaufleiste. |
| [IsVerticalScrollBarVisible](../../aspose.cells.griddesktop/griddesktop/isverticalscrollbarvisible/) { get; set; } | Setzt die Sichtbarkeit für die vertikale Bildlaufleiste. |
| [Names](../../aspose.cells.griddesktop/griddesktop/names/) { get; } | Ruft die Sammlung aller Name‑Objekte im Tabellenblatt ab. |
| [PageRows](../../aspose.cells.griddesktop/griddesktop/pagerows/) { get; set; } | Setzt oder liest die Zeilengröße für die Paginierung. Das Maximum unterstützter PageRows beträgt 100000, das Maximum unterstützter Seitenzahlen beträgt 5000. |
| [PasteType](../../aspose.cells.griddesktop/griddesktop/pastetype/) { get; set; } | Gibt an, welcher Einfügetyp bei einer Einfügeaktion verwendet wird, nur verfügbar, wenn EnableClipboardCopyPaste false ist. Der Standardwert ist GridPasteType.Default; |
| [R1C1](../../aspose.cells.griddesktop/griddesktop/r1c1/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob die Steuerung den R1C1-Referenzstil verwendet. |
| [RecalculateFormulas](../../aspose.cells.griddesktop/griddesktop/recalculateformulas/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob alle Formeln der Zellen neu berechnet werden sollen, wenn sich der Wert einer Zelle ändert. Der Standardwert ist true. |
| [RowHeaderVisible](../../aspose.cells.griddesktop/griddesktop/rowheadervisible/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob die Zeilenüberschrift sichtbar ist. |
| [SheetNameFont](../../aspose.cells.griddesktop/griddesktop/sheetnamefont/) { get; set; } | Liest oder setzt die standardmäßig angezeigte Schriftart der Blattleiste. |
| [SheetsBarVisible](../../aspose.cells.griddesktop/griddesktop/sheetsbarvisible/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob die Blattleiste sichtbar ist. |
| [SheetTabWidth](../../aspose.cells.griddesktop/griddesktop/sheettabwidth/) { get; set; } | Setzt/Liest die Breite des Blattregisters. |
| [ShowContextMenu](../../aspose.cells.griddesktop/griddesktop/showcontextmenu/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob die Steuerung das Kontextmenü anzeigen kann. |
| [ShowFormulaWarning](../../aspose.cells.griddesktop/griddesktop/showformulawarning/) { get; set; } | Setzt/Liest, ob die Fehlermeldung oder Warnmeldung für das Setzen des Zellformelwerts angezeigt wird, der Standardwert ist true. |
| [ShowNumberStoredAsTextSymbol](../../aspose.cells.griddesktop/griddesktop/shownumberstoredastextsymbol/) { get; set; } | Setzt/Liest, ob das Dreieckssymbol für Zellen angezeigt wird, die Zahlen als Text gespeichert enthalten. |
| [ShowStatus](../../aspose.cells.griddesktop/griddesktop/showstatus/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob der Berechnungsstatus angezeigt wird. Der Standardwert ist true. |
| [UndoManager](../../aspose.cells.griddesktop/griddesktop/undomanager/) { get; } | Liest die UndoManager-Instanz. |
| [Worksheets](../../aspose.cells.griddesktop/griddesktop/worksheets/) { get; } | Liest die Arbeitsblätter. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Clear](../../aspose.cells.griddesktop/griddesktop/clear/)() | Löscht die GridDesktop-Steuerung. |
| [Copy](../../aspose.cells.griddesktop/griddesktop/copy/)() | Kopiert den Inhalt der fokussierten Zelle in die Zwischenablage. |
| [Cut](../../aspose.cells.griddesktop/griddesktop/cut/)() | Schneidet den Inhalt der fokussierten Zelle in die Zwischenablage. |
| [DoSplit](../../aspose.cells.griddesktop/griddesktop/dosplit/)() | Setzt die geteilte Ansicht. |
| [EndFormatPainter](../../aspose.cells.griddesktop/griddesktop/endformatpainter/)() | Benachrichtigt GridDesktop, den FormatPainter zu beenden. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile)(Stream) | Exportiert in einen Excel-Dateistream, einschließlich Festplatten‑IO‑Stream oder Speicher‑Stream. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile_2)(string) | Exportiert in eine Excel-Datei. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile_1)(Stream, FileFormatType) | Exportiert in einen Excel-Dateistream, einschließlich Festplatten‑IO‑Stream oder Speicher‑Stream. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile_3)(string, FileFormatType) | Exportiert in eine Excel-Datei. |
| [ExportPdfFile](../../aspose.cells.griddesktop/griddesktop/exportpdffile/#exportpdffile)(Stream, GridPdfSaveOptions) | Exportiert in einen PDF-Dateistream, einschließlich Festplatten‑IO‑Stream oder Speicher‑Stream. |
| [ExportPdfFile](../../aspose.cells.griddesktop/griddesktop/exportpdffile/#exportpdffile_1)(string, GridPdfSaveOptions) | Exportiert in einen PDF-Dateistream, einschließlich Festplatten‑IO‑Stream oder Speicher‑Stream. |
| [GetActiveWorksheet](../../aspose.cells.griddesktop/griddesktop/getactiveworksheet/)() | Liest das aktuell aktive Arbeitsblatt. |
| [getHScrollBar](../../aspose.cells.griddesktop/griddesktop/gethscrollbar/)() | Gibt die horizontale Bildlaufleiste zurück |
| [getVScrollBar](../../aspose.cells.griddesktop/griddesktop/getvscrollbar/)() | Gibt die vertikale Bildlaufleiste zurück |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile)(Stream) | Importiert aus einem Excel-Dateistream, einschließlich Dateistream von Festplatte oder Speicherstream. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_3)(string) | Importiert aus einer Excel-Datei. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_1)(Stream, bool) | Importiert aus einem Excel-Dateistream, einschließlich Dateistream von Festplatte oder Speicherstream. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_4)(string, bool) | Importiert aus einer Excel-Datei. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_5)(string, int) | Importiert ein Arbeitsblatt aus einer Excel-Datei. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_2)(Stream, string, string, bool, bool) | Importiert aus einer Excel-Datei. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_6)(string, string, string, bool, bool) | Importiert aus einer Excel-Datei. |
| [Invalidate](../../aspose.cells.griddesktop/griddesktop/invalidate/#invalidate)() | Ungültigkeit überschreiben. |
| [OpenFindReplaceDialog](../../aspose.cells.griddesktop/griddesktop/openfindreplacedialog/)(bool) | Öffnet den FindReplace-Dialog, um Zellen zu finden oder zu ersetzen. |
| [Paste](../../aspose.cells.griddesktop/griddesktop/paste/)() | Fügt den Inhalt der Zwischenablage in die fokussierte Zelle ein. |
| [RefreshControl](../../aspose.cells.griddesktop/griddesktop/refreshcontrol/)() | Aktualisiert die GridDesktop-Steuerung. |
| [RunAllFormulas](../../aspose.cells.griddesktop/griddesktop/runallformulas/)() | Führt die Formeln aller Zellen aus. |
| [SetAllScrollBarsVisible](../../aspose.cells.griddesktop/griddesktop/setallscrollbarsvisible/)() | Setzt alle Bildlaufleisten sichtbar. |
| [SetCustomResourceManager](../../aspose.cells.griddesktop/griddesktop/setcustomresourcemanager/)(ResourceManager) | Benutzerdefinierten Ressourcen-Manager festlegen, um benutzerdefinierte Lokalisierung zu implementieren |
| [ShowStyleDialog](../../aspose.cells.griddesktop/griddesktop/showstyledialog/)() | Öffnet einen Stil-Dialog, um den Zellenstil, die Schrift, Farben usw. festzulegen. |
| [StartFormatPainter](../../aspose.cells.griddesktop/griddesktop/startformatpainter/)(bool) | Benachrichtigt GridDesktop, um den FormatPainter zu starten. |
| [UnDoSplit](../../aspose.cells.griddesktop/griddesktop/undosplit/)() | Geteiltansicht zurücksetzen. |
| static [GetVersion](../../aspose.cells.griddesktop/griddesktop/getversion/)() | Ermittelt die Release-Version. |

## Felder

| Name | Beschreibung |
| --- | --- |
| [LoadDataFilter](../../aspose.cells.griddesktop/griddesktop/loaddatafilter/) | Die Optionen zum Filtern von Daten beim Laden einer Arbeitsmappe aus einer Vorlage. |
| [ShowImportMessage](../../aspose.cells.griddesktop/griddesktop/showimportmessage/) | Ob ein Meldungsfeld angezeigt werden soll, wenn das Importieren der Datei fehlschlägt, der Standardwert ist true. |

## Ereignisse

| Name | Beschreibung |
| --- | --- |
| event [AfterDeleteColumns](../../aspose.cells.griddesktop/griddesktop/afterdeletecolumns/) | Tritt auf, nachdem eine Spalte gelöscht wurde. |
| event [AfterDeleteRows](../../aspose.cells.griddesktop/griddesktop/afterdeleterows/) | Tritt auf, nachdem eine Zeile gelöscht wurde. |
| event [AfterInsertColumns](../../aspose.cells.griddesktop/griddesktop/afterinsertcolumns/) | Tritt auf, nachdem eine neue Spalte eingefügt wurde. |
| event [AfterInsertRows](../../aspose.cells.griddesktop/griddesktop/afterinsertrows/) | Tritt auf, nachdem eine neue Zeile eingefügt wurde. |
| event [BeforeCalculate](../../aspose.cells.griddesktop/griddesktop/beforecalculate/) | Tritt auf, bevor die Formel in der Arbeitsmappe berechnet wird. |
| event [BeforeLoadFile](../../aspose.cells.griddesktop/griddesktop/beforeloadfile/) | Tritt auf, bevor die Arbeitsmappe aus einer Datei geladen wird. |
| event [CellButtonClick](../../aspose.cells.griddesktop/griddesktop/cellbuttonclick/) | Tritt auf, wenn die Zellschaltfläche geklickt wird. |
| event [CellCheckedChanged](../../aspose.cells.griddesktop/griddesktop/cellcheckedchanged/) | Tritt auf, wenn die Eigenschaft Checked der Zellen-Checkbox geändert wird. |
| event [CellClick](../../aspose.cells.griddesktop/griddesktop/cellclick/) | Tritt auf, wenn die Gridzelle angeklickt wird. |
| event [CellComboBoxCopy](../../aspose.cells.griddesktop/griddesktop/cellcomboboxcopy/) | Tritt auf, wenn ein Gridzellen-ComboBox kopiert wird. |
| event [CellDataChanged](../../aspose.cells.griddesktop/griddesktop/celldatachanged/) | Tritt auf, wenn die Dateneigenschaft der Gridzelle geändert wird. |
| event [CellDoubleClick](../../aspose.cells.griddesktop/griddesktop/celldoubleclick/) | Tritt auf, wenn die Gridzelle doppelt angeklickt wird. |
| event [CellFormatChanged](../../aspose.cells.griddesktop/griddesktop/cellformatchanged/) | Tritt auf, wenn das Zellenformat über das Dialogfeld 'Zellen formatieren' geändert wird. |
| event [CellKeyPressed](../../aspose.cells.griddesktop/griddesktop/cellkeypressed/) | Tritt auf, wenn eine Taste gedrückt wird, während eine Zelle den Fokus hat. |
| event [CellSelectedIndexChanged](../../aspose.cells.griddesktop/griddesktop/cellselectedindexchanged/) | Tritt auf, wenn die SelectedIndex-Eigenschaft der Zellen-ComboBox geändert wurde. |
| event [CellTextBoxChanging](../../aspose.cells.griddesktop/griddesktop/celltextboxchanging/) | Tritt auf, wenn Zeichen in einer Rasterzelle eingegeben werden. |
| event [CellValidationFailed](../../aspose.cells.griddesktop/griddesktop/cellvalidationfailed/) | Tritt auf, wenn die Validierung einer Rasterzelle fehlgeschlagen ist. |
| event [ColumnHeaderClick](../../aspose.cells.griddesktop/griddesktop/columnheaderclick/) | Tritt auf, wenn die Spaltenüberschrift angeklickt wird. |
| event [ColumnHeaderDoubleClick](../../aspose.cells.griddesktop/griddesktop/columnheaderdoubleclick/) | Tritt auf, wenn die Spaltenüberschrift doppelt angeklickt wird. |
| event [CommentDataChanged](../../aspose.cells.griddesktop/griddesktop/commentdatachanged/) | Tritt auf, wenn die Kommentardaten geändert wurden. |
| event [FailLoadFile](../../aspose.cells.griddesktop/griddesktop/failloadfile/) |  |
| event [FinishCalculate](../../aspose.cells.griddesktop/griddesktop/finishcalculate/) | Tritt nach der Berechnung einer Formel in der Arbeitsmappe auf. |
| event [FinishLoadFile](../../aspose.cells.griddesktop/griddesktop/finishloadfile/) | Tritt auf, wenn die Arbeitsmappe geladen wird. |
| event [FocusedCellChanged](../../aspose.cells.griddesktop/griddesktop/focusedcellchanged/) | Tritt auf, wenn die fokussierte Zelle geändert wird. |
| event [PictureClick](../../aspose.cells.griddesktop/griddesktop/pictureclick/) | Tritt auf, wenn die Form angeklickt wird. |
| event [RowColumnHiddenChanged](../../aspose.cells.griddesktop/griddesktop/rowcolumnhiddenchanged/) | Tritt auf, wenn der Ausblendungsstatus von Zeile/Spalte geändert wurde. |
| event [RowFilteredEvent](../../aspose.cells.griddesktop/griddesktop/rowfilteredevent/) | Tritt auf, nachdem ein Zeilenfilterelement ausgewählt wurde. |
| event [RowHeaderClick](../../aspose.cells.griddesktop/griddesktop/rowheaderclick/) | Tritt auf, wenn die Zeilenüberschrift angeklickt wird. |
| event [RowHeaderDoubleClick](../../aspose.cells.griddesktop/griddesktop/rowheaderdoubleclick/) | Tritt auf, wenn die Zeilenüberschrift doppelt angeklickt wird. |
| event [SelectedCellRangeChanged](../../aspose.cells.griddesktop/griddesktop/selectedcellrangechanged/) | Tritt auf, wenn der ausgewählte Zellbereich geändert wird. |
| event [SelectedSheetIndexChanged](../../aspose.cells.griddesktop/griddesktop/selectedsheetindexchanged/) | Tritt auf, wenn die SelectedSheetIndex-Eigenschaft geändert wird. |
| event [ShapeClick](../../aspose.cells.griddesktop/griddesktop/shapeclick/) | Tritt auf, wenn die Form angeklickt wird. |

### Hinweise

Bitte beziehen Sie sich auf die .NET SDK-Dokumentation für weitere Informationen zu System.Windows.Forms.UserControl.

### Beispiele

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

### Siehe auch

* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


