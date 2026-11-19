---
title: "ICellsDataTable"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente la table de données."
type: docs
url: /fr/java/com.aspose.cells/icellsdatatable/
---
```
public interface ICellsDataTable
```

Représente la table de données.

**Remarks**
## Méthodes

| Méthode | Description |
| --- | --- |
| [beforeFirst()](#beforeFirst--) | Déplacez le curseur au début de cet objet, juste avant la première ligne. |
| [get(int columnIndex)](#get-int-) | Récupère les données stockées dans la colonne spécifiée par l'index. |
| [get(String columnName)](#get-java.lang.String-) | Récupère les données stockées dans la colonne spécifiée par le nom de la colonne. |
| [getColumns()](#getColumns--) | Récupère le nom des colonnes. |
| [getCount()](#getCount--) | Récupère le nombre d'enregistrements. -1 pour un nombre d'enregistrements inconnu. |
| [next()](#next--) | Déplace le curseur d'une ligne vers le bas depuis sa position actuelle. |
### beforeFirst() {#beforeFirst--}
```
public abstract void beforeFirst()
```


Déplacez le curseur au début de cet objet, juste avant la première ligne.

### get(int columnIndex) {#get-int-}
```
public abstract Object get(int columnIndex)
```


Récupère les données stockées dans la colonne spécifiée par l'index.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | int | L'index de la colonne, basé sur zéro. |

**Returns:**
java.lang.Object -
### get(String columnName) {#get-java.lang.String-}
```
public abstract Object get(String columnName)
```


Récupère les données stockées dans la colonne spécifiée par le nom de la colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnName | java.lang.String | Le nom de la colonne. |

**Returns:**
java.lang.Object -
### getColumns() {#getColumns--}
```
public abstract String[] getColumns()
```


Récupère le nom des colonnes.

**Returns:**
java.lang.String[]
### getCount() {#getCount--}
```
public abstract int getCount()
```


Récupère le nombre d'enregistrements. -1 pour un nombre d'enregistrements inconnu.

**Returns:**
int
### next() {#next--}
```
public abstract boolean next()
```


Déplace le curseur d'une ligne vers le bas depuis sa position actuelle.

**Returns:**
booléen - si la nouvelle ligne courante est valide ; false s'il n'y a plus de lignes
