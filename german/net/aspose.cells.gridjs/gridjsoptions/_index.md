---
title: "Klasse GridJsOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridJs.GridJsOptions-Klasse. Stellt alle Ladeoptionen für GridJs dar"
type: docs
url: /de/net/aspose.cells.gridjs/gridjsoptions/
---
## GridJsOptions class

Stellt alle Ladeoptionen für GridJs dar.

```csharp
public class GridJsOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [GridJsOptions](gridjsoptions/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AutoFitColumnsOnLoad](../../aspose.cells.gridjs/gridjsoptions/autofitcolumnsonload/) { get; set; } | Gibt an, ob die Spaltenbreite beim Laden der Datei automatisch angepasst werden soll, der Standardwert ist false. |
| [AutoFitRowsHeightOnLoad](../../aspose.cells.gridjs/gridjsoptions/autofitrowsheightonload/) { get; set; } | Gibt an, ob die Zeilenhöhe beim Laden der Datei automatisch angepasst werden soll, der Standardwert ist false. |
| [AutoOptimizeForLargeCells](../../aspose.cells.gridjs/gridjsoptions/autooptimizeforlargecells/) { get; set; } | Liest/Setzt, ob die Ladeleistung für Arbeitsblätter mit großen Zellen automatisch optimiert werden soll. Es werden einige Stile /Ränder ignoriert, um die Ladezeit zu verkürzen. Der Standardwert ist true. |
| [BaseRouteName](../../aspose.cells.gridjs/gridjsoptions/baseroutename/) { get; set; } | Liest/Setzt den Basisnamen der Routen-URL für den GridJs-Controller. Der Standard ist GridJs2 |
| [CustomPdfSaveOptions](../../aspose.cells.gridjs/gridjsoptions/custompdfsaveoptions/) { get; set; } | Liest/Setzt benutzerdefinierte PdfSaveOptions für den PDF-Export. Wenn gesetzt, werden diese anstelle der Standardoptionen verwendet. Der Standardwert ist null. |
| [EmptySheetMaxCol](../../aspose.cells.gridjs/gridjsoptions/emptysheetmaxcol/) { get; set; } | Liest/Setzt die standardmäßige maximale Spaltenzahl für ein leeres Arbeitsblatt. Der Standardwert ist 15. |
| [EmptySheetMaxRow](../../aspose.cells.gridjs/gridjsoptions/emptysheetmaxrow/) { get; set; } | Liest/Setzt die standardmäßige maximale Zeilenzahl für ein leeres Arbeitsblatt. Der Standardwert ist 12. |
| [EnableChartClientRendering](../../aspose.cells.gridjs/gridjsoptions/enablechartclientrendering/) { get; set; } | Liest/Setzt, ob das clientseitige Diagrammrendering aktiviert werden soll. Wenn auf false gesetzt, gibt GridJs nur Diagrammbilder/-formen aus und erfordert kein clientseitiges Diagrammrendering. Der Standardwert ist true. |
| [FileCacheDirectory](../../aspose.cells.gridjs/gridjsoptions/filecachedirectory/) { get; set; } | Liest/Setzt das Cache-Verzeichnis zum Speichern von Tabellenkalkulationsdateien. Wir müssen es vor der Verwendung von GridJs auf einen bestimmten Pfad setzen. |
| [FontFolders](../../aspose.cells.gridjs/gridjsoptions/fontfolders/) { get; set; } | Liest/Setzt die Schriftordner für Schriften in den gerenderten Bildern/Formen |
| [IgnoreEmptyContent](../../aspose.cells.gridjs/gridjsoptions/ignoreemptycontent/) { get; set; } | Liest/Setzt, ob der maximale Bereich angezeigt werden soll, der Daten, Stil, zusammengeführte Zellen und Formen enthält. Wenn die letzte Zeile oder Spalte Zellen ohne Wert und Formel, aber mit benutzerdefiniertem Stil enthält, wird diese Zeile/Spalte nicht angezeigt, wenn dieser Wert true ist. Der Standardwert ist true. |
| [IsCollaborative](../../aspose.cells.gridjs/gridjsoptions/iscollaborative/) { get; set; } | Liest/Setzt, ob kollaboratives Bearbeiten unterstützt werden soll, der Standard ist false. |
| [IslimitShapeOrImage](../../aspose.cells.gridjs/gridjsoptions/islimitshapeorimage/) { get; set; } | Liest/Setzt, ob die Gesamtzahl der angezeigten Formen/Bilder in einem Arbeitsblatt begrenzt werden soll. Wenn true, begrenzt GridJs die Gesamtzahl der angezeigten Formen oder Bilder in einem Arbeitsblatt auf MaxShapeOrImageCount. Der Standardwert ist true. |
| [IsWasm](../../aspose.cells.gridjs/gridjsoptions/iswasm/) { get; set; } | Liest/Setzt, ob GridJs innerhalb eines Browser-WebAssembly-Hosts statt eines Serverprozesses ausgeführt wird. Wenn true, wird kein FileCacheDirectory / Festplatte / Interrupt-Thread-Pfad verwendet, und der Dateicache muss von CacheImp stammen, da ein Browser-Host keinen lokalen Datenträger hat. Es wählt zur Laufzeit Codepfade aus, sodass eine Aspose.Cells.GridJs.dll beide Hosts bedient. Der Standardwert ist false. |
| [JsonCache](../../aspose.cells.gridjs/gridjsoptions/jsoncache/) { get; set; } | Liest/Setzt JSON-Cache-Konfigurationsoptionen. Steuert das Verhalten des Speicher- (L1) und Festplatten- (L2) Caches für das erzeugte Arbeitsbuch-JSON. |
| [LazyLoading](../../aspose.cells.gridjs/gridjsoptions/lazyloading/) { get; set; } | Liest/Setzt, ob nur das aktive Arbeitsblatt geladen werden soll, der Standard ist false. |
| [MaxPdfSaveSeconds](../../aspose.cells.gridjs/gridjsoptions/maxpdfsaveseconds/) { get; set; } | Liest/Setzt die maximalen Timeout‑Sekunden beim Speichern als PDF. Der Standardwert ist 10. |
| [MaxShapeOrImageCount](../../aspose.cells.gridjs/gridjsoptions/maxshapeorimagecount/) { get; set; } | Liest/Setzt die Gesamtzahl der angezeigten Formen oder Bilder im aktiven Blatt, wirksam wenn IslimitShapeOrImage=true. Der Standardwert ist 100. |
| [MaxShapeOrImageWidthOrHeight](../../aspose.cells.gridjs/gridjsoptions/maxshapeorimagewidthorheight/) { get; set; } | Liest/Setzt die maximale Breite oder Höhe für eine Form oder ein Bild, GridJs ignoriert Formen oder Bilder mit einer Breite oder Höhe, die größer ist. Wirksam wenn IslimitShapeOrImage=true. Der Standardwert ist 10000. |
| [MaxTotalShapeOrImageCount](../../aspose.cells.gridjs/gridjsoptions/maxtotalshapeorimagecount/) { get; set; } | Liest/Setzt die Gesamtzahl der angezeigten Formen oder Bilder in der Arbeitsmappe, wirksam wenn IslimitShapeOrImage=true. Der Standardwert ist 300. |
| [MessageTopic](../../aspose.cells.gridjs/gridjsoptions/messagetopic/) { get; set; } | Liest/Setzt die Websocket-Ziele, die mit \"/topic\" beginnen. Der Standard ist \"/topic/opr\". Wird nur im Kollaborationsmodus verwendet. |
| [PictureCacheDirectory](../../aspose.cells.gridjs/gridjsoptions/picturecachedirectory/) { get; set; } | Liest/Setzt das Cache-Verzeichnis für Bilder. (Dies wird wirksam, wenn GridJsWorkbook.CacheImp null ist) Der Standardpfad ist \"_piccache\" im FileCacheDirectory. |
| [SameImageDetecting](../../aspose.cells.gridjs/gridjsoptions/sameimagedetecting/) { get; set; } | Liest/Setzt, ob geprüft wird, ob Bilder dieselbe Quelle haben, der Standardwert ist true. |
| [SaveHtmlAsZip](../../aspose.cells.gridjs/gridjsoptions/savehtmlaszip/) { get; set; } | Liest/Setzt, ob HTML-Dateien als ZIP-Archiv gespeichert werden, der Standardwert ist false. |
| [ShowChartSheet](../../aspose.cells.gridjs/gridjsoptions/showchartsheet/) { get; set; } | Liest/Setzt, ob das Diagramm-Arbeitsblatt angezeigt wird. Der Standardwert ist false. |
| [SkipInvisibleShapes](../../aspose.cells.gridjs/gridjsoptions/skipinvisibleshapes/) { get; set; } | Liest/Setzt, ob Formen übersprungen werden sollen, die für die UI unsichtbar sind, der Standardwert ist true. |
| [UsePrintArea](../../aspose.cells.gridjs/gridjsoptions/useprintarea/) { get; set; } | Liest/Setzt, ob PageSetup.PrintArea für den UI-Anzeigebereich verwendet wird, wenn das Arbeitsblatt eine PageSetup-Einstellung für PrintArea hat. Der Standardwert ist false. |

## Felder

| Name | Beschreibung |
| --- | --- |
| [CacheImp](../../aspose.cells.gridjs/gridjsoptions/cacheimp/) | Benutzerdefinierte Implementierung für den Cache-Speicher. Wenn Sie den Cache stromweise speichern möchten, müssen Sie ihn setzen und implementieren. Ein WebAssembly-Host (IsWasm = true) muss ihn setzen, da für den Standard-Dateicache kein lokaler Datenträger vorhanden ist. |
| [RedactionUseClientGenerateId](../../aspose.cells.gridjs/gridjsoptions/redactionuseclientgenerateid/) | Gibt an, ob bei redaktionsbezogenen Vorgängen die vom Client generierte ID anstelle der tatsächlichen Shape-ID verwendet wird. |

### Siehe auch

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


