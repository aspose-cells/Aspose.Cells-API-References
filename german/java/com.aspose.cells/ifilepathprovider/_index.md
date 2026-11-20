---
title: "IFilePathProvider"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt den Anbieter für den exportierten Dateipfad dar."
type: docs
url: /de/java/com.aspose.cells/ifilepathprovider/
---
```
public interface IFilePathProvider
```

Stellt den Anbieter für den exportierten Dateipfad dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getFullName(String sheetName)](#getFullName-java.lang.String-) | Ermittelt den vollständigen Pfad der Datei anhand des Arbeitsblattnamens beim separaten Exportieren des Arbeitsblatts nach HTML. |
### getFullName(String sheetName) {#getFullName-java.lang.String-}
```
public abstract String getFullName(String sheetName)
```


Ermittelt den vollständigen Pfad der Datei anhand des Arbeitsblattnamens beim separaten Exportieren des Arbeitsblatts nach HTML, sodass die Verweise zwischen den Arbeitsblättern korrekt exportiert werden können.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetName | java.lang.String | Arbeitsblattname |

**Returns:**
java.lang.String – der vollständige Pfad der Datei
