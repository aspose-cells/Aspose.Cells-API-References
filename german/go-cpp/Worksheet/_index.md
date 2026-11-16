---
title: "Worksheet Klasse"
linktitle: "Worksheet"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "Worksheet Klasse. Kapselt das Objekt, das worksheet in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/worksheet/
---

## Worksheet class

Kapselt das Objekt, das ein einzelnes Arbeitsblatt darstellt.

```go

type Worksheet struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [Dispose](./dispose/) | Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
| [GetProtection](./getprotection/) | Stellt die verschiedenen Arten von Schutzoptionen dar, die für ein Arbeitsblatt verfügbar sind. Unterstützt erweiterte Schutzoptionen in ExcelXP und höheren Versionen. |
| [GetUniqueId](./getuniqueid/) | Liest und setzt die eindeutige ID, sie ist identisch mit {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [SetUniqueId](./setuniqueid/) | Liest und setzt die eindeutige ID, sie ist identisch mit {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [GetPanes](./getpanes/) | Liest die Fensterbereiche. |
| [GetWorkbook](./getworkbook/) | Liest das Arbeitsmappen-Objekt, das dieses Blatt enthält. |
| [GetCells](./getcells/) | Liest die Aspose.Cells.Cells Sammlung. |
| [GetQueryTables](./getquerytables/) | Liest die QueryTableCollection im Arbeitsblatt. |
| [GetType](./gettype/) | Stellt den Arbeitsblatttyp dar. |
| [SetType](./settype/) | Stellt den Arbeitsblatttyp dar. |
| [GetName](./getname/) | Liest oder setzt den Namen des Arbeitsblatts. |
| [SetName](./setname/) | Liest oder setzt den Namen des Arbeitsblatts. |
| [GetShowFormulas](./getshowformulas/) | Gibt an, ob Formeln oder deren Ergebnisse angezeigt werden. |
| [SetShowFormulas](./setshowformulas/) | Gibt an, ob Formeln oder deren Ergebnisse angezeigt werden. |
| [GetShowDataTypeIcons](./getshowdatatypeicons/) | Gibt an, ob Datentyp‑Symbole angezeigt werden. |
| [SetShowDataTypeIcons](./setshowdatatypeicons/) | Gibt an, ob Datentyp‑Symbole angezeigt werden. |
| [IsGridlinesVisible](./isgridlinesvisible/) | Liest oder legt einen Wert fest, der angibt, ob die Gitternetzlinien sichtbar sind. Standard ist true. |
| [SetIsGridlinesVisible](./setisgridlinesvisible/) | Liest oder legt einen Wert fest, der angibt, ob die Gitternetzlinien sichtbar sind. Standard ist true. |
| [IsRowColumnHeadersVisible](./isrowcolumnheadersvisible/) | Liest oder legt einen Wert fest, der angibt, ob das Arbeitsblatt Zeilen‑ und Spaltenüberschriften anzeigt. Standard ist true. |
| [SetIsRowColumnHeadersVisible](./setisrowcolumnheadersvisible/) | Liest oder legt einen Wert fest, der angibt, ob das Arbeitsblatt Zeilen‑ und Spaltenüberschriften anzeigt. Standard ist true. |
| [GetPaneState](./getpanestate/) | Gibt an, ob das Fenster horizontale oder vertikale Teilungen hat und ob diese Teilungen eingefroren sind. |
| [GetDisplayZeros](./getdisplayzeros/) | True, wenn Nullwerte angezeigt werden. |
| [SetDisplayZeros](./setdisplayzeros/) | True, wenn Nullwerte angezeigt werden. |
| [GetDisplayRightToLeft](./getdisplayrighttoleft/) | Gibt an, ob das angegebene Arbeitsblatt von rechts nach links statt von links nach rechts angezeigt wird. Standard ist false. |
| [SetDisplayRightToLeft](./setdisplayrighttoleft/) | Gibt an, ob das angegebene Arbeitsblatt von rechts nach links statt von links nach rechts angezeigt wird. Standard ist false. |
| [IsOutlineShown](./isoutlineshown/) | Gibt an, ob die Gliederung angezeigt wird. |
| [SetIsOutlineShown](./setisoutlineshown/) | Gibt an, ob die Gliederung angezeigt wird. |
| [IsSelected](./isselected/) | Gibt an, ob dieses Arbeitsblatt beim Öffnen der Arbeitsmappe ausgewählt ist. |
| [SetIsSelected](./setisselected/) | Gibt an, ob dieses Arbeitsblatt beim Öffnen der Arbeitsmappe ausgewählt ist. |
| [FreezePanes_Int_Int_Int_Int](./freezepanes_int_int_int_int/) | Friert Fenster am angegebenen Zellbereich im Arbeitsblatt ein. |
| [GetFreezedPanes](./getfreezedpanes/) | Liest die eingefrorenen Fenster. |
| [Split](./split/) | Teilt das Fenster. |
| [FreezePanes_String_Int_Int](./freezepanes_string_int_int/) | Friert Fenster am angegebenen Zellbereich im Arbeitsblatt ein. |
| [UnFreezePanes](./unfreezepanes/) | Löst das Einfrieren der Fenster im Arbeitsblatt. |
| [RemoveSplit](./removesplit/) | Entfernt das geteilte Fenster. |
| [GetPivotTables](./getpivottables/) | Liest alle Pivot‑Tabellen in diesem Arbeitsblatt. |
| [GetListObjects](./getlistobjects/) | Liest alle ListObjects in diesem Arbeitsblatt. |
| [GetTabId](./gettabid/) | Gibt den internen Bezeichner für das Blatt an. |
| [SetTabId](./settabid/) | Gibt den internen Bezeichner für das Blatt an. |
| [GetHorizontalPageBreaks](./gethorizontalpagebreaks/) | Liest die HorizontalPageBreakCollection‑Sammlung. |
| [GetVerticalPageBreaks](./getverticalpagebreaks/) | Liest die VerticalPageBreakCollection‑Sammlung. |
| [AddPageBreaks](./addpagebreaks/) | Fügt einen Seitenumbruch hinzu. |
| [GetHyperlinks](./gethyperlinks/) | Liest die HyperlinkCollection‑Sammlung. |
| [Copy_Worksheet](./copy_worksheet/) | Kopiert Inhalte und Formate von einem anderen Arbeitsblatt. |
| [Copy_Worksheet_CopyOptions](./copy_worksheet_copyoptions/) | Kopiert Inhalte und Formate von einem anderen Arbeitsblatt. |
| [AutoFitColumn_Int_Int_Int](./autofitcolumn_int_int_int/) | Passt die Spaltenbreite automatisch an. |
| [AutoFitColumns](./autofitcolumns/) | Passt alle Spalten in diesem Arbeitsblatt automatisch an. |
| [AutoFitColumns_AutoFitterOptions](./autofitcolumns_autofitteroptions/) | Passt alle Spalten in diesem Arbeitsblatt automatisch an. |
| [AutoFitColumn_Int](./autofitcolumn_int/) | Passt die Spaltenbreite automatisch an. |
| [AutoFitColumns_Int_Int](./autofitcolumns_int_int/) | Passt die Spaltenbreite automatisch an. |
| [AutoFitColumns_Int_Int_AutoFitterOptions](./autofitcolumns_int_int_autofitteroptions/) | Passt die Spaltenbreite automatisch an. |
| [AutoFitColumns_Int_Int_Int_Int](./autofitcolumns_int_int_int_int/) | Passt die Spaltenbreite automatisch an. |
| [AutoFitColumns_Int_Int_Int_Int_AutoFitterOptions](./autofitcolumns_int_int_int_int_autofitteroptions/) | Passt die Spaltenbreite automatisch an. |
| [AutoFitRow_Int_Int_Int](./autofitrow_int_int_int/) | Passt die Zeilenhöhe automatisch an. |
| [AutoFitRow_Int_Int_Int_AutoFitterOptions](./autofitrow_int_int_int_autofitteroptions/) | Passt die Zeilenhöhe automatisch an. |
| [AutoFitRows](./autofitrows/) | Passt alle Zeilen in diesem Arbeitsblatt automatisch an. |
| [AutoFitRows_Bool](./autofitrows_bool/) | Passt alle Zeilen in diesem Arbeitsblatt automatisch an. |
| [AutoFitRows_AutoFitterOptions](./autofitrows_autofitteroptions/) | Passt alle Zeilen in diesem Arbeitsblatt automatisch an. |
| [AutoFitRows_Int_Int](./autofitrows_int_int/) | Passt die Zeilenhöhe in einem Bereich automatisch an. |
| [AutoFitRows_Int_Int_AutoFitterOptions](./autofitrows_int_int_autofitteroptions/) | Passt die Zeilenhöhe in einem Bereich automatisch an. |
| [AutoFitRow_Int_Int_Int_Int](./autofitrow_int_int_int_int/) | Passt die Zeilenhöhe in einem rechteckigen Bereich automatisch an. |
| [AutoFitRow_Int](./autofitrow_int/) | Passt die Zeilenhöhe automatisch an. |
| [GetPageSetup](./getpagesetup/) | Stellt die Seitenlayoutbeschreibung in diesem Blatt dar. |
| [GetAutoFilter](./getautofilter/) | Stellt den Auto-Filter für das angegebene Arbeitsblatt dar. |
| [Filter](./filter/) | Filtert den Bereich. |
| [GetAdvancedFilter](./getadvancedfilter/) | Liest die Einstellungen des erweiterten Filters. |
| [Advanced_Filter](./advanced_filter/) | Filtert Daten anhand komplexer Kriterien. |
| [RemoveAutoFilter](./removeautofilter/) | Entfernt den Auto-Filter des Arbeitsblatts. |
| [GetHasAutofilter](./gethasautofilter/) | Gibt an, ob dieses Arbeitsblatt einen Auto-Filter hat. |
| [GetTransitionEvaluation](./gettransitionevaluation/) | Gibt an, ob die Option zur Übergangsformel‑Auswertung (Lotus‑Kompatibilität) aktiviert ist. |
| [SetTransitionEvaluation](./settransitionevaluation/) | Gibt an, ob die Option zur Übergangsformel‑Auswertung (Lotus‑Kompatibilität) aktiviert ist. |
| [GetTransitionEntry](./gettransitionentry/) | Gibt an, ob die Option zum Übergangsformel‑Eintrag (Lotus‑Kompatibilität) aktiviert ist. |
| [SetTransitionEntry](./settransitionentry/) | Gibt an, ob die Option zum Übergangsformel‑Eintrag (Lotus‑Kompatibilität) aktiviert ist. |
| [GetVisibilityType](./getvisibilitytype/) | Gibt den Sichtbarkeitsstatus für dieses Blatt an. |
| [SetVisibilityType](./setvisibilitytype/) | Gibt den Sichtbarkeitsstatus für dieses Blatt an. |
| [SetVisible](./setvisible/) | Setzt die Sichtbarkeitsoptionen. |
| [IsVisible](./isvisible/) | Stellt dar, ob das Arbeitsblatt sichtbar ist. |
| [SetIsVisible](./setisvisible/) | Stellt dar, ob das Arbeitsblatt sichtbar ist. |
| [SelectRange](./selectrange/) | Wählt einen Bereich aus. |
| [RemoveAllDrawingObjects](./removealldrawingobjects/) | Entfernt alle Zeichenobjekte in diesem Arbeitsblatt. |
| [ClearComments](./clearcomments/) | Löscht alle Kommentare im Designer‑Tabellenblatt. |
| [GetSparklineGroups](./getsparklinegroups/) | Liest die Sparkline‑Gruppen im Arbeitsblatt. |
| [GetCharts](./getcharts/) | Liest eine Diagrammsammlung |
| [GetComments](./getcomments/) | Liest die Kommentar‑Sammlung. |
| [GetPictures](./getpictures/) | Liest eine Bildersammlung. |
| [GetAllPictures](./getallpictures/) | Liest alle Bilder, einschließlich in Zellen eingebetteter und über Zellen liegender Bilder. |
| [GetTextBoxes](./gettextboxes/) | Liest eine Textfeldsammlung. |
| [GetCheckBoxes](./getcheckboxes/) | Ruft eine CheckBox‑Sammlung ab. |
| [GetOleObjects](./getoleobjects/) | Stellt eine Sammlung von OleObject in einem Arbeitsblatt dar. |
| [GetShapes](./getshapes/) | Gibt alle Zeichenformen in diesem Arbeitsblatt zurück. |
| [GetSlicers](./getslicers/) | Rufe die Slicer‑Sammlung im Arbeitsblatt ab |
| [GetTimelines](./gettimelines/) | Rufe die Timeline‑Sammlung im Arbeitsblatt ab |
| [Protect_ProtectionType](./protect_protectiontype/) | Schützt das Arbeitsblatt. |
| [Protect_ProtectionType_String_String](./protect_protectiontype_string_string/) | Schützt das Arbeitsblatt. |
| [Unprotect](./unprotect/) | Hebt den Schutz des Arbeitsblatts auf. |
| [Unprotect_String](./unprotect_string/) | Hebt den Schutz des Arbeitsblatts auf. |
| [GetIndex](./getindex/) | Ruft den Index des Blatts in der Arbeitsblatt‑Sammlung ab. |
| [MoveTo](./moveto/) | Verschiebt das Blatt an eine andere Position in der Tabellenkalkulation. |
| [IsProtected](./isprotected/) | Gibt an, ob das Arbeitsblatt geschützt ist. |
| [GetValidations](./getvalidations/) | Ruft die Sammlung der Datenvalidierungseinstellungen im Arbeitsblatt ab. |
| [GetAllowEditRanges](./getalloweditranges/) | Ruft die Sammlung der zulässigen Bearbeitungsbereiche im Arbeitsblatt ab. |
| [GetErrorCheckOptions](./geterrorcheckoptions/) | Ruft die Fehlerprüfungs‑Einstellung ab, die auf bestimmte Bereiche angewendet wird. |
| [GetOutline](./getoutline/) | Ruft die Gliederung in diesem Arbeitsblatt ab. |
| [GetFirstVisibleRow](./getfirstvisiblerow/) | Stellt den Index der ersten sichtbaren Zeile dar. |
| [SetFirstVisibleRow](./setfirstvisiblerow/) | Stellt den Index der ersten sichtbaren Zeile dar. |
| [GetFirstVisibleColumn](./getfirstvisiblecolumn/) | Stellt den Index der ersten sichtbaren Spalte dar. |
| [SetFirstVisibleColumn](./setfirstvisiblecolumn/) | Stellt den Index der ersten sichtbaren Spalte dar. |
| [Replace](./replace/) | Ersetzt den Text aller Zellen durch eine neue Zeichenkette. |
| [GetZoom](./getzoom/) | Stellt den Skalierungsfaktor in Prozent dar. Er sollte zwischen 10 und 400 liegen. |
| [SetZoom](./setzoom/) | Stellt den Skalierungsfaktor in Prozent dar. Er sollte zwischen 10 und 400 liegen. |
| [GetViewType](./getviewtype/) | Ruft den Ansichtstyp ab und legt ihn fest. |
| [SetViewType](./setviewtype/) | Ruft den Ansichtstyp ab und legt ihn fest. |
| [IsPageBreakPreview](./ispagebreakpreview/) | Gibt an, ob das angegebene Arbeitsblatt in der Normalansicht oder in der Seitenumbruchvorschau angezeigt wird. |
| [SetIsPageBreakPreview](./setispagebreakpreview/) | Gibt an, ob das angegebene Arbeitsblatt in der Normalansicht oder in der Seitenumbruchvorschau angezeigt wird. |
| [IsRulerVisible](./isrulervisible/) | Gibt an, ob das Lineal sichtbar ist. Diese Eigenschaft wird nur in der Seitenumbruchvorschau angewendet. |
| [SetIsRulerVisible](./setisrulervisible/) | Gibt an, ob das Lineal sichtbar ist. Diese Eigenschaft wird nur in der Seitenumbruchvorschau angewendet. |
| [GetSelectedAreas](./getselectedareas/) | Ruft die ausgewählten Zellbereiche im Designer‑Tabellenblatt ab. |
| [GetTabColor](./gettabcolor/) | Stellt die Registerkartenfarbe des Arbeitsblatts dar. |
| [SetTabColor](./settabcolor/) | Stellt die Registerkartenfarbe des Arbeitsblatts dar. |
| [GetGridlineColor](./getgridlinecolor/) | Ruft die Farbe der Gitternetzlinie ab und legt sie fest |
| [SetGridlineColor](./setgridlinecolor/) | Ruft die Farbe der Gitternetzlinie ab und legt sie fest |
| [GetCodeName](./getcodename/) | Ruft den Code‑Namen des Arbeitsblatts ab. |
| [SetCodeName](./setcodename/) | Ruft den Code‑Namen des Arbeitsblatts ab. |
| [GetBackgroundImage](./getbackgroundimage/) | Liest und setzt das Hintergrundbild des Arbeitsblatts. |
| [SetBackgroundImage](./setbackgroundimage/) | Liest und setzt das Hintergrundbild des Arbeitsblatts. |
| [GetConditionalFormattings](./getconditionalformattings/) | Liest die ConditionalFormattings im Arbeitsblatt. |
| [GetActiveCell](./getactivecell/) | Liest oder setzt die aktive Zelle im Arbeitsblatt. |
| [SetActiveCell](./setactivecell/) | Liest oder setzt die aktive Zelle im Arbeitsblatt. |
| [GetCustomProperties](./getcustomproperties/) | Liest ein Objekt, das die Identifikationsinformationen darstellt, die mit einem Arbeitsblatt verknüpft sind. |
| [GetPrintingPageBreaks](./getprintingpagebreaks/) | Liest automatische Seitenumbrüche. |
| [GetSmartTagSetting](./getsmarttagsetting/) | Liest alle SmartTagCollection-Objekte des Arbeitsblatts. |
| [ToString](./tostring/) | Gibt eine Zeichenkette zurück, die das aktuelle Worksheet-Objekt darstellt. |
| [GetScenarios](./getscenarios/) | Liest die Sammlung von Scenario. |
| [StartAccessCache](./startaccesscache/) | Startet die Sitzung, die Cache verwendet, um auf die Daten in diesem Arbeitsblatt zuzugreifen. |
| [CloseAccessCache](./closeaccesscache/) | Schließt die Sitzung, die Cache verwendet, um auf die Daten in diesem Arbeitsblatt zuzugreifen. |
| [ConvertFormulaReferenceStyle](./convertformulareferencestyle/) | Konvertiert den Referenzstil der Formel. |
| [CalculateFormula_String](./calculateformula_string/) | Berechnet eine Formel. |
| [CalculateFormula_String_CalculationOptions](./calculateformula_string_calculationoptions/) | Berechnet einen Formelausdruck direkt. |
| [CalculateFormula_String_FormulaParseOptions_CalculationOptions_Int_Int_CalculationData](./calculateformula_string_formulaparseoptions_calculationoptions_int_int_calculationdata/) | Berechnet einen Formelausdruck direkt. |
| [CalculateArrayFormula_String_CalculationOptions](./calculatearrayformula_string_calculationoptions/) | Berechnet eine Formel als Array-Formel. |
| [CalculateArrayFormula_String_CalculationOptions_Int_Int](./calculatearrayformula_string_calculationoptions_int_int/) | Berechnet eine Formel als Array-Formel. |
| [CalculateArrayFormula_String_FormulaParseOptions_CalculationOptions_Int_Int_Int_Int_CalculationData](./calculatearrayformula_string_formulaparseoptions_calculationoptions_int_int_int_int_calculationdata/) | Berechnet eine Formel als Array-Formel. |
| [CalculateFormula_CalculationOptions_Bool](./calculateformula_calculationoptions_bool/) | Berechnet alle Formeln in diesem Arbeitsblatt. |
| [GetAreasOfXmlMapQuery](./getareasofxmlmapquery/) | Abfrage von Zellbereichen, die dem spezifischen Pfad einer xml map zugeordnet/verknüpft sind. |
| [GetCellWatches](./getcellwatches/) | Liest die Sammlung von Zellen in diesem Arbeitsblatt, die im 'watch window' überwacht werden. |
| [RefreshPivotTables](./refreshpivottables/) | Aktualisiert alle PivotTables in diesem Arbeitsblatt. |
| [RefreshPivotTables_PivotTableRefreshOption](./refreshpivottables_pivottablerefreshoption/) | Aktualisiert alle PivotTables in diesem Arbeitsblatt. |
