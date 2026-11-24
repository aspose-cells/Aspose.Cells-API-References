---
title: "Klasse Config"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Klasse Aspose.Cells.GridJs.Config. Stellt alle statischen Einstellungen für GridJs dar."
type: docs
url: /de/net/aspose.cells.gridjs/config/
---
## Config class

Stellt alle statischen Einstellungen für GridJs dar

```csharp
public class Config
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [Config](config/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| static [AutoFitColumnsOnLoad](../../aspose.cells.gridjs/config/autofitcolumnsonload/) { get; set; } | Gibt an, ob die Spaltenbreiten beim Laden der Datei automatisch angepasst werden sollen. Der Standardwert ist `false`. Hinweis: Wird dieser Wert auf `true` gesetzt, wird nach dem Laden ein automatisches Anpassen aller Spalten durchgeführt, was die Leistung merklich beeinträchtigen kann. |
| static [AutoFitRowsHeightOnLoad](../../aspose.cells.gridjs/config/autofitrowsheightonload/) { get; set; } | Gibt an, ob die Zeilenhöhen beim Laden der Datei automatisch angepasst werden sollen. Der Standardwert ist `false`. Hinweis: Wird dieser Wert auf `true` gesetzt, wird nach dem Laden ein automatisches Anpassen aller Zeilen durchgeführt, was die Leistung merklich beeinträchtigen kann. |
| static [AutoOptimizeForLargeCells](../../aspose.cells.gridjs/config/autooptimizeforlargecells/) { get; set; } | Liest/Setzt, ob die Ladeleistung für Arbeitsblätter mit großen Zellen automatisch optimiert werden soll. Es werden einige Stile /Ränder ignoriert, um die Ladezeit zu verkürzen. Der Standardwert ist true. |
| static [BaseRouteName](../../aspose.cells.gridjs/config/baseroutename/) { get; set; } | Liest/Setzt den Basisroutennamen für die GridJs‑Controller‑URL. Der Standardwert ist "/GridJs2". |
| static [CustomPdfSaveOptions](../../aspose.cells.gridjs/config/custompdfsaveoptions/) { get; set; } | Liest/Setzt benutzerdefinierte PdfSaveOptions für den PDF-Export. Wenn gesetzt, werden diese anstelle der Standardoptionen verwendet. Der Standardwert ist null. |
| static [EmptySheetMaxCol](../../aspose.cells.gridjs/config/emptysheetmaxcol/) { get; set; } | Liest/Setzt die standardmäßige maximale Spaltenzahl für ein leeres Arbeitsblatt. Der Standardwert ist 15. |
| static [EmptySheetMaxRow](../../aspose.cells.gridjs/config/emptysheetmaxrow/) { get; set; } | Liest/Setzt die standardmäßige maximale Zeilenzahl für ein leeres Arbeitsblatt. Der Standardwert ist 12. |
| static [EnableChartClientRendering](../../aspose.cells.gridjs/config/enablechartclientrendering/) { get; set; } | Liest/Setzt, ob die clientseitige Diagrammdarstellung aktiviert werden soll. Wenn auf false gesetzt, greift GridJs nur auf serverseitig erzeugte Diagrammbilder/-formen zurück. Der Standardwert ist true. |
| static [FileCacheDirectory](../../aspose.cells.gridjs/config/filecachedirectory/) { get; set; } | Liest/Setzt das Cache-Verzeichnis zum Speichern von Tabellenkalkulationsdateien. Wir müssen es vor der Verwendung von GridJs auf einen bestimmten Pfad setzen. |
| static [IgnoreEmptyContent](../../aspose.cells.gridjs/config/ignoreemptycontent/) { get; set; } | Liest/Setzt, ob der maximale Bereich angezeigt werden soll, der Daten, Stil, zusammengeführte Zellen und Formen enthält. Wenn die letzte Zeile oder Spalte Zellen ohne Wert und Formel, aber mit benutzerdefiniertem Stil enthält, wird diese Zeile/Spalte nicht angezeigt, wenn dieser Wert true ist. Der Standardwert ist true. |
| static [IsCollaborative](../../aspose.cells.gridjs/config/iscollaborative/) { get; set; } | Liest/Setzt, ob kollaboratives Bearbeiten unterstützt werden soll, der Standard ist false. |
| static [IslimitShapeOrImage](../../aspose.cells.gridjs/config/islimitshapeorimage/) { get; set; } | Liest/Setzt, ob die Gesamtzahl der angezeigten Formen/Bilder in einem Arbeitsblatt begrenzt werden soll. Wenn true, begrenzt GridJs die Gesamtzahl der angezeigten Formen oder Bilder in einem Arbeitsblatt auf MaxShapeOrImageCount. Der Standardwert ist true. |
| static [IsWasm](../../aspose.cells.gridjs/config/iswasm/) { get; set; } | Liest/Setzt, ob GridJs in einem Browser‑WebAssembly‑Host anstelle eines Serverprozesses ausgeführt wird. Wenn true, wird kein FileCacheDirectory / Festplatte / Interrupt‑Thread‑Pfad verwendet und der Dateicache muss von GridJsOptions.CacheImp stammen. GridJsOptions.IsWasm setzt dies, wenn der GridJs‑Dienst erstellt wird, sodass eine Aspose.Cells.GridJs.dll beide Hosts bedienen kann. Der Standardwert ist false. |
| static [JsonCache](../../aspose.cells.gridjs/config/jsoncache/) { get; set; } | Liest/Setzt JSON-Cache-Konfigurationsoptionen. Steuert das Verhalten des Speicher- (L1) und Festplatten- (L2) Caches für das erzeugte Arbeitsbuch-JSON. |
| static [LazyLoading](../../aspose.cells.gridjs/config/lazyloading/) { get; set; } | Liest/Setzt, ob nur das aktive Arbeitsblatt geladen werden soll, der Standard ist false. |
| static [MaxPdfSaveSeconds](../../aspose.cells.gridjs/config/maxpdfsaveseconds/) { get; set; } | Liest/Setzt die maximalen Timeout‑Sekunden beim Speichern als PDF. Der Standardwert ist 10. |
| static [MaxShapeOrImageCount](../../aspose.cells.gridjs/config/maxshapeorimagecount/) { get; set; } | Liest/Setzt die Gesamtzahl der angezeigten Formen oder Bilder im aktiven Blatt, wirksam wenn IslimitShapeOrImage=true. Der Standardwert ist 100. |
| static [MaxShapeOrImageWidthOrHeight](../../aspose.cells.gridjs/config/maxshapeorimagewidthorheight/) { get; set; } | Liest/Setzt die maximale Breite oder Höhe für eine Form oder ein Bild, GridJs ignoriert Formen oder Bilder mit einer Breite oder Höhe, die größer ist. Wirksam wenn IslimitShapeOrImage=true. Der Standardwert ist 10000. |
| static [MaxTotalShapeOrImageCount](../../aspose.cells.gridjs/config/maxtotalshapeorimagecount/) { get; set; } | Liest/Setzt die Gesamtzahl der angezeigten Formen oder Bilder in der Arbeitsmappe, wirksam wenn IslimitShapeOrImage=true. Der Standardwert ist 300. |
| static [MessageTopic](../../aspose.cells.gridjs/config/messagetopic/) { get; set; } | Liest/Setzt die Websocket-Ziele, die mit \"/topic\" beginnen. Der Standard ist \"/topic/opr\". Wird nur im Kollaborationsmodus verwendet. |
| static [PictureCacheDirectory](../../aspose.cells.gridjs/config/picturecachedirectory/) { get; set; } | Liest/Setzt das Cache-Verzeichnis für Bilder. (Dies wird wirksam, wenn GridJsWorkbook.CacheImp null ist) Der Standardpfad ist \"_piccache\" im FileCacheDirectory. |
| static [SameImageDetecting](../../aspose.cells.gridjs/config/sameimagedetecting/) { get; set; } | Liest/Setzt, ob geprüft wird, ob Bilder dieselbe Quelle haben, der Standardwert ist true. |
| static [SaveHtmlAsZip](../../aspose.cells.gridjs/config/savehtmlaszip/) { get; set; } | Liest/Setzt, ob HTML-Dateien als ZIP-Archiv gespeichert werden, der Standardwert ist false. |
| static [ShowChartSheet](../../aspose.cells.gridjs/config/showchartsheet/) { get; set; } | Liest/Setzt, ob das Diagramm-Arbeitsblatt angezeigt wird. Der Standardwert ist false. |
| static [SkipInvisibleShapes](../../aspose.cells.gridjs/config/skipinvisibleshapes/) { get; set; } | Liest/Setzt, ob Formen übersprungen werden sollen, die für die UI unsichtbar sind, der Standardwert ist true. |
| static [UsePrintArea](../../aspose.cells.gridjs/config/useprintarea/) { get; set; } | Liest/Setzt, ob PageSetup.PrintArea für den UI-Anzeigebereich verwendet wird, wenn das Arbeitsblatt eine PageSetup-Einstellung für PrintArea hat. Der Standardwert ist false. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [SetFontFolder](../../aspose.cells.gridjs/config/setfontfolder/)(string, bool) | Legt den Schriftartenordner fest |
| static [SetFontFolders](../../aspose.cells.gridjs/config/setfontfolders/)(string[], bool) | Setzt die Schriftordner. |

## Felder

| Name | Beschreibung |
| --- | --- |
| static [RedactionUseClientGenerateId](../../aspose.cells.gridjs/config/redactionuseclientgenerateid/) | Gibt an, ob bei redaktionsbezogenen Vorgängen die vom Client generierte ID anstelle der tatsächlichen Shape-ID verwendet wird. |

### Siehe auch

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


