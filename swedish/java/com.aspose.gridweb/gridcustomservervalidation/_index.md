---
title: "GridCustomServerValidation"
second_title: "Aspose.Cells för Java API-referens"
description: "gränssnittet du behöver implementera när du använder servervalidering."
type: docs
url: /sv/java/com.aspose.gridweb/gridcustomservervalidation/
---
```
public interface GridCustomServerValidation
```

gränssnittet du behöver implementera när du använder server-sidovalidering. CustomServerFunction.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [validate(GridWorksheet sheet, int row, int col, String value)](#validate-com.aspose.gridweb.GridWorksheet-int-int-java.lang.String-) | **Anmärkningar** |
### validate(GridWorksheet sheet, int row, int col, String value) {#validate-com.aspose.gridweb.GridWorksheet-int-int-java.lang.String-}
```
public abstract String validate(GridWorksheet sheet, int row, int col, String value)
```


**Remarks**

om du returnerar string.empty så anses valideringen godkänd, annars kan du returnera ett relaterat meddelande som kan hanteras i ClientCallback-funktionen

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheet | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) | GridWorksheet |
| rad | int | radindex för cellen |
| kol | int | kolumnindex för cellen |
| värde | java.lang.String | värdet för validering |

**Returns:**
java.lang.String - strängbaserat resultatvärde
