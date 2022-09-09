---
title: BorderLineColor
second_title: Aspose.Cells für .NET-API-Referenz
description: steht für dieColor der Randlinie eines Bildes.
type: docs
weight: 10
url: /de/net/aspose.cells.drawing/picture/borderlinecolor/
---
## Picture.BorderLineColor property

steht für dieColor der Randlinie eines Bildes.

```csharp
public Color BorderLineColor { get; set; }
```

### Beispiele

```csharp

[C#]
//Instanziieren eines Workbook-Objekts
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
//Hinzufügen eines Bildes an der Position einer Zelle, deren Zeilen- und Spaltenindizes 1 im Arbeitsblatt sind. Es ist eine "B2"-Zelle
int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
//Das eingefügte Bildobjekt abrufen
Picture pic = worksheet.Pictures[imgIndex];
// Legen Sie die Rahmenfarbe des Bildes fest
pic.BorderLineColor = Color.Red;
//Speichern Sie die Excel-Datei.
workbook.Save("result.xlsx");
```

### Siehe auch

* class [Picture](../../picture)
* namensraum [Aspose.Cells.Drawing](../../picture)
* Montage [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->