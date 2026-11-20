---
title: "GridCustomServerValidation"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Die Schnittstelle, die Sie implementieren müssen, wenn Sie serverseitige Validierung verwenden."
type: docs
url: /de/java/com.aspose.gridweb/gridcustomservervalidation/
---
```
public interface GridCustomServerValidation
```

die Schnittstelle, die Sie implementieren müssen, wenn Sie serverseitige Validierung verwenden. CustomServerFunction.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [validate(GridWorksheet sheet, int row, int col, String value)](#validate-com.aspose.gridweb.GridWorksheet-int-int-java.lang.String-) | **Hinweise** |
### validate(GridWorksheet sheet, int row, int col, String value) {#validate-com.aspose.gridweb.GridWorksheet-int-int-java.lang.String-}
```
public abstract String validate(GridWorksheet sheet, int row, int col, String value)
```


**Remarks**

wenn string.empty zurückgegeben wird, ist die Validierung bestanden, andernfalls können Sie eine beliebige zugehörige Meldung zurückgeben, die in der ClientCallback‑Funktion verarbeitet werden kann

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheet | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) | das GridWorksheet |
| Zeile | int | der Zeilenindex der Zelle |
| Spalte | int | der Spaltenindex der Zelle |
| Wert | java.lang.String | der Wert für die Validierung |

**Returns:**
java.lang.String – stringbasierter Ergebniswert
