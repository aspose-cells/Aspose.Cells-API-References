---
title: "Klasse GridJsService"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridJs.GridJsService Klasse. Stellt die grundlegenden API‑Operationen bereit, die in Controller‑Aktionen verwendet werden"
type: docs
url: /de/net/aspose.cells.gridjs/gridjsservice/
---
## GridJsService class

Stellt die grundlegenden Betriebs‑APIs bereit, die in Controller‑Aktionen verwendet werden.

```csharp
public class GridJsService : IGridJsService
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [GridJsService](gridjsservice/#constructor)(GridJsOptions) | Der Konstruktor für GridJsService für Hosts, die das Optionsobjekt selbst erstellen (der Browser‑WASM‑Host und jede nicht‑DI‑Serverkonfiguration). |
| [GridJsService](gridjsservice/#constructor_1)(IOptions&lt;GridJsOptions&gt;) | Der Standardkonstruktor für GridJsService |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Settings](../../aspose.cells.gridjs/gridjsservice/settings/) { get; set; } | Stellt die Einstellungen der Arbeitsmappe dar. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddImage](../../aspose.cells.gridjs/gridjsservice/addimage/#addimage)(string, string, string, byte[]) | Wendet die Operation zum Hinzufügen eines Bildes aus einer lokalen Datei an (Dateibytes stammen aus JS FormData oder einem beliebigen Host). |
| [AddImage](../../aspose.cells.gridjs/gridjsservice/addimage/#addimage_1)(string, string, string, IFormFileCollection) | Wendet die Operation zum Hinzufügen eines Bildes aus einer lokalen Datei an. |
| [AddImageByURL](../../aspose.cells.gridjs/gridjsservice/addimagebyurl/)(string, string, string) | Wendet die Operation zum Hinzufügen eines Bildes von einer entfernten URL an. |
| [CheckInCacheForCollaborative](../../aspose.cells.gridjs/gridjsservice/checkincacheforcollaborative/)(string) | Prüft, ob die Arbeitsmappeninstanz im Speicher-Cache ist. Diese Methode wird nur im kollaborativen Modus angewendet. |
| [ClearAllJsonCache](../../aspose.cells.gridjs/gridjsservice/clearalljsoncache/)() | Löscht alle JSON-Cache-Einträge (Speicher und Festplatte). |
| [ClearJsonCacheForUid](../../aspose.cells.gridjs/gridjsservice/clearjsoncacheforuid/)(string) | Löscht alle JSON-Cache-Einträge, die zur angegebenen eindeutigen ID gehören. Rufen Sie dies auf, nachdem die Quelldatei außerhalb des normalen Ablaufs geändert wurde, damit die nächste Anforderung das JSON neu generiert. |
| [CopyImage](../../aspose.cells.gridjs/gridjsservice/copyimage/)(string, string) | Wendet die Kopier‑Bild‑Operation an. |
| [Destroy](../../aspose.cells.gridjs/gridjsservice/destroy/)() | Diese Methode ist nur für Java, sie implementiert die destroy‑Methode in DisposableBean, die von Spring automatisch aufgerufen wird, wenn die Anforderung abgeschlossen ist; tatsächlich ruft sie die Dispose‑Methode auf. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid_1)(string, string) | Liefert den JSON‑String für die Datei anhand der angegebenen eindeutigen ID. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid)(Workbook, string, string) | Liefert den JSON‑String für die Arbeitsmappe anhand der angegebenen eindeutigen ID. |
| [DetailStreamJson](../../aspose.cells.gridjs/gridjsservice/detailstreamjson/#detailstreamjson_1)(Stream, string) | Schreibt den JSON‑String für die Datei in den Stream. |
| [DetailStreamJson](../../aspose.cells.gridjs/gridjsservice/detailstreamjson/#detailstreamjson)(Stream, Workbook, string) | Schreibt den JSON‑String für die Arbeitsmappe in den Stream |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid_1)(Stream, string, string) | Schreibt den JSON‑String für die Datei in den Stream anhand der angegebenen eindeutigen ID. |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid)(Stream, Workbook, string, string) | Schreibt den JSON‑String für die Arbeitsmappe in den Stream anhand der angegebenen eindeutigen ID. |
| [Dispose](../../aspose.cells.gridjs/gridjsservice/dispose/)() | Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
| [Download](../../aspose.cells.gridjs/gridjsservice/download/)(string, string, string) | Wendet die Download‑Datei‑Operation an |
| [GetFile](../../aspose.cells.gridjs/gridjsservice/getfile/)(string) | Datei‑Stream abrufen |
| [GetWarningCallback](../../aspose.cells.gridjs/gridjsservice/getwarningcallback/)() | Ruft den benutzerdefinierten Warn‑Callback für das Importieren von Dateien ab. |
| [Image](../../aspose.cells.gridjs/gridjsservice/image/)(string, string) | Bild‑Stream abrufen. |
| [ImageUrl](../../aspose.cells.gridjs/gridjsservice/imageurl/)(string, string, string) | Liefert die Bild‑URL. |
| [LazyLoadingJson](../../aspose.cells.gridjs/gridjsservice/lazyloadingjson/)(string, string) | Liefert den JSON‑String des angegebenen Arbeitsblatts in der Datei aus dem Cache anhand der angegebenen eindeutigen ID. |
| [LazyLoadingStreamJson](../../aspose.cells.gridjs/gridjsservice/lazyloadingstreamjson/)(Stream, string, string) | Schreibt den JSON‑String des angegebenen Arbeitsblatts in der Datei aus dem Cache anhand der angegebenen eindeutigen ID in den Stream. |
| [Load](../../aspose.cells.gridjs/gridjsservice/load/)(string, string) | Liefert den JSON‑String der Datei aus dem Cache anhand der angegebenen eindeutigen ID, setzt den Ausgabedateinamen im JSON. |
| [Ole](../../aspose.cells.gridjs/gridjsservice/ole/)(string, string, int, out string) | Liefert die Byte‑Array‑Daten des eingebetteten OLE‑Objekts. |
| [SetWarningCallback](../../aspose.cells.gridjs/gridjsservice/setwarningcallback/)(IWarningCallback) | Setzt den benutzerdefinierten Warn‑Callback für das Importieren von Dateien. |
| [TranslateSheetAsync](../../aspose.cells.gridjs/gridjsservice/translatesheetasync/)(string, string, ITextTranslator, string) | Übersetze alle Zeichenkettenwerte in die Zielsprache im Arbeitsblatt |
| [UpdateCell](../../aspose.cells.gridjs/gridjsservice/updatecell/)(string, string) | Wendet die Aktualisierungsoperation an. |

### Siehe auch

* interface [IGridJsService](../igridjsservice/)
* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


