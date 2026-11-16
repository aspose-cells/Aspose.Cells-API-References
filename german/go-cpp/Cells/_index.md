---
title: "Cells Klasse"
linktitle: "Cells"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "Cells Klasse. Kapselt das Objekt, das Zellen in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/cells/
---

## Cells class

Kapselt eine Sammlung von zellrelevanten Objekten, wie <see cref=\"Cell\"/>, <see cref=\"Row\"/>, usw.

```go

type Cells struct  {
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
| [GetOdsCellFields](./getodscellfields/) | Liefert die Liste der Felder von ods. |
| [Dispose](./dispose/) | Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
| [GetCount](./getcount/) | Liefert die Gesamtanzahl der instanziierten Cell-Objekte. |
| [GetCountLarge](./getcountlarge/) | Liefert die Gesamtanzahl der instanziierten Cell-Objekte. |
| [GetEnumerator](./getenumerator/) | Liefert den Zellen-Enumerator. |
| [GetRows](./getrows/) | Liefert die Sammlung von Row-Objekten, die die einzelnen Zeilen in diesem Arbeitsblatt darstellen. |
| [GetMergedAreas](./getmergedareas/) | Liefert alle zusammengeführten Zellen. |
| [CheckCell](./checkcell/) | Liefert das Cell-Element oder null am angegebenen Zeilen- und Spaltenindex der Zelle. |
| [CheckRow](./checkrow/) | Liefert das Row-Element oder null am angegebenen Zeilenindex der Zelle. |
| [CheckColumn](./checkcolumn/) | Liefert das Column-Element oder null am angegebenen Spaltenindex. |
| [IsRowHidden](./isrowhidden/) | Prüft, ob eine Zeile am angegebenen Index ausgeblendet ist. |
| [IsColumnHidden](./iscolumnhidden/) | Prüft, ob eine Spalte am angegebenen Index ausgeblendet ist. |
| [AddRange](./addrange/) | Fügt eine Referenz auf ein Bereichsobjekt zu Zellen hinzu |
| [CreateRange_String_String](./createrange_string_string/) | Erstellt ein Range-Objekt aus einem Zellbereich. |
| [CreateRange_Int_Int_Int_Int](./createrange_int_int_int_int/) | Erstellt ein Range-Objekt aus einem Zellbereich. |
| [CreateRange_String](./createrange_string/) | Erstellt ein Range-Objekt aus einer Adresse des Bereichs. |
| [CreateRange_Int_Int_Bool](./createrange_int_int_bool/) | Erstellt ein Range-Objekt aus Zeilen von Zellen oder Spalten von Zellen. |
| [Get_Int_Int](./get_int_int/) | Liefert das Cell-Element am angegebenen Zeilenindex und Spaltenindex der Zelle. |
| [Get_String](./get_string/) | Liefert das Cell-Element am angegebenen Zellenamen. |
| [GetMultiThreadReading](./getmultithreadreading/) | Liest oder setzt, ob das Zellen-Datenmodell Multi-Thread-Lesen unterstützen soll. Standardwert dieser Eigenschaft ist false. |
| [SetMultiThreadReading](./setmultithreadreading/) | Liest oder setzt, ob das Zellen-Datenmodell Multi-Thread-Lesen unterstützen soll. Standardwert dieser Eigenschaft ist false. |
| [GetMemorySetting](./getmemorysetting/) | Liest oder setzt die Speicherverbrauchsoption für diese Zellen. |
| [SetMemorySetting](./setmemorysetting/) | Liest oder setzt die Speicherverbrauchsoption für diese Zellen. |
| [Clear](./clear/) | Löscht alle Daten des Arbeitsblatts. |
| [GetStyle](./getstyle/) | Liest und setzt den Standardstil des Arbeitsblatts. |
| [SetStyle](./setstyle/) | Liest und setzt den Standardstil des Arbeitsblatts. |
|[IsDefaultColumnHidden](./isdefaultcolumnhidden/) |  | 
|[SetIsDefaultColumnHidden](./setisdefaultcolumnhidden/) |  | 
| [GetStandardWidthInch](./getstandardwidthinch/) | Liest oder setzt die Standardspaltenbreite im Arbeitsblatt, in Zoll. |
| [SetStandardWidthInch](./setstandardwidthinch/) | Liest oder setzt die Standardspaltenbreite im Arbeitsblatt, in Zoll. |
| [GetStandardWidthPixels](./getstandardwidthpixels/) | Liest oder setzt die Standardspaltenbreite im Arbeitsblatt, in Pixel. |
| [SetStandardWidthPixels](./setstandardwidthpixels/) | Liest oder setzt die Standardspaltenbreite im Arbeitsblatt, in Pixel. |
| [GetStandardWidth](./getstandardwidth/) | Liest oder setzt die Standardspaltenbreite im Arbeitsblatt, in Zeichen. |
| [SetStandardWidth](./setstandardwidth/) | Liest oder setzt die Standardspaltenbreite im Arbeitsblatt, in Zeichen. |
| [GetStandardHeight](./getstandardheight/) | Liest oder setzt die Standardzeilenhöhe in diesem Arbeitsblatt, in Punkten. |
| [SetStandardHeight](./setstandardheight/) | Liest oder setzt die Standardzeilenhöhe in diesem Arbeitsblatt, in Punkten. |
| [GetStandardHeightPixels](./getstandardheightpixels/) | Liest oder setzt die Standardzeilenhöhe in diesem Arbeitsblatt, in Pixel. |
| [SetStandardHeightPixels](./setstandardheightpixels/) | Liest oder setzt die Standardzeilenhöhe in diesem Arbeitsblatt, in Pixel. |
| [GetStandardHeightInch](./getstandardheightinch/) | Liest oder setzt die Standardzeilenhöhe in diesem Arbeitsblatt, in Zoll. |
| [SetStandardHeightInch](./setstandardheightinch/) | Liest oder setzt die Standardzeilenhöhe in diesem Arbeitsblatt, in Zoll. |
| [ImportFormulaArray](./importformulaarray/) | Importiert ein Array von Formeln in ein Arbeitsblatt. |
| [TextToColumns](./texttocolumns/) | Teilt den Inhalt in der angegebenen Spalte in mehrere Spalten.. |
| [ImportCSV_String_String_Bool_Int_Int](./importcsv_string_string_bool_int_int/) | Importiert eine CSV-Datei in die Zellen. |
| [ImportCSV_Stream_String_Bool_Int_Int](./importcsv_stream_string_bool_int_int/) | Importiert eine CSV-Datei in die Zellen. |
| [ImportCSV_String_TxtLoadOptions_Int_Int](./importcsv_string_txtloadoptions_int_int/) | Importiert eine CSV-Datei in die Zellen. |
| [ImportCSV_Stream_TxtLoadOptions_Int_Int](./importcsv_stream_txtloadoptions_int_int/) | Importiert eine CSV-Datei in die Zellen. |
| [GetPreserveString](./getpreservestring/) | Liest oder setzt einen Wert, der angibt, ob alle Arbeitsblattwerte als Zeichenketten erhalten bleiben. Standard ist false. |
| [SetPreserveString](./setpreservestring/) | Liest oder setzt einen Wert, der angibt, ob alle Arbeitsblattwerte als Zeichenketten erhalten bleiben. Standard ist false. |
| [Merge_Int_Int_Int_Int](./merge_int_int_int_int/) | Fügt einen angegebenen Zellbereich zu einer einzelnen Zelle zusammen. |
| [Merge_Int_Int_Int_Int_Bool](./merge_int_int_int_int_bool/) | Fügt einen angegebenen Zellbereich zu einer einzelnen Zelle zusammen. |
| [Merge_Int_Int_Int_Int_Bool_Bool](./merge_int_int_int_int_bool_bool/) | Fügt einen angegebenen Zellbereich zu einer einzelnen Zelle zusammen. |
| [UnMerge](./unmerge/) | Teilt einen angegebenen Bereich zusammengeführter Zellen. |
| [ClearMergedCells](./clearmergedcells/) | Löscht alle zusammengeführten Bereiche. |
| [HideRow](./hiderow/) | Blendet eine Zeile aus. |
| [UnhideRow](./unhiderow/) | Blendet eine Zeile wieder ein. |
| [HideRows](./hiderows/) | Versteckt mehrere Zeilen. |
| [UnhideRows](./unhiderows/) | Blendet die versteckten Zeilen wieder ein. |
| [SetRowHeightPixel](./setrowheightpixel/) | Setzt die Zeilenhöhe in Pixeln. |
| [SetRowHeightInch](./setrowheightinch/) | Setzt die Zeilenhöhe in Zoll. |
| [SetRowHeight](./setrowheight/) | Setzt die Höhe der angegebenen Zeile. |
| [GetRowHeight_Int_Bool_CellsUnitType](./getrowheight_int_bool_cellsunittype/) | Ermittelt die Höhe der Zeile. |
| [GetColumnWidth_Int_Bool_CellsUnitType](./getcolumnwidth_int_bool_cellsunittype/) | Ermittelt die Spaltenbreite. |
| [HideColumn](./hidecolumn/) | Versteckt eine Spalte. |
| [UnhideColumn](./unhidecolumn/) | Blendet eine Spalte wieder ein |
| [HideColumns](./hidecolumns/) | Versteckt mehrere Spalten. |
| [UnhideColumns](./unhidecolumns/) | Blendet mehrere Spalten wieder ein. |
| [GetRowHeight_Int](./getrowheight_int/) | Ermittelt die Höhe einer angegebenen Zeile in Punkten. |
| [GetViewRowHeight](./getviewrowheight/) | Ermittelt die Höhe einer angegebenen Zeile. |
| [GetRowHeightInch](./getrowheightinch/) | Ermittelt die Höhe einer angegebenen Zeile in Zoll. |
| [GetViewRowHeightInch](./getviewrowheightinch/) | Ermittelt die Höhe einer angegebenen Zeile in Zoll. |
| [GetRowHeightPixel](./getrowheightpixel/) | Ermittelt die Höhe einer angegebenen Zeile in Pixeln. |
| [SetColumnWidthPixel](./setcolumnwidthpixel/) | Setzt die Spaltenbreite in Pixeln in der Normalansicht. |
| [SetColumnWidthInch](./setcolumnwidthinch/) | Setzt die Spaltenbreite in Zoll in der Normalansicht. |
| [SetColumnWidth](./setcolumnwidth/) | Setzt die Breite der angegebenen Spalte in der Normalansicht. |
| [GetColumnWidthPixel](./getcolumnwidthpixel/) | Ermittelt die Breite der angegebenen Spalte in der Normalansicht in Pixeln. |
| [GetColumnWidth_Int](./getcolumnwidth_int/) | Ermittelt die Breite (in Zeichen) der angegebenen Spalte in der Normalansicht |
| [GetViewColumnWidthPixel](./getviewcolumnwidthpixel/) | Ermittelt die Breite in verschiedenen Ansichtstypen. |
| [SetViewColumnWidthPixel](./setviewcolumnwidthpixel/) | Setzt die Breite der Spalte in verschiedenen Ansichten. |
| [GetMinRow](./getminrow/) | Minimaler Zeilenindex einer Zelle, die Daten oder Formatierungen enthält. |
| [GetMaxRow](./getmaxrow/) | Maximaler Zeilenindex einer Zelle, die Daten oder Formatierungen enthält. |
| [GetMinColumn](./getmincolumn/) | Minimaler Spaltenindex derjenigen Zellen, die in der Sammlung instanziiert wurden (does not include the columnwhere style is defined for the whole column but no cell has been instantiated in it). |
| [GetMaxColumn](./getmaxcolumn/) | Maximaler Spaltenindex der Zellen, die in der Sammlung instanziiert wurden (schließt die Spalte nicht ein, für die der Stil für die gesamte Spalte definiert ist, aber in der keine Zelle instanziiert wurde). |
| [GetMinDataRow](./getmindatarow/) | Minimaler Zeilenindex der Zelle, die Daten enthält. |
| [GetMaxDataRow](./getmaxdatarow/) | Maximaler Zeilenindex der Zelle, die Daten enthält. |
| [GetMinDataColumn](./getmindatacolumn/) | Minimaler Spaltenindex der Zelle, die Daten enthält. |
| [GetMaxDataColumn](./getmaxdatacolumn/) | Maximaler Spaltenindex der Zelle, die Daten enthält. |
| [GetLastDataRow](./getlastdatarow/) | Ermittelt den letzten Zeilenindex der Zelle, die Daten in der angegebenen Spalte enthält. |
| [GetFirstDataRow](./getfirstdatarow/) | Ermittelt den ersten Zeilenindex der Zelle, die Daten in der angegebenen Spalte enthält. |
| [IsDefaultRowHeightMatched](./isdefaultrowheightmatched/) | Gibt an, dass Zeilenhöhe und Standard‑Schriftgröße übereinstimmen |
| [SetIsDefaultRowHeightMatched](./setisdefaultrowheightmatched/) | Gibt an, dass Zeilenhöhe und Standard‑Schriftgröße übereinstimmen |
| [IsDefaultRowHidden](./isdefaultrowhidden/) | Gibt an, ob die Zeile standardmäßig ausgeblendet ist. |
| [SetIsDefaultRowHidden](./setisdefaultrowhidden/) | Gibt an, ob die Zeile standardmäßig ausgeblendet ist. |
| [GetColumns](./getcolumns/) | Ermittelt die Sammlung von Column-Objekten, die die einzelnen Spalten in diesem Arbeitsblatt darstellen. |
| [ApplyColumnStyle](./applycolumnstyle/) | Wendet Formate für eine gesamte Spalte an. |
| [ApplyRowStyle](./applyrowstyle/) | Wendet Formate für eine gesamte Zeile an. |
| [ApplyStyle](./applystyle/) | Wendet Formate für ein gesamtes Arbeitsblatt an. |
| [CopyColumns_Cells_Int_Int_Int_PasteOptions](./copycolumns_cells_int_int_int_pasteoptions/) | Kopiert Daten und Formate einer gesamten Spalte. |
| [CopyColumn](./copycolumn/) | Kopiert Daten und Formate einer gesamten Spalte. |
| [CopyColumns_Cells_Int_Int_Int](./copycolumns_cells_int_int_int/) | Kopiert Daten und Formate mehrerer Spalten. |
| [CopyColumns_Cells_Int_Int_Int_Int](./copycolumns_cells_int_int_int_int/) | Kopiert Daten und Formate aller Spalten. |
| [CopyRow](./copyrow/) | Kopiert Daten und Formate einer gesamten Zeile. |
| [CopyRows_Cells_Int_Int_Int](./copyrows_cells_int_int_int/) | Kopiert Daten und Formate einiger gesamter Zeilen. |
| [CopyRows_Cells_Int_Int_Int_CopyOptions](./copyrows_cells_int_int_int_copyoptions/) | Kopiert Daten und Formate einiger gesamter Zeilen. |
| [CopyRows_Cells_Int_Int_Int_CopyOptions_PasteOptions](./copyrows_cells_int_int_int_copyoptions_pasteoptions/) | Kopiert Daten und Formate einiger gesamter Zeilen. |
| [GetGroupedRowOutlineLevel](./getgroupedrowoutlinelevel/) | Ermittelt die Gliederungsebene (nullbasiert) der Zeile. |
| [GetGroupedColumnOutlineLevel](./getgroupedcolumnoutlinelevel/) | Ermittelt die Gliederungsebene (nullbasiert) der Spalte. |
| [GetMaxGroupedColumnOutlineLevel](./getmaxgroupedcolumnoutlinelevel/) | Ermittelt die maximale gruppierte Spalten‑Gliederungsebene (nullbasiert). |
| [GetMaxGroupedRowOutlineLevel](./getmaxgroupedrowoutlinelevel/) | Ermittelt die maximale gruppierte Zeilen‑Gliederungsebene (nullbasiert). |
| [ShowGroupDetail](./showgroupdetail/) | Erweitert die gruppierten Zeilen/Spalten. |
| [HideGroupDetail](./hidegroupdetail/) | Klappt die gruppierten Zeilen/Spalten zusammen. |
| [UngroupColumns](./ungroupcolumns/) | Hebt die Gruppierung von Spalten auf. |
| [GroupColumns_Int_Int](./groupcolumns_int_int/) | Gruppiert Spalten. |
| [GroupColumns_Int_Int_Bool](./groupcolumns_int_int_bool/) | Gruppiert Spalten. |
| [UngroupRows_Int_Int_Bool](./ungrouprows_int_int_bool/) | Entgruppiert Zeilen. |
| [UngroupRows_Int_Int](./ungrouprows_int_int/) | Entgruppiert Zeilen. |
| [GroupRows_Int_Int_Bool](./grouprows_int_int_bool/) | Gruppiert Zeilen. |
| [GroupRows_Int_Int](./grouprows_int_int/) | Gruppiert Zeilen. |
| [DeleteColumn_Int_Bool](./deletecolumn_int_bool/) | Löscht eine Spalte. |
| [DeleteColumn_Int](./deletecolumn_int/) | Löscht eine Spalte. |
| [DeleteColumns_Int_Int_Bool](./deletecolumns_int_int_bool/) | Löscht mehrere Spalten. |
| [DeleteColumns_Int_Int_DeleteOptions](./deletecolumns_int_int_deleteoptions/) | Löscht mehrere Spalten. |
| [IsDeletingRangeEnabled](./isdeletingrangeenabled/) | Prüfen, ob der Bereich gelöscht werden kann. |
| [DeleteRow_Int](./deleterow_int/) | Löscht eine Zeile. |
| [DeleteRow_Int_Bool](./deleterow_int_bool/) | Löscht eine Zeile. |
| [DeleteRows_Int_Int](./deleterows_int_int/) | Löscht mehrere Zeilen. |
| [DeleteRows_Int_Int_Bool](./deleterows_int_int_bool/) | Löscht mehrere Zeilen im Arbeitsblatt. |
| [DeleteRows_Int_Int_DeleteOptions](./deleterows_int_int_deleteoptions/) | Löscht mehrere Zeilen im Arbeitsblatt. |
| [DeleteBlankColumns](./deleteblankcolumns/) | Lösche alle leeren Spalten, die keine Daten enthalten. |
| [DeleteBlankColumns_DeleteOptions](./deleteblankcolumns_deleteoptions/) | Lösche alle leeren Spalten, die keine Daten enthalten. |
| [IsBlankColumn](./isblankcolumn/) | Prüft, ob die angegebene Spalte leer ist (keine Daten enthält). |
| [DeleteBlankRows](./deleteblankrows/) | Lösche alle leeren Zeilen, die keine Daten oder andere Objekte enthalten. |
| [DeleteBlankRows_DeleteOptions](./deleteblankrows_deleteoptions/) | Lösche alle leeren Zeilen, die keine Daten oder bestimmte Spezialobjekte wie sichtbare Kommentare oder Pivot-Tabellen enthalten. |
| [InsertColumns_Int_Int](./insertcolumns_int_int/) | Fügt einige Spalten in das Arbeitsblatt ein. |
| [InsertColumns_Int_Int_Bool](./insertcolumns_int_int_bool/) | Fügt einige Spalten in das Arbeitsblatt ein. |
| [InsertColumns_Int_Int_InsertOptions](./insertcolumns_int_int_insertoptions/) | Fügt einige Spalten in das Arbeitsblatt ein. |
| [InsertColumn_Int_Bool](./insertcolumn_int_bool/) | Fügt eine neue Spalte in das Arbeitsblatt ein. |
| [InsertColumn_Int](./insertcolumn_int/) | Fügt eine neue Spalte in das Arbeitsblatt ein. |
| [InsertRows_Int_Int_Bool](./insertrows_int_int_bool/) | Fügt mehrere Zeilen in das Arbeitsblatt ein. |
| [InsertRows_Int_Int_InsertOptions](./insertrows_int_int_insertoptions/) | Fügt mehrere Zeilen in das Arbeitsblatt ein. |
| [InsertRows_Int_Int](./insertrows_int_int/) | Fügt mehrere Zeilen in das Arbeitsblatt ein. |
| [InsertRow](./insertrow/) | Fügt eine neue Zeile in das Arbeitsblatt ein. |
| [GetRanges](./getranges/) | Ermittelt die Sammlung von Range-Objekten, die zur Laufzeit erstellt wurden. |
| [ClearRange_CellArea](./clearrange_cellarea/) | Löscht Inhalte und Formatierung eines Bereichs. |
| [ClearRange_Int_Int_Int_Int](./clearrange_int_int_int_int/) | Löscht Inhalte und Formatierung eines Bereichs. |
| [ClearContents_CellArea](./clearcontents_cellarea/) | Löscht Inhalte eines Bereichs. |
| [ClearContents_Int_Int_Int_Int](./clearcontents_int_int_int_int/) | Löscht Inhalte eines Bereichs. |
| [ClearFormats_CellArea](./clearformats_cellarea/) | Löscht die Formatierung eines Bereichs. |
| [ClearFormats_Int_Int_Int_Int](./clearformats_int_int_int_int/) | Löscht die Formatierung eines Bereichs. |
| [GetLastCell](./getlastcell/) | Ermittelt die letzte Zelle in diesem Arbeitsblatt. |
| [LinkToXmlMap](./linktoxmlmap/) | Link zu einer XML-Map. |
| [GetMaxDisplayRange](./getmaxdisplayrange/) | Ermittelt den maximalen Bereich, der Daten, zusammengeführte Zellen und Formen enthält. |
| [GetFirstCell](./getfirstcell/) | Ermittelt die erste Zelle in diesem Arbeitsblatt. |
| [Find_Object_Cell](./find_object_cell/) | Findet die Zelle, die das Eingabeobjekt enthält. |
| [Find_Object_Cell_FindOptions](./find_object_cell_findoptions/) | Findet die Zelle, die das Eingabeobjekt enthält. |
| [EndCellInRow_Int](./endcellinrow_int/) | Ermittelt die letzte Zelle in dieser Zeile. |
| [EndCellInColumn_Int](./endcellincolumn_int/) | Ermittelt die letzte Zelle in dieser Spalte. |
| [EndCellInColumn_Int_Int_Int_Int](./endcellincolumn_int_int_int_int/) | Ermittelt die letzte Zelle mit dem maximalen Spaltenindex in diesem Bereich. |
| [EndCellInRow_Int_Int_Int_Int](./endcellinrow_int_int_int_int/) | Ermittelt die letzte Zelle mit dem maximalen Zeilenindex in diesem Bereich. |
| [MoveRange](./moverange/) | Verschiebt den Bereich. |
| [InsertCutCells](./insertcutcells/) | Einfügen des ausgeschnittenen Bereichs. |
| [InsertRange_CellArea_Int_ShiftType_Bool](./insertrange_cellarea_int_shifttype_bool/) | Fügt einen Zellbereich ein und verschiebt Zellen gemäß der Verschiebungsoption. |
| [InsertRange_CellArea_ShiftType](./insertrange_cellarea_shifttype/) | Fügt einen Zellbereich ein und verschiebt Zellen gemäß der Verschiebungsoption. |
| [InsertRange_CellArea_Int_ShiftType](./insertrange_cellarea_int_shifttype/) | Fügt einen Zellbereich ein und verschiebt Zellen gemäß der Verschiebungsoption. |
| [DeleteRange](./deleterange/) | Löscht einen Zellbereich und verschiebt Zellen gemäß der Verschiebungsoption. |
| [ExportArray](./exportarray/) | Exportiert Daten aus der Cells‑Sammlung in ein zweidimensionales Array‑Objekt. |
| [RetrieveSubtotalSetting](./retrievesubtotalsetting/) | Ruft die Zwischensummen‑Einstellung des Bereichs ab. |
| [Subtotal_CellArea_Int_ConsolidationFunction_int32Array](./subtotal_cellarea_int_consolidationfunction_int32array/) | Erstellt Zwischensummen für den Bereich. |
| [Subtotal_CellArea_Int_ConsolidationFunction_int32Array_Bool_Bool_Bool](./subtotal_cellarea_int_consolidationfunction_int32array_bool_bool_bool/) | Erstellt Zwischensummen für den Bereich. |
| [RemoveFormulas](./removeformulas/) | Entfernt alle Formeln und ersetzt sie durch den Formelwert. |
| [RemoveDuplicates](./removeduplicates/) | Entfernt doppelte Zeilen im Blatt. |
| [RemoveDuplicates_Int_Int_Int_Int](./removeduplicates_int_int_int_int/) | Entfernt doppelte Werte im Bereich. |
| [RemoveDuplicates_Int_Int_Int_Int_Bool_int32Array](./removeduplicates_int_int_int_int_bool_int32array/) | Entfernt doppelte Daten im Bereich. |
| [ConvertStringToNumericValue](./convertstringtonumericvalue/) | Konvertiert alle Zeichenketten‑Daten im Arbeitsblatt nach Möglichkeit in numerische Werte. |
| [GetDependents](./getdependents/) | Ermittelt alle Zellen, die auf die bestimmte Zelle verweisen. |
| [GetDependentsInCalculation](./getdependentsincalculation/) | Ermittelt alle Zellen, deren berechnetes Ergebnis von einer bestimmten Zelle abhängt. |
| [GetCellsWithPlaceInCellPicture](./getcellswithplaceincellpicture/) | Ermittelt alle Zellen, die ein eingebettetes Bild enthalten. |
| [GetCellStyle](./getcellstyle/) | Ermittelt den Stil der angegebenen Zelle. |
| [GetCellDisplayStyle_Int_Int](./getcelldisplaystyle_int_int/) | Ermittelt den Anzeigestil der angegebenen Zelle. |
| [GetCellDisplayStyle_Int_Int_BorderType](./getcelldisplaystyle_int_int_bordertype/) | Ermittelt den Anzeigestil der angegebenen Zelle. |
