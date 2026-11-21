---
title: "IFilePathProvider"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar leverantören av den exporterade filsökvägen."
type: docs
url: /sv/java/com.aspose.cells/ifilepathprovider/
---
```
public interface IFilePathProvider
```

Representerar leverantören av den exporterade filsökvägen.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getFullName(String sheetName)](#getFullName-java.lang.String-) | Hämtar den fullständiga sökvägen för filen efter kalkylbladets namn när kalkylbladet exporteras till HTML separat. |
### getFullName(String sheetName) {#getFullName-java.lang.String-}
```
public abstract String getFullName(String sheetName)
```


Hämtar den fullständiga sökvägen för filen efter kalkylbladets namn när kalkylbladet exporteras till HTML separat. Så att referenserna mellan kalkylbladen kan exporteras korrekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetName | java.lang.String | Kalkylbladsnamn |

**Returns:**
java.lang.String – den fullständiga sökvägen för filen
