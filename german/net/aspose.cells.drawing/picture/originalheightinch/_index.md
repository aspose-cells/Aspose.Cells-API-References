---
title: OriginalHeightInch
second_title: Aspose.Cells für .NET-API-Referenz
description: Ruft die Originalhöhe des Bildes in Zoll ab.
type: docs
weight: 120
url: /de/net/aspose.cells.drawing/picture/originalheightinch/
---
## Picture.OriginalHeightInch property

Ruft die Originalhöhe des Bildes in Zoll ab.

```csharp
public double OriginalHeightInch { get; }
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
// Ruft die ursprüngliche Höhe des Bildes ab.
double picHeightInch = pic.OriginalHeightInch;
//Speichern Sie die Excel-Datei.
workbook.Save("result.xlsx");
```

### Siehe auch

* class [Picture](../../picture)
* namensraum [Aspose.Cells.Drawing](../../picture)
* Montage [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->