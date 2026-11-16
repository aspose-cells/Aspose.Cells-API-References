---
title: "EbookSaveOptions Klasse"
linktitle: "EbookSaveOptions"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "EbookSaveOptions Klasse. Kapselt das Objekt, das ebooksaveoptions in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/ebooksaveoptions/
---

## EbookSaveOptions class

Stellt die Optionen zum Speichern einer E-Book-Datei dar.

```go

type EbookSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewEbookSaveOptions](./newebooksaveoptions/) | Erstellt Optionen zum Speichern der E‑Book-Datei. |
| [NewEbookSaveOptions_SaveFormat](./newebooksaveoptions_saveformat/) | Erstellt Optionen zum Speichern der E‑Book-Datei. |
| [NewEbookSaveOptions_HtmlSaveOptions](./newebooksaveoptions_htmlsaveoptions/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetIgnoreInvisibleShapes](./getignoreinvisibleshapes/) | Geben Sie an, ob nicht sichtbare Formen exportiert werden sollen |
| [SetIgnoreInvisibleShapes](./setignoreinvisibleshapes/) | Geben Sie an, ob nicht sichtbare Formen exportiert werden sollen |
| [GetPageTitle](./getpagetitle/) | Der Titel der HTML‑Seite. Nur beim Speichern in einen HTML‑Stream. |
| [SetPageTitle](./setpagetitle/) | Der Titel der HTML‑Seite. Nur beim Speichern in einen HTML‑Stream. |
| [GetAttachedFilesDirectory](./getattachedfilesdirectory/) | Das Verzeichnis, in dem die angehängten Dateien gespeichert werden. Nur beim Speichern in einen HTML‑Stream. |
| [SetAttachedFilesDirectory](./setattachedfilesdirectory/) | Das Verzeichnis, in dem die angehängten Dateien gespeichert werden. Nur beim Speichern in einen HTML‑Stream. |
| [GetAttachedFilesUrlPrefix](./getattachedfilesurlprefix/) | Geben Sie das URL‑Präfix der angehängten Dateien wie Bilder in der HTML‑Datei an. Nur beim Speichern in einen HTML‑Stream. |
| [SetAttachedFilesUrlPrefix](./setattachedfilesurlprefix/) | Geben Sie das URL‑Präfix der angehängten Dateien wie Bilder in der HTML‑Datei an. Nur beim Speichern in einen HTML‑Stream. |
| [GetDefaultFontName](./getdefaultfontname/) | Geben Sie den Standard‑Schriftartnamen für den HTML‑Export an; die Standardschrift wird verwendet, wenn die Schriftart des Stils nicht vorhanden ist. Wenn diese Eigenschaft null ist, verwendet Aspose.Cells eine universelle Schriftart, die dieselbe Familie wie die Originalschrift hat; der Standardwert ist null. |
| [SetDefaultFontName](./setdefaultfontname/) | Geben Sie den Standard‑Schriftartnamen für den HTML‑Export an; die Standardschrift wird verwendet, wenn die Schriftart des Stils nicht vorhanden ist. Wenn diese Eigenschaft null ist, verwendet Aspose.Cells eine universelle Schriftart, die dieselbe Familie wie die Originalschrift hat; der Standardwert ist null. |
| [GetAddGenericFont](./getaddgenericfont/) | Gibt an, ob eine generische Schriftart zur CSS‑font-family hinzugefügt werden soll. Der Standardwert ist true. |
| [SetAddGenericFont](./setaddgenericfont/) | Gibt an, ob eine generische Schriftart zur CSS‑font-family hinzugefügt werden soll. Der Standardwert ist true. |
| [GetWorksheetScalable](./getworksheetscalable/) | Gibt an, ob beim Speichern der Datei nach HTML über das Arbeitsblatt‑Zoomlevel gezoomt wird. Der Standardwert ist false. |
| [SetWorksheetScalable](./setworksheetscalable/) | Gibt an, ob beim Speichern der Datei nach HTML über das Arbeitsblatt‑Zoomlevel gezoomt wird. Der Standardwert ist false. |
| [IsExportComments](./isexportcomments/) | Gibt an, ob Kommentare beim Speichern der Datei nach HTML exportiert werden. Der Standardwert ist false. |
| [SetIsExportComments](./setisexportcomments/) | Gibt an, ob Kommentare beim Speichern der Datei nach HTML exportiert werden. Der Standardwert ist false. |
| [GetExportCommentsType](./getexportcommentstype/) | Stellt den Typ des Exports von Kommentaren in HTML‑Dateien dar. |
| [SetExportCommentsType](./setexportcommentstype/) | Stellt den Typ des Exports von Kommentaren in HTML‑Dateien dar. |
| [GetDisableDownlevelRevealedComments](./getdisabledownlevelrevealedcomments/) | Gibt an, ob Downlevel‑revealed bedingte Kommentare beim Exportieren der Datei nach HTML deaktiviert werden sollen. Der Standardwert ist false. |
| [SetDisableDownlevelRevealedComments](./setdisabledownlevelrevealedcomments/) | Gibt an, ob Downlevel‑revealed bedingte Kommentare beim Exportieren der Datei nach HTML deaktiviert werden sollen. Der Standardwert ist false. |
| [IsExpImageToTempDir](./isexpimagetotempdir/) | Gibt an, ob Bilddateien in ein temporäres Verzeichnis exportiert werden. Nur beim Speichern in einen HTML‑Stream. |
| [SetIsExpImageToTempDir](./setisexpimagetotempdir/) | Gibt an, ob Bilddateien in ein temporäres Verzeichnis exportiert werden. Nur beim Speichern in einen HTML‑Stream. |
| [GetImageScalable](./getimagescalable/) | Gibt an, ob eine skalierbare Einheit zur Beschreibung der Bildbreite verwendet wird, wenn eine skalierbare Einheit zur Beschreibung der Spaltenbreite verwendet wird. Der Standardwert ist true. |
| [SetImageScalable](./setimagescalable/) | Gibt an, ob eine skalierbare Einheit zur Beschreibung der Bildbreite verwendet wird, wenn eine skalierbare Einheit zur Beschreibung der Spaltenbreite verwendet wird. Der Standardwert ist true. |
| [GetWidthScalable](./getwidthscalable/) | Gibt an, ob die Spaltenbreite in Skalierungseinheiten nach HTML exportiert wird. Der Standardwert ist false. |
| [SetWidthScalable](./setwidthscalable/) | Gibt an, ob die Spaltenbreite in Skalierungseinheiten nach HTML exportiert wird. Der Standardwert ist false. |
| [GetExportSingleTab](./getexportsingletab/) | Gibt an, ob das einzelne Tabellenblatt exportiert wird, wenn die Datei nur ein Arbeitsblatt enthält. Der Standardwert ist false. |
| [SetExportSingleTab](./setexportsingletab/) | Gibt an, ob das einzelne Tabellenblatt exportiert wird, wenn die Datei nur ein Arbeitsblatt enthält. Der Standardwert ist false. |
| [GetExportImagesAsBase64](./getexportimagesasbase64/) | Gibt an, ob Bilder im Base64‑Format in HTML, MHTML oder EPUB gespeichert werden. |
| [SetExportImagesAsBase64](./setexportimagesasbase64/) | Gibt an, ob Bilder im Base64‑Format in HTML, MHTML oder EPUB gespeichert werden. |
| [GetExportActiveWorksheetOnly](./getexportactiveworksheetonly/) | Gibt an, ob nur das aktive Arbeitsblatt in die HTML‑Datei exportiert wird. Wenn true, wird nur das aktive Arbeitsblatt exportiert; wenn false, wird die gesamte Arbeitsmappe exportiert. Der Standardwert ist false. |
| [SetExportActiveWorksheetOnly](./setexportactiveworksheetonly/) | Gibt an, ob nur das aktive Arbeitsblatt in die HTML‑Datei exportiert wird. Wenn true, wird nur das aktive Arbeitsblatt exportiert; wenn false, wird die gesamte Arbeitsmappe exportiert. Der Standardwert ist false. |
| [GetExportPrintAreaOnly](./getexportprintareaonly/) | Gibt an, ob nur der Druckbereich in die HTML‑Datei exportiert wird. Der Standardwert ist false. |
| [SetExportPrintAreaOnly](./setexportprintareaonly/) | Gibt an, ob nur der Druckbereich in die HTML‑Datei exportiert wird. Der Standardwert ist false. |
| [GetExportArea](./getexportarea/) | Liest oder setzt den zu exportierenden CellArea des aktuell aktiven Arbeitsblatts. Wenn Sie dieses Attribut festlegen, wird der Druckbereich des aktuell aktiven Arbeitsblatts weggelassen. Nur der angegebene Bereich wird beim Speichern der Datei nach HTML exportiert. |
| [SetExportArea](./setexportarea/) | Liest oder setzt den zu exportierenden CellArea des aktuell aktiven Arbeitsblatts. Wenn Sie dieses Attribut festlegen, wird der Druckbereich des aktuell aktiven Arbeitsblatts weggelassen. Nur der angegebene Bereich wird beim Speichern der Datei nach HTML exportiert. |
| [GetParseHtmlTagInCell](./getparsehtmltagincell/) | Gibt an, ob HTML‑Tags (wie <c>&lt;div&gt;&lt;/div&gt;</c>) in einer Zelle als Zellwert geparst oder unverändert beibehalten werden sollen. Der Standardwert ist true. |
| [SetParseHtmlTagInCell](./setparsehtmltagincell/) | Gibt an, ob HTML‑Tags (wie <c>&lt;div&gt;&lt;/div&gt;</c>) in einer Zelle als Zellwert geparst oder unverändert beibehalten werden sollen. Der Standardwert ist true. |
| [GetHtmlCrossStringType](./gethtmlcrossstringtype/) | Gibt an, ob ein über mehrere Zellen erstreckender Text beim Speichern einer Excel‑Datei im HTML‑Format genauso wie in MS Excel angezeigt wird. Standardmäßig ist der Wert Default, sodass es bei übergreifenden Zeichenketten nur geringe Unterschiede zwischen den von Aspose.Cells und MS Excel erstellten HTML‑Dateien gibt. Für die Erstellung großer HTML‑Dateien ist die Leistung jedoch mehrere Male höher, wenn der Wert auf Cross gesetzt wird, im Vergleich zu Default oder Fit2Cell. |
| [SetHtmlCrossStringType](./sethtmlcrossstringtype/) | Gibt an, ob ein über mehrere Zellen erstreckender Text beim Speichern einer Excel‑Datei im HTML‑Format genauso wie in MS Excel angezeigt wird. Standardmäßig ist der Wert Default, sodass es bei übergreifenden Zeichenketten nur geringe Unterschiede zwischen den von Aspose.Cells und MS Excel erstellten HTML‑Dateien gibt. Für die Erstellung großer HTML‑Dateien ist die Leistung jedoch mehrere Male höher, wenn der Wert auf Cross gesetzt wird, im Vergleich zu Default oder Fit2Cell. |
| [GetHiddenColDisplayType](./gethiddencoldisplaytype/) | Versteckte Spalte (die Breite dieser Spalte ist 0) in Excel; bevor sie in das HTML‑Format gespeichert wird, wird bei HtmlHiddenColDisplayType = "Remove" die versteckte Spalte nicht ausgegeben, bei "Hidden" wird die Spalte ausgegeben, aber verborgen. Der Standardwert ist "Hidden" |
| [SetHiddenColDisplayType](./sethiddencoldisplaytype/) | Versteckte Spalte (die Breite dieser Spalte ist 0) in Excel; bevor sie in das HTML‑Format gespeichert wird, wird bei HtmlHiddenColDisplayType = "Remove" die versteckte Spalte nicht ausgegeben, bei "Hidden" wird die Spalte ausgegeben, aber verborgen. Der Standardwert ist "Hidden" |
| [GetHiddenRowDisplayType](./gethiddenrowdisplaytype/) | Versteckte Zeile (die Höhe dieser Zeile ist 0) in Excel, bevor sie in HTML-Format gespeichert wird, wenn HtmlHiddenRowDisplayType "Remove" ist, wird die versteckte Zeile nicht ausgegeben, wenn der Wert "Hidden" ist, wird die Zeile ausgegeben, aber verborgen, der Standardwert ist "Hidden" |
| [SetHiddenRowDisplayType](./sethiddenrowdisplaytype/) | Versteckte Zeile (die Höhe dieser Zeile ist 0) in Excel, bevor sie in HTML-Format gespeichert wird, wenn HtmlHiddenRowDisplayType "Remove" ist, wird die versteckte Zeile nicht ausgegeben, wenn der Wert "Hidden" ist, wird die Zeile ausgegeben, aber verborgen, der Standardwert ist "Hidden" |
| [GetEncoding](./getencoding/) | Wenn nicht festgelegt, wird Encoding.UTF8 als Standardkodierung verwendet. |
| [SetEncoding](./setencoding/) | Wenn nicht festgelegt, wird Encoding.UTF8 als Standardkodierung verwendet. |
| [GetImageOptions](./getimageoptions/) | Rufen Sie das ImageOrPrintOptions-Objekt vor dem Exportieren ab |
| [GetSaveAsSingleFile](./getsaveassinglefile/) | Gibt an, ob das HTML als einzelne Datei gespeichert wird. Der Standardwert ist false. |
| [SetSaveAsSingleFile](./setsaveassinglefile/) | Gibt an, ob das HTML als einzelne Datei gespeichert wird. Der Standardwert ist false. |
| [GetShowAllSheets](./getshowallsheets/) | Gibt an, ob beim Speichern als einzelne HTML-Datei alle Arbeitsblätter angezeigt werden. |
| [SetShowAllSheets](./setshowallsheets/) | Gibt an, ob beim Speichern als einzelne HTML-Datei alle Arbeitsblätter angezeigt werden. |
| [GetExportPageHeaders](./getexportpageheaders/) | Gibt an, ob Seitenköpfe exportiert werden. |
| [SetExportPageHeaders](./setexportpageheaders/) | Gibt an, ob Seitenköpfe exportiert werden. |
| [GetExportPageFooters](./getexportpagefooters/) | Gibt an, ob Seitenköpfe exportiert werden. |
| [SetExportPageFooters](./setexportpagefooters/) | Gibt an, ob Seitenköpfe exportiert werden. |
| [GetExportHiddenWorksheet](./getexporthiddenworksheet/) | Gibt an, ob der versteckte Arbeitsblattinhalt exportiert wird. Der Standardwert ist true. |
| [SetExportHiddenWorksheet](./setexporthiddenworksheet/) | Gibt an, ob der versteckte Arbeitsblattinhalt exportiert wird. Der Standardwert ist true. |
| [GetPresentationPreference](./getpresentationpreference/) | Gibt an, ob HTML- oder MHT-Datei die bevorzugte Darstellung ist. Der Standardwert ist false. Wenn Sie eine schönere Darstellung erhalten möchten, setzen Sie den Wert auf true. |
| [SetPresentationPreference](./setpresentationpreference/) | Gibt an, ob HTML- oder MHT-Datei die bevorzugte Darstellung ist. Der Standardwert ist false. Wenn Sie eine schönere Darstellung erhalten möchten, setzen Sie den Wert auf true. |
| [GetCellCssPrefix](./getcellcssprefix/) | Liest und setzt das Präfix des CSS-Namens, der Standardwert ist "". |
| [SetCellCssPrefix](./setcellcssprefix/) | Liest und setzt das Präfix des CSS-Namens, der Standardwert ist "". |
| [GetTableCssId](./gettablecssid/) | Liest und setzt das Präfix des Typ‑CSS‑Namens wie tr, col, td usw., die im Table‑Element enthalten sind, das das spezifische TableCssId‑Attribut hat. Der Standardwert ist "". |
| [SetTableCssId](./settablecssid/) | Liest und setzt das Präfix des Typ‑CSS‑Namens wie tr, col, td usw., die im Table‑Element enthalten sind, das das spezifische TableCssId‑Attribut hat. Der Standardwert ist "". |
| [IsFullPathLink](./isfullpathlink/) | Gibt an, ob Vollpfad-Links in sheet00x.htm, filelist.xml und tabstrip.htm verwendet werden. Der Standardwert ist false. |
| [SetIsFullPathLink](./setisfullpathlink/) | Gibt an, ob Vollpfad-Links in sheet00x.htm, filelist.xml und tabstrip.htm verwendet werden. Der Standardwert ist false. |
| [GetExportWorksheetCSSSeparately](./getexportworksheetcssseparately/) | Gibt an, ob das Arbeitsblatt‑CSS separat exportiert wird. Der Standardwert ist false. |
| [SetExportWorksheetCSSSeparately](./setexportworksheetcssseparately/) | Gibt an, ob das Arbeitsblatt‑CSS separat exportiert wird. Der Standardwert ist false. |
| [GetExportSimilarBorderStyle](./getexportsimilarborderstyle/) | Gibt an, ob ein ähnlicher Rahmenstil exportiert wird, wenn der Rahmenstil von Browsern nicht unterstützt wird. Wenn Sie die HTML‑ oder MHT‑Datei in Excel importieren möchten, behalten Sie den Standardwert bei. Der Standardwert ist false. |
| [SetExportSimilarBorderStyle](./setexportsimilarborderstyle/) | Gibt an, ob ein ähnlicher Rahmenstil exportiert wird, wenn der Rahmenstil von Browsern nicht unterstützt wird. Wenn Sie die HTML‑ oder MHT‑Datei in Excel importieren möchten, behalten Sie den Standardwert bei. Der Standardwert ist false. |
| [GetMergeEmptyTdType](./getmergeemptytdtype/) | Die Option, zusammenhängende leere Zellen (leere td‑Elemente) zu verbinden. Der Standardwert ist MergeEmptyTdType.Default. |
| [SetMergeEmptyTdType](./setmergeemptytdtype/) | Die Option, zusammenhängende leere Zellen (leere td‑Elemente) zu verbinden. Der Standardwert ist MergeEmptyTdType.Default. |
| [GetExportCellCoordinate](./getexportcellcoordinate/) | Gibt an, ob die Excel‑Koordinaten nicht leerer Zellen beim Speichern der Datei als HTML exportiert werden. Der Standardwert ist false. Wenn Sie das erzeugte HTML in Excel importieren möchten, behalten Sie den Standardwert bei. |
| [SetExportCellCoordinate](./setexportcellcoordinate/) | Gibt an, ob die Excel‑Koordinaten nicht leerer Zellen beim Speichern der Datei als HTML exportiert werden. Der Standardwert ist false. Wenn Sie das erzeugte HTML in Excel importieren möchten, behalten Sie den Standardwert bei. |
| [GetExportExtraHeadings](./getexportextraheadings/) | Gibt an, ob zusätzliche Überschriften exportiert werden, wenn die Textlänge länger als die maximale Anzeigespalte ist. Der Standardwert ist false. Wenn Sie die HTML‑Datei in Excel importieren möchten, behalten Sie den Standardwert bei. |
| [SetExportExtraHeadings](./setexportextraheadings/) | Gibt an, ob zusätzliche Überschriften exportiert werden, wenn die Textlänge länger als die maximale Anzeigespalte ist. Der Standardwert ist false. Wenn Sie die HTML‑Datei in Excel importieren möchten, behalten Sie den Standardwert bei. |
| [GetExportRowColumnHeadings](./getexportrowcolumnheadings/) | Gibt an, ob Zeilen‑ und Spaltenüberschriften des Arbeitsblatts beim Speichern in HTML‑Dateien exportiert werden. |
| [SetExportRowColumnHeadings](./setexportrowcolumnheadings/) | Gibt an, ob Zeilen‑ und Spaltenüberschriften des Arbeitsblatts beim Speichern in HTML‑Dateien exportiert werden. |
| [GetExportFormula](./getexportformula/) | Gibt an, ob Formeln beim Speichern der Datei als HTML exportiert werden. Der Standardwert ist true. Wenn Sie das erzeugte HTML in Excel importieren möchten, behalten Sie den Standardwert bei. |
| [SetExportFormula](./setexportformula/) | Gibt an, ob Formeln beim Speichern der Datei als HTML exportiert werden. Der Standardwert ist true. Wenn Sie das erzeugte HTML in Excel importieren möchten, behalten Sie den Standardwert bei. |
| [GetAddTooltipText](./getaddtooltiptext/) | Gibt an, ob Tooltip‑Text hinzugefügt wird, wenn die Daten nicht vollständig angezeigt werden können. Der Standardwert ist false. |
| [SetAddTooltipText](./setaddtooltiptext/) | Gibt an, ob Tooltip‑Text hinzugefügt wird, wenn die Daten nicht vollständig angezeigt werden können. Der Standardwert ist false. |
| [GetExportGridLines](./getexportgridlines/) | Gibt an, ob Rasterlinien exportiert werden. Der Standardwert ist false. |
| [SetExportGridLines](./setexportgridlines/) | Gibt an, ob Rasterlinien exportiert werden. Der Standardwert ist false. |
| [GetExportBogusRowData](./getexportbogusrowdata/) | Gibt an, ob falsche Daten der unteren Zeile exportiert werden. Der Standardwert ist true. Wenn Sie die HTML‑ oder MHT‑Datei in Excel importieren möchten, behalten Sie den Standardwert bei. |
| [SetExportBogusRowData](./setexportbogusrowdata/) | Gibt an, ob falsche Daten der unteren Zeile exportiert werden. Der Standardwert ist true. Wenn Sie die HTML‑ oder MHT‑Datei in Excel importieren möchten, behalten Sie den Standardwert bei. |
| [GetExcludeUnusedStyles](./getexcludeunusedstyles/) | Gibt an, ob ungenutzte Stile ausgeschlossen werden. Für die erzeugten HTML‑Dateien kann das Ausschließen ungenutzter Stile die Dateigröße verkleinern, ohne die visuellen Effekte zu beeinträchtigen. Daher ist der Standardwert dieser Eigenschaft true. Wenn der Benutzer alle Stile in der Arbeitsmappe für das erzeugte HTML beibehalten muss (z. B. wenn die Arbeitsmappe später aus dem erzeugten HTML wiederhergestellt werden soll), setzen Sie diese Eigenschaft auf false. |
| [SetExcludeUnusedStyles](./setexcludeunusedstyles/) | Gibt an, ob ungenutzte Stile ausgeschlossen werden. Für die erzeugten HTML‑Dateien kann das Ausschließen ungenutzter Stile die Dateigröße verkleinern, ohne die visuellen Effekte zu beeinträchtigen. Daher ist der Standardwert dieser Eigenschaft true. Wenn der Benutzer alle Stile in der Arbeitsmappe für das erzeugte HTML beibehalten muss (z. B. wenn die Arbeitsmappe später aus dem erzeugten HTML wiederhergestellt werden soll), setzen Sie diese Eigenschaft auf false. |
| [GetExportDocumentProperties](./getexportdocumentproperties/) | Gibt an, ob Dokumenteigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML- oder MHT-Datei nach Excel importieren möchten, lassen Sie den Standardwert unverändert. |
| [SetExportDocumentProperties](./setexportdocumentproperties/) | Gibt an, ob Dokumenteigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML- oder MHT-Datei nach Excel importieren möchten, lassen Sie den Standardwert unverändert. |
| [GetExportWorksheetProperties](./getexportworksheetproperties/) | Gibt an, ob Arbeitsblatt-Eigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML- oder MHT-Datei nach Excel importieren möchten, lassen Sie den Standardwert unverändert. |
| [SetExportWorksheetProperties](./setexportworksheetproperties/) | Gibt an, ob Arbeitsblatt-Eigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML- oder MHT-Datei nach Excel importieren möchten, lassen Sie den Standardwert unverändert. |
| [GetExportWorkbookProperties](./getexportworkbookproperties/) | Gibt an, ob Arbeitsmappen-Eigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML- oder MHT-Datei nach Excel importieren möchten, lassen Sie den Standardwert unverändert. |
| [SetExportWorkbookProperties](./setexportworkbookproperties/) | Gibt an, ob Arbeitsmappen-Eigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML- oder MHT-Datei nach Excel importieren möchten, lassen Sie den Standardwert unverändert. |
| [GetExportFrameScriptsAndProperties](./getexportframescriptsandproperties/) | Gibt an, ob Frame‑Skripte und Dokumenteigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML- oder MHT-Datei nach Excel importieren möchten, lassen Sie den Standardwert unverändert. |
| [SetExportFrameScriptsAndProperties](./setexportframescriptsandproperties/) | Gibt an, ob Frame‑Skripte und Dokumenteigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML- oder MHT-Datei nach Excel importieren möchten, lassen Sie den Standardwert unverändert. |
| [GetExportDataOptions](./getexportdataoptions/) | Gibt die Regel für den Export von HTML-Dateidaten an. Der Standardwert ist All. |
| [SetExportDataOptions](./setexportdataoptions/) | Gibt die Regel für den Export von HTML-Dateidaten an. Der Standardwert ist All. |
| [GetLinkTargetType](./getlinktargettype/) | Gibt den Typ des Zielattributs im <c>&lt;a&gt;</c>-Link an. Der Standardwert ist HtmlLinkTargetType.Parent. |
| [SetLinkTargetType](./setlinktargettype/) | Gibt den Typ des Zielattributs im <c>&lt;a&gt;</c>-Link an. Der Standardwert ist HtmlLinkTargetType.Parent. |
| [IsIECompatible](./isiecompatible/) | Gibt an, ob das ausgegebene HTML mit dem IE‑Browser kompatibel ist. Der Standardwert ist false. |
| [SetIsIECompatible](./setisiecompatible/) | Gibt an, ob das ausgegebene HTML mit dem IE‑Browser kompatibel ist. Der Standardwert ist false. |
| [GetFormatDataIgnoreColumnWidth](./getformatdataignorecolumnwidth/) | Gibt an, ob die gesamten formatierten Zellen­daten angezeigt werden sollen, wenn sie die Spalte überlaufen. Wenn true, wird die Spaltenbreite ignoriert und die gesamten Zellen­daten werden exportiert. Wenn false, werden die Daten wie in Excel exportiert. Der Standardwert ist false. |
| [SetFormatDataIgnoreColumnWidth](./setformatdataignorecolumnwidth/) | Gibt an, ob die gesamten formatierten Zellen­daten angezeigt werden sollen, wenn sie die Spalte überlaufen. Wenn true, wird die Spaltenbreite ignoriert und die gesamten Zellen­daten werden exportiert. Wenn false, werden die Daten wie in Excel exportiert. Der Standardwert ist false. |
| [GetCalculateFormula](./getcalculateformula/) | Gibt an, ob Formeln vor dem Speichern der HTML‑Datei berechnet werden sollen. |
| [SetCalculateFormula](./setcalculateformula/) | Gibt an, ob Formeln vor dem Speichern der HTML‑Datei berechnet werden sollen. |
| [IsJsBrowserCompatible](./isjsbrowsercompatible/) | Gibt an, ob JavaScript mit Browsern kompatibel ist, die JavaScript nicht unterstützen. Der Standardwert ist true. |
| [SetIsJsBrowserCompatible](./setisjsbrowsercompatible/) | Gibt an, ob JavaScript mit Browsern kompatibel ist, die JavaScript nicht unterstützen. Der Standardwert ist true. |
| [IsMobileCompatible](./ismobilecompatible/) | Gibt an, ob das ausgegebene HTML mit mobilen Geräten kompatibel ist. Der Standardwert ist false. |
| [SetIsMobileCompatible](./setismobilecompatible/) | Gibt an, ob das ausgegebene HTML mit mobilen Geräten kompatibel ist. Der Standardwert ist false. |
| [GetCssStyles](./getcssstyles/) | Liest oder legt die zusätzlichen CSS‑Stile für den Formatter fest. Wirkt nur, wenn SaveAsSingleFile true ist. |
| [SetCssStyles](./setcssstyles/) | Liest oder legt die zusätzlichen CSS‑Stile für den Formatter fest. Wirkt nur, wenn SaveAsSingleFile true ist. |
| [GetHideOverflowWrappedText](./gethideoverflowwrappedtext/) | Gibt an, ob überlaufender Text ausgeblendet werden soll, wenn das Zellenformat auf Zeilenumbruch gesetzt ist. Der Standardwert ist false. |
| [SetHideOverflowWrappedText](./sethideoverflowwrappedtext/) | Gibt an, ob überlaufender Text ausgeblendet werden soll, wenn das Zellenformat auf Zeilenumbruch gesetzt ist. Der Standardwert ist false. |
| [IsBorderCollapsed](./isbordercollapsed/) | Gibt an, ob Tabellenrahmen zusammengeführt werden. Der Standardwert ist true. |
| [SetIsBorderCollapsed](./setisbordercollapsed/) | Gibt an, ob Tabellenrahmen zusammengeführt werden. Der Standardwert ist true. |
| [GetEncodeEntityAsCode](./getencodeentityascode/) | Gibt an, ob HTML‑Zeichen­entitäten durch dezimale Codes ersetzt werden (z. B. "&amp;nbsp;" wird durch "&amp;#160;" ersetzt). Der Standardwert ist false. |
| [SetEncodeEntityAsCode](./setencodeentityascode/) | Gibt an, ob HTML‑Zeichen­entitäten durch dezimale Codes ersetzt werden (z. B. "&amp;nbsp;" wird durch "&amp;#160;" ersetzt). Der Standardwert ist false. |
| [GetOfficeMathOutputMode](./getofficemathoutputmode/) | Gibt an, wie OfficeMath‑Objekte nach HTML exportiert werden. Der Standardwert ist Image. |
| [SetOfficeMathOutputMode](./setofficemathoutputmode/) | Gibt an, wie OfficeMath‑Objekte nach HTML exportiert werden. Der Standardwert ist Image. |
| [GetCellNameAttribute](./getcellnameattribute/) | Gibt das Attribut an, das den zu schreibenden Zellnamen kennzeichnet (z. B. Wenn der Wert "id" ist, wird für die Zelle "A1" die Ausgabe &lt;td id='A1'&gt; sein). Der Standardwert ist null. |
| [SetCellNameAttribute](./setcellnameattribute/) | Gibt das Attribut an, das den zu schreibenden Zellnamen kennzeichnet (z. B. Wenn der Wert "id" ist, wird für die Zelle "A1" die Ausgabe &lt;td id='A1'&gt; sein). Der Standardwert ist null. |
| [GetDisableCss](./getdisablecss/) | Gibt an, ob nur Inline‑Stile angewendet werden, ohne CSS zu verwenden. Der Standardwert ist false. |
| [SetDisableCss](./setdisablecss/) | Gibt an, ob nur Inline‑Stile angewendet werden, ohne CSS zu verwenden. Der Standardwert ist false. |
| [GetEnableCssCustomProperties](./getenablecsscustomproperties/) | Optimiert die HTML‑Ausgabe durch Verwendung von CSS‑Custom‑Properties. Zum Beispiel muss bei mehreren Vorkommen desselben Base64‑Bildes das Bilddaten nur einmal gespeichert werden, wodurch die Leistung des resultierenden HTML verbessert wird. Der Standardwert ist false. |
| [SetEnableCssCustomProperties](./setenablecsscustomproperties/) | Optimiert die HTML‑Ausgabe durch Verwendung von CSS‑Custom‑Properties. Zum Beispiel muss bei mehreren Vorkommen desselben Base64‑Bildes das Bilddaten nur einmal gespeichert werden, wodurch die Leistung des resultierenden HTML verbessert wird. Der Standardwert ist false. |
| [GetHtmlVersion](./gethtmlversion/) | Gibt die HTML‑Standardversion an, die beim Speichern des HTML‑Formats verwendet werden soll. Der Standardwert ist HtmlVersion.Default. |
| [SetHtmlVersion](./sethtmlversion/) | Gibt die HTML‑Standardversion an, die beim Speichern des HTML‑Formats verwendet werden soll. Der Standardwert ist HtmlVersion.Default. |
| [GetSheetSet](./getsheetset/) | Liest oder legt die zu rendernden Arbeitsblätter fest. Standard ist: Alle sichtbaren Arbeitsblätter in der Arbeitsmappe: Aspose.Cells.Rendering.SheetSet.Visible. |
| [SetSheetSet](./setsheetset/) | Liest oder legt die zu rendernden Arbeitsblätter fest. Standard ist: Alle sichtbaren Arbeitsblätter in der Arbeitsmappe: Aspose.Cells.Rendering.SheetSet.Visible. |
| [GetLayoutMode](./getlayoutmode/) | Liest oder legt den Layout‑Modus beim Speichern nach HTML fest. Der Standardwert ist HtmlLayoutMode.Normal. |
| [SetLayoutMode](./setlayoutmode/) | Liest oder legt den Layout‑Modus beim Speichern nach HTML fest. Der Standardwert ist HtmlLayoutMode.Normal. |
| [GetEmbeddedFontType](./getembeddedfonttype/) | Liest oder legt den Typ der Einbettung von Schriftdateien in die HTML‑Datei fest. Der Standardwert ist HtmlEmbeddedFontType.None, was bedeutet, dass keine Schrift in HTML eingebettet wird. |
| [SetEmbeddedFontType](./setembeddedfonttype/) | Liest oder legt den Typ der Einbettung von Schriftdateien in die HTML‑Datei fest. Der Standardwert ist HtmlEmbeddedFontType.None, was bedeutet, dass keine Schrift in HTML eingebettet wird. |
| [GetExportNamedRangeAnchors](./getexportnamedrangeanchors/) | Gibt an, ob Anker-Elemente für benannte Bereiche beim Speichern als HTML exportiert werden sollen. Der Standardwert ist true. |
| [SetExportNamedRangeAnchors](./setexportnamedrangeanchors/) | Gibt an, ob Anker-Elemente für benannte Bereiche beim Speichern als HTML exportiert werden sollen. Der Standardwert ist true. |
| [GetDataBarRenderMode](./getdatabarrendermode/) | Stellt den Modus dar, wie DataBar beim Konvertieren von Excel-Dateien in HTML-Dateien gerendert wird. Der Standardwert ist DataBarRenderMode.BackgroundColor. |
| [SetDataBarRenderMode](./setdatabarrendermode/) | Stellt den Modus dar, wie DataBar beim Konvertieren von Excel-Dateien in HTML-Dateien gerendert wird. Der Standardwert ist DataBarRenderMode.BackgroundColor. |
| [GetSpaceMode](./getspacemode/) | Gibt an, wie Leerzeichen in der HTML-Ausgabe gerendert werden. Diese Option wird derzeit nur auf numerische Formate (z. B. Buchhaltungsformat) angewendet. Der Standardwert ist HtmlSpaceMode.Css. |
| [SetSpaceMode](./setspacemode/) | Gibt an, wie Leerzeichen in der HTML-Ausgabe gerendert werden. Diese Option wird derzeit nur auf numerische Formate (z. B. Buchhaltungsformat) angewendet. Der Standardwert ist HtmlSpaceMode.Css. |
| [GetSaveFormat](./getsaveformat/) | Ermittelt das Dateiformat zum Speichern. |
| [GetClearData](./getcleardata/) | Leert die Arbeitsmappe nach dem Speichern der Datei. |
| [SetClearData](./setcleardata/) | Leert die Arbeitsmappe nach dem Speichern der Datei. |
| [GetCachedFileFolder](./getcachedfilefolder/) | Der Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können. |
| [SetCachedFileFolder](./setcachedfilefolder/) | Der Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können. |
| [GetValidateMergedAreas](./getvalidatemergedareas/) | Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden sollen. |
| [SetValidateMergedAreas](./setvalidatemergedareas/) | Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden sollen. |
| [GetMergeAreas](./getmergeareas/) | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden sollen. |
| [SetMergeAreas](./setmergeareas/) | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden sollen. |
| [GetCreateDirectory](./getcreatedirectory/) | Wenn wahr und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt. |
| [SetCreateDirectory](./setcreatedirectory/) | Wenn wahr und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt. |
| [GetSortNames](./getsortnames/) | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden sollen. |
| [SetSortNames](./setsortnames/) | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden sollen. |
| [GetSortExternalNames](./getsortexternalnames/) | Gibt an, ob externe definierte Namen vor dem Speichern der Datei sortiert werden sollen. |
| [SetSortExternalNames](./setsortexternalnames/) | Gibt an, ob externe definierte Namen vor dem Speichern der Datei sortiert werden sollen. |
| [GetRefreshChartCache](./getrefreshchartcache/) | Gibt an, ob die neuesten Daten des Diagramms zwischengespeichert werden sollen. |
| [SetRefreshChartCache](./setrefreshchartcache/) | Gibt an, ob die neuesten Daten des Diagramms zwischengespeichert werden sollen. |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | Ob Beschränkungen der Excel-Datei geprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht, einen Zeichenwert länger als 32 KB einzugeben. Wenn Sie einen Wert länger als 32 KB eingeben, wird er abgeschnitten. |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | Ob Beschränkungen der Excel-Datei geprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht, einen Zeichenwert länger als 32 KB einzugeben. Wenn Sie einen Wert länger als 32 KB eingeben, wird er abgeschnitten. |
| [GetUpdateSmartArt](./getupdatesmartart/) | Gibt an, ob die SmartArt-Einstellung aktualisiert wird. Der Standardwert ist false. |
| [SetUpdateSmartArt](./setupdatesmartart/) | Gibt an, ob die SmartArt-Einstellung aktualisiert wird. Der Standardwert ist false. |
| [GetEncryptDocumentProperties](./getencryptdocumentproperties/) | Gibt an, ob Dokumenteigenschaften beim Speichern als .xls-Datei verschlüsselt werden. Der Standardwert ist true. |
| [SetEncryptDocumentProperties](./setencryptdocumentproperties/) | Gibt an, ob Dokumenteigenschaften beim Speichern als .xls-Datei verschlüsselt werden. Der Standardwert ist true. |
