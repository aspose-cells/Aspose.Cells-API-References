---
title: "ICustomParser"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Ermöglicht Benutzern, ihren eigenen Wertparser hinzuzufügen, um Zeichenkettenwerte in andere geeignete Zellwertobjekte zu parsen."
type: docs
url: /de/java/com.aspose.cells/icustomparser/
---
```
public interface ICustomParser
```

Ermöglicht Benutzern, ihren eigenen Wertparser hinzuzufügen, um Zeichenkettenwerte in andere geeignete Zellwertobjekte zu parsen.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getFormat()](#getFormat--) | Liest das Formatierungsmuster, das dem zuletzt aufgerufenen [parseObject(String)](../../com.aspose.cells/icustomparser\#parseObject-String-) entspricht. |
| [parseObject(String value)](#parseObject-java.lang.String-) | Parst die angegebene Zeichenkette in ein geeignetes Wertobjekt. |
### getFormat() {#getFormat--}
```
public abstract String getFormat()
```


Liest das Formatierungsmuster, das dem zuletzt aufgerufenen [parseObject(String)](../../com.aspose.cells/icustomparser\#parseObject-String-) entspricht.

**Remarks**

Das zurückgegebene Formatierungsmuster kann verwendet werden, um die entsprechende Zelle zu formatieren (auf Style.Custom für die Zelle setzen).

**Returns:**
java.lang.String
### parseObject(String value) {#parseObject-java.lang.String-}
```
public abstract Object parseObject(String value)
```


Parst die angegebene Zeichenkette in ein geeignetes Wertobjekt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | Der zu parsende Zeichenkettenwert |

**Returns:**
java.lang.Object – Geparstes Wertobjekt aus der angegebenen Zeichenkette. Wenn die Zeichenkette nicht in ein geeignetes Wertobjekt geparst werden kann, wird null zurückgegeben.
