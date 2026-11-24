---
title: "Schnittstelle IGridJsService"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridJs.IGridJsService Schnittstelle. Stellt die grundlegende Operations‑API‑Schnittstelle dar, die in Controller‑Aktionen verwendet wird."
type: docs
url: /de/net/aspose.cells.gridjs/igridjsservice/
---
## IGridJsService interface

Stellt die grundlegende Betriebs‑APIs‑Schnittstelle bereit, die in Controller‑Aktionen verwendet wird.

```csharp
public interface IGridJsService : IDisposable
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddImage](../../aspose.cells.gridjs/igridjsservice/addimage/#addimage)(string, string, string, byte[]) | Wendet die Operation zum Hinzufügen eines Bildes aus einer lokalen Datei an und verwendet die Bildbytes direkt. |
| [AddImage](../../aspose.cells.gridjs/igridjsservice/addimage/#addimage_1)(string, string, string, IFormFileCollection) | Wendet die Operation zum Hinzufügen eines Bildes aus einer lokalen Datei an und verwendet die hochgeladenen Formulardateien. |
| [AddImageByURL](../../aspose.cells.gridjs/igridjsservice/addimagebyurl/)(string, string, string) | Wendet die Operation zum Hinzufügen eines Bildes von einer entfernten URL an. |
| [CheckInCacheForCollaborative](../../aspose.cells.gridjs/igridjsservice/checkincacheforcollaborative/)(string) | Prüft, ob die Arbeitsmappeninstanz im Speicher-Cache ist. Diese Methode wird nur im kollaborativen Modus angewendet. |
| [ClearAllJsonCache](../../aspose.cells.gridjs/igridjsservice/clearalljsoncache/)() | Löscht alle JSON-Cache-Einträge (Speicher und Festplatte). |
| [ClearJsonCacheForUid](../../aspose.cells.gridjs/igridjsservice/clearjsoncacheforuid/)(string) | Löscht alle JSON-Cache-Einträge, die zur angegebenen eindeutigen ID gehören. Rufen Sie dies auf, nachdem die Quelldatei außerhalb des normalen Ablaufs geändert wurde, damit die nächste Anforderung das JSON neu generiert. |
| [CopyImage](../../aspose.cells.gridjs/igridjsservice/copyimage/)(string, string) | Wendet die Kopier‑Bild‑Operation an. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid_1)(string, string) | Liefert den JSON‑String für die Datei anhand der angegebenen eindeutigen ID. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid)(Workbook, string, string) | Liefert den JSON‑String für die Arbeitsmappe anhand der angegebenen eindeutigen ID. |
| [DetailStreamJson](../../aspose.cells.gridjs/igridjsservice/detailstreamjson/#detailstreamjson_1)(Stream, string) | Schreibt den JSON‑String für die Arbeitsmappe in den Stream |
| [DetailStreamJson](../../aspose.cells.gridjs/igridjsservice/detailstreamjson/#detailstreamjson)(Stream, Workbook, string) | Schreibt den JSON‑String für die Arbeitsmappe in den Stream |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid_1)(Stream, string, string) | Schreibt den JSON‑String für die Datei in den Stream anhand der angegebenen eindeutigen ID. |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid)(Stream, Workbook, string, string) | Schreibt den JSON‑String für die Arbeitsmappe in den Stream anhand der angegebenen eindeutigen ID. |
| [Download](../../aspose.cells.gridjs/igridjsservice/download/)(string, string, string) | Wendet die Download‑Datei‑Operation an |
| [GetFile](../../aspose.cells.gridjs/igridjsservice/getfile/)(string) | Datei‑Stream abrufen |
| [GetWarningCallback](../../aspose.cells.gridjs/igridjsservice/getwarningcallback/)() | Ruft den benutzerdefinierten Warn‑Callback für das Importieren von Dateien ab. |
| [Image](../../aspose.cells.gridjs/igridjsservice/image/)(string, string) | Bild‑Stream abrufen. |
| [ImageUrl](../../aspose.cells.gridjs/igridjsservice/imageurl/)(string, string, string) | Liefert die Bild‑URL. |
| [LazyLoadingJson](../../aspose.cells.gridjs/igridjsservice/lazyloadingjson/)(string, string) | Liefert den JSON‑String des angegebenen Arbeitsblatts in der Datei aus dem Cache anhand der angegebenen eindeutigen ID. |
| [LazyLoadingStreamJson](../../aspose.cells.gridjs/igridjsservice/lazyloadingstreamjson/)(Stream, string, string) | Schreibt den JSON‑String des angegebenen Arbeitsblatts in der Datei aus dem Cache anhand der angegebenen eindeutigen ID in den Stream. |
| [Load](../../aspose.cells.gridjs/igridjsservice/load/)(string, string) | Liefert den JSON‑String der Datei aus dem Cache anhand der angegebenen eindeutigen ID, setzt den Ausgabedateinamen im JSON. |
| [Ole](../../aspose.cells.gridjs/igridjsservice/ole/)(string, string, int, out string) | Liefert die Byte‑Array‑Daten des eingebetteten OLE‑Objekts. |
| [SetWarningCallback](../../aspose.cells.gridjs/igridjsservice/setwarningcallback/)(IWarningCallback) | Setzt den benutzerdefinierten Warn‑Callback für das Importieren von Dateien. |
| [UpdateCell](../../aspose.cells.gridjs/igridjsservice/updatecell/)(string, string) | Wendet die Aktualisierungsoperation an. |

### Siehe auch

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


