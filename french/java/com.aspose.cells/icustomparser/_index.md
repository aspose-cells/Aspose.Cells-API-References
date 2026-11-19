---
title: "ICustomParser"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Permet aux utilisateurs d'ajouter leur analyseur de valeurs personnalisé pour analyser les valeurs de chaîne en d'autres objets de valeur de cellule appropriés."
type: docs
url: /fr/java/com.aspose.cells/icustomparser/
---
```
public interface ICustomParser
```

Permet aux utilisateurs d'ajouter leur analyseur de valeurs personnalisé pour analyser les valeurs de chaîne en d'autres objets de valeur de cellule appropriés.
## Méthodes

| Méthode | Description |
| --- | --- |
| [getFormat()](#getFormat--) | Obtient le modèle de formatage correspondant à la valeur analysée lors de la dernière invocation de [parseObject(String)](../../com.aspose.cells/icustomparser\#parseObject-String-). |
| [parseObject(String value)](#parseObject-java.lang.String-) | Analyse la chaîne donnée pour obtenir l'objet valeur approprié. |
### getFormat() {#getFormat--}
```
public abstract String getFormat()
```


Obtient le modèle de formatage correspondant à la valeur analysée lors de la dernière invocation de [parseObject(String)](../../com.aspose.cells/icustomparser\#parseObject-String-).

**Remarks**

Le modèle de formatage retourné peut être utilisé pour formater la cellule correspondante (définissez Style.Custom pour la cellule).

**Returns:**
java.lang.String
### parseObject(String value) {#parseObject-java.lang.String-}
```
public abstract Object parseObject(String value)
```


Analyse la chaîne donnée pour obtenir l'objet valeur approprié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | La valeur chaîne à analyser |

**Returns:**
java.lang.Object - Objet valeur analysé à partir de la chaîne donnée. Si la chaîne donnée ne peut pas être analysée en un objet valeur approprié, renvoie null.
