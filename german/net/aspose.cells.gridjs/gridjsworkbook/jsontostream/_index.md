---
title: "GridJsWorkbook.JsonToStream"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridJsWorkbook‑Methode. Erzeugt JSON aus dem im Speicher befindlichen Workbook und schreibt es in den angegebenen Stream. Optional wird das erzeugte JSON zwischengespeichert, um spätere Abrufe zu beschleunigen. Wichtige Unterschiede zu JsonToStreamByUid: Diese Methode verwendet den aktuellen im Speicher befindlichen Workbook‑Zustand (wb‑Feld). JsonToStreamByUid lädt das Workbook aus .cells‑Cache‑Dateien auf der Festplatte neu. Verwenden Sie diese Methode, wenn Sie den aktuellen Workbook‑Zustand nach Änderungen exportieren möchten. Verwenden Sie JsonToStreamByUid, wenn Sie JSON aus einem zuvor zwischengespeicherten Dateizustand neu generieren müssen. Caching‑Verhalten, wenn eine uid angegeben ist: Prüft den JSON‑Cache, bevor JSON im L1‑Speicher (Arbeitsspeicher) bzw. L2‑Disk (Festplatte) erzeugt wird. Bei einem Cache‑Fehltritt wird JSON aus dem im Speicher befindlichen Workbook erzeugt. Das erzeugte JSON wird für zukünftige Anfragen im Cache gespeichert."
type: docs
url: /de/net/aspose.cells.gridjs/gridjsworkbook/jsontostream/
---
## GridJsWorkbook.JsonToStream method

Erstellt JSON aus der im Speicher befindlichen Arbeitsmappe und schreibt es in den angegebenen Stream. Optional wird das erzeugte JSON zwischengespeichert, um spätere Abrufe zu beschleunigen. Wesentliche Unterschiede zu JsonToStreamByUid: - Diese Methode verwendet den aktuellen im Speicher befindlichen Arbeitsmappenstatus (wb-Feld) - JsonToStreamByUid lädt die Arbeitsmappe aus .cells-Cache-Dateien auf der Festplatte neu - Verwenden Sie diese Methode, wenn Sie den aktuellen Arbeitsmappenstatus nach Änderungen exportieren möchten - Verwenden Sie JsonToStreamByUid, wenn Sie JSON aus einem zuvor zwischengespeicherten Dateistatus neu generieren müssen. Caching‑Verhalten (wenn uid angegeben ist): - Prüft den JSON-Cache vor der Erzeugung (L1 Speicher + L2 Festplatte) - Bei einem Cache‑Fehltreffer wird JSON aus der im Speicher befindlichen Arbeitsmappe erzeugt - Speichert das erzeugte JSON im Cache für zukünftige Anfragen.

```csharp
public void JsonToStream(Stream stream, string filename, string uid = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | Stream | Der Ausgabestream, in den JSON‑Daten geschrieben werden sollen |
| Dateiname | String | Gibt den Dateinamen im JSON an. Wenn auf null gesetzt, ist der Standarddateiname: book1. |
| uid | String | Optionaler eindeutiger Bezeichner für das JSON‑Caching. Wenn angegeben, ermöglicht er das Nachschlagen und Speichern im Cache. |

### Siehe auch

* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


