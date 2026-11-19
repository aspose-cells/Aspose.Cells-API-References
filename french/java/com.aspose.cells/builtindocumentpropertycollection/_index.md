---
title: "BuiltInDocumentPropertyCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Une collection de propriétés de document intégrées."
type: docs
url: /fr/java/com.aspose.cells/builtindocumentpropertycollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase), [com.aspose.cells.DocumentPropertyCollection](../../com.aspose.cells/documentpropertycollection)
```
public class BuiltInDocumentPropertyCollection extends DocumentPropertyCollection
```

Une collection de propriétés de document intégrées.

**Remarks**

Fournit un accès aux objets par leurs noms (en utilisant un indexeur) et via un ensemble de propriétés typées qui renvoient des valeurs des types appropriés.
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Ajoute un élément à l'instance CollectionBase. |
| [clear()](#clear--) | Supprime tous les objets de l'instance CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Renvoie si l'instance contient cet objet |
| [contains(String name)](#contains-java.lang.String-) | Renvoie true si une propriété portant le nom spécifié existe dans la collection. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Renvoie un objet [DocumentProperty](../../com.aspose.cells/documentproperty) par indice. |
| [get(String name)](#get-java.lang.String-) | Renvoie un objet [DocumentProperty](../../com.aspose.cells/documentproperty) par le nom de la propriété. |
| [getAuthor()](#getAuthor--) | Obtient le nom de l'auteur du document. |
| [getBytes()](#getBytes--) | Représente une estimation du nombre d'octets dans le document. |
| [getCategory()](#getCategory--) | Obtient la catégorie du document. |
| [getCharacters()](#getCharacters--) | Représente une estimation du nombre de caractères dans le document. |
| [getCharactersWithSpaces()](#getCharactersWithSpaces--) | Représente une estimation du nombre de caractères (espaces inclus) dans le document. |
| [getClass()](#getClass--) |  |
| [getComments()](#getComments--) | Obtient les commentaires du document. |
| [getCompany()](#getCompany--) | Obtient la propriété de l'entreprise. |
| [getContentStatus()](#getContentStatus--) | Obtient le statut du contenu du document. |
| [getContentType()](#getContentType--) | Obtient le type de contenu du document. |
| [getCount()](#getCount--) | Obtient le nombre d'éléments contenus dans l'instance CollectionBase. |
| [getCreatedTime()](#getCreatedTime--) | Obtient la date de création du document dans le fuseau horaire local. |
| [getCreatedUniversalTime()](#getCreatedUniversalTime--) | Obtient l'heure universelle de la création du document. |
| [getDocumentVersion()](#getDocumentVersion--) | Représente la version du fichier. |
| [getHyperlinkBase()](#getHyperlinkBase--) | Obtient la propriété hyperlinkbase. |
| [getKeywords()](#getKeywords--) | Obtient les mots-clés du document. |
| [getLanguage()](#getLanguage--) | Obtient la langue du document. |
| [getLastPrinted()](#getLastPrinted--) | Obtient la date à laquelle le document a été imprimé pour la dernière fois dans le fuseau horaire local. |
| [getLastPrintedUniversalTime()](#getLastPrintedUniversalTime--) | Obtient l'heure universelle à laquelle le document a été imprimé pour la dernière fois. |
| [getLastSavedBy()](#getLastSavedBy--) | Obtient le nom du dernier auteur. |
| [getLastSavedTime()](#getLastSavedTime--) | Obtient l'heure de la dernière sauvegarde dans le fuseau horaire local. |
| [getLastSavedUniversalTime()](#getLastSavedUniversalTime--) | Obtient l'heure universelle de la dernière sauvegarde. |
| [getLines()](#getLines--) | Représente une estimation du nombre de lignes dans le document. |
| [getLinksUpToDate()](#getLinksUpToDate--) | Indique si les hyperliens dans un document sont à jour. |
| [getManager()](#getManager--) | Obtient la propriété manager. |
| [getNameOfApplication()](#getNameOfApplication--) | Obtient le nom de l'application. |
| [getPages()](#getPages--) | Représente une estimation du nombre de pages dans le document. |
| [getParagraphs()](#getParagraphs--) | Représente une estimation du nombre de paragraphes dans le document. |
| [getRevisionNumber()](#getRevisionNumber--) | Obtient le numéro de révision du document. |
| [getScaleCrop()](#getScaleCrop--) | Indique le mode d'affichage de la vignette du document. |
| [getSubject()](#getSubject--) | Obtient le sujet du document. |
| [getTemplate()](#getTemplate--) | Obtient le nom informatif du modèle de document. |
| [getTitle()](#getTitle--) | Obtient le titre du document. |
| [getTotalEditingTime()](#getTotalEditingTime--) | Obtient le temps total d'édition en minutes. |
| [getVersion()](#getVersion--) | Représente le numéro de version de l'application qui a créé le document. |
| [getWords()](#getWords--) | Représente une estimation du nombre de mots dans le document. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Détermine l'index d'un élément spécifique dans l'instance CollectionBase. |
| [indexOf(String name)](#indexOf-java.lang.String-) | Obtient l'indice d'une propriété par son nom. |
| [iterator()](#iterator--) | Renvoie un énumérateur qui parcourt l'instance CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String name)](#remove-java.lang.String-) | Supprime une propriété portant le nom spécifié de la collection. |
| [removeAt(int index)](#removeAt-int-) | Supprime une propriété à l'indice spécifié. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Définit le nom de l'auteur du document. |
| [setBytes(int value)](#setBytes-int-) | Représente une estimation du nombre d'octets dans le document. |
| [setCategory(String value)](#setCategory-java.lang.String-) | Définit la catégorie du document. |
| [setCharacters(int value)](#setCharacters-int-) | Représente une estimation du nombre de caractères dans le document. |
| [setCharactersWithSpaces(int value)](#setCharactersWithSpaces-int-) | Représente une estimation du nombre de caractères (espaces inclus) dans le document. |
| [setComments(String value)](#setComments-java.lang.String-) | Définit les commentaires du document. |
| [setCompany(String value)](#setCompany-java.lang.String-) | Définit la propriété company. |
| [setContentStatus(String value)](#setContentStatus-java.lang.String-) | Définit l'état du contenu du document. |
| [setContentType(String value)](#setContentType-java.lang.String-) | Définit le type de contenu du document. |
| [setCreatedTime(DateTime value)](#setCreatedTime-com.aspose.cells.DateTime-) | Définit la date de création du document dans le fuseau horaire local. |
| [setCreatedUniversalTime(DateTime value)](#setCreatedUniversalTime-com.aspose.cells.DateTime-) | Définit l'heure universelle de création du document. |
| [setDocumentVersion(String value)](#setDocumentVersion-java.lang.String-) | Représente la version du fichier. |
| [setHyperlinkBase(String value)](#setHyperlinkBase-java.lang.String-) | Définit la propriété hyperlinkbase. |
| [setKeywords(String value)](#setKeywords-java.lang.String-) | Définit les mots-clés du document. |
| [setLanguage(String value)](#setLanguage-java.lang.String-) | Définit la langue du document. |
| [setLastPrinted(DateTime value)](#setLastPrinted-com.aspose.cells.DateTime-) | Définit la date à laquelle le document a été imprimé pour la dernière fois dans le fuseau horaire local. |
| [setLastPrintedUniversalTime(DateTime value)](#setLastPrintedUniversalTime-com.aspose.cells.DateTime-) | Définit l'heure universelle à laquelle le document a été imprimé pour la dernière fois. |
| [setLastSavedBy(String value)](#setLastSavedBy-java.lang.String-) | Définit le nom du dernier auteur. |
| [setLastSavedTime(DateTime value)](#setLastSavedTime-com.aspose.cells.DateTime-) | Définit l'heure de la dernière sauvegarde dans le fuseau horaire local. |
| [setLastSavedUniversalTime(DateTime value)](#setLastSavedUniversalTime-com.aspose.cells.DateTime-) | Définit l'heure universelle de la dernière sauvegarde. |
| [setLines(int value)](#setLines-int-) | Représente une estimation du nombre de lignes dans le document. |
| [setLinksUpToDate(boolean value)](#setLinksUpToDate-boolean-) | Indique si les hyperliens dans un document sont à jour. |
| [setManager(String value)](#setManager-java.lang.String-) | Définit la propriété manager. |
| [setNameOfApplication(String value)](#setNameOfApplication-java.lang.String-) | Définit le nom de l'application. |
| [setPages(int value)](#setPages-int-) | Représente une estimation du nombre de pages dans le document. |
| [setParagraphs(int value)](#setParagraphs-int-) | Représente une estimation du nombre de paragraphes dans le document. |
| [setRevisionNumber(String value)](#setRevisionNumber-java.lang.String-) | Définit le numéro de révision du document. |
| [setScaleCrop(boolean value)](#setScaleCrop-boolean-) | Indique le mode d'affichage de la vignette du document. |
| [setSubject(String value)](#setSubject-java.lang.String-) | Définit le sujet du document. |
| [setTemplate(String value)](#setTemplate-java.lang.String-) | Définit le nom informatif du modèle de document. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Définit le titre du document. |
| [setTotalEditingTime(double value)](#setTotalEditingTime-double-) | Définit le temps total d'édition en minutes. |
| [setVersion(String value)](#setVersion-java.lang.String-) | Représente le numéro de version de l'application qui a créé le document. |
| [setWords(int value)](#setWords-int-) | Représente une estimation du nombre de mots dans le document. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Ajoute un élément à l'instance CollectionBase.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | L'objet à ajouter à l'instance CollectionBase. |

**Returns:**
int - La position dans laquelle le nouvel élément a été inséré.
### clear() {#clear--}
```
public void clear()
```


Supprime tous les objets de l'instance CollectionBase.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Renvoie si l'instance contient cet objet

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | objet de test |

**Returns:**
boolean - Si l'instance contient cet objet
### contains(String name) {#contains-java.lang.String-}
```
public boolean contains(String name)
```


Renvoie true si une propriété portant le nom spécifié existe dans la collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de la propriété, insensible à la casse. |

**Returns:**
boolean - True si la propriété existe dans la collection ; false sinon.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int index) {#get-int-}
```
public DocumentProperty get(int index)
```


Renvoie un objet [DocumentProperty](../../com.aspose.cells/documentproperty) par indice.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | Indice basé sur zéro du [DocumentProperty](../../com.aspose.cells/documentproperty) à récupérer. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
### get(String name) {#get-java.lang.String-}
```
public DocumentProperty get(String name)
```


Renvoie un objet [DocumentProperty](../../com.aspose.cells/documentproperty) par le nom de la propriété.

**Remarks**

Les noms de chaîne des propriétés correspondent aux noms des propriétés typées disponibles depuis .

Si vous demandez une propriété qui n'est pas présente dans le document, mais que le nom de la propriété est reconnu comme un nom intégré valide, une nouvelle  est créée, ajoutée à la collection et renvoyée. La propriété nouvellement créée reçoit une valeur par défaut (chaîne vide, zéro, false ou DateTime.MinValue selon le type de la propriété intégrée).

Si vous demandez une propriété qui n'est pas présente dans le document et que le nom n'est pas reconnu comme un nom intégré, null est renvoyé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de la propriété, insensible à la casse, à récupérer. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Obtient le nom de l'auteur du document.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public int getBytes()
```


Représente une estimation du nombre d'octets dans le document.

**Returns:**
int
### getCategory() {#getCategory--}
```
public String getCategory()
```


Obtient la catégorie du document.

**Returns:**
java.lang.String
### getCharacters() {#getCharacters--}
```
public int getCharacters()
```


Représente une estimation du nombre de caractères dans le document.

**Returns:**
int
### getCharactersWithSpaces() {#getCharactersWithSpaces--}
```
public int getCharactersWithSpaces()
```


Représente une estimation du nombre de caractères (espaces inclus) dans le document.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getComments() {#getComments--}
```
public String getComments()
```


Obtient les commentaires du document.

**Returns:**
java.lang.String
### getCompany() {#getCompany--}
```
public String getCompany()
```


Obtient la propriété de l'entreprise.

**Returns:**
java.lang.String
### getContentStatus() {#getContentStatus--}
```
public String getContentStatus()
```


Obtient le statut du contenu du document.

**Returns:**
java.lang.String
### getContentType() {#getContentType--}
```
public String getContentType()
```


Obtient le type de contenu du document.

**Returns:**
java.lang.String
### getCount() {#getCount--}
```
public int getCount()
```


Obtient le nombre d'éléments contenus dans l'instance CollectionBase.

**Returns:**
int - Le nombre d'éléments contenus dans l'instance CollectionBase.
### getCreatedTime() {#getCreatedTime--}
```
public DateTime getCreatedTime()
```


Obtient la date de création du document dans le fuseau horaire local.

**Remarks**

Aspose.Cells ne met pas à jour cette propriété lorsque vous modifiez le document.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getCreatedUniversalTime() {#getCreatedUniversalTime--}
```
public DateTime getCreatedUniversalTime()
```


Obtient l'heure universelle de la création du document.

**Remarks**

Aspose.Cells ne met pas à jour cette propriété lorsque vous modifiez le document.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getDocumentVersion() {#getDocumentVersion--}
```
public String getDocumentVersion()
```


Représente la version du fichier.

**Returns:**
java.lang.String
### getHyperlinkBase() {#getHyperlinkBase--}
```
public String getHyperlinkBase()
```


Obtient la propriété hyperlinkbase.

**Returns:**
java.lang.String
### getKeywords() {#getKeywords--}
```
public String getKeywords()
```


Obtient les mots-clés du document.

**Returns:**
java.lang.String
### getLanguage() {#getLanguage--}
```
public String getLanguage()
```


Obtient la langue du document.

**Returns:**
java.lang.String
### getLastPrinted() {#getLastPrinted--}
```
public DateTime getLastPrinted()
```


Obtient la date à laquelle le document a été imprimé pour la dernière fois dans le fuseau horaire local.

**Remarks**

Si le document n'a jamais été imprimé, cette propriété renverra DateTime.MinValue.

Aspose.Cells ne met pas à jour cette propriété lorsque vous modifiez le document.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLastPrintedUniversalTime() {#getLastPrintedUniversalTime--}
```
public DateTime getLastPrintedUniversalTime()
```


Obtient l'heure universelle à laquelle le document a été imprimé pour la dernière fois.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLastSavedBy() {#getLastSavedBy--}
```
public String getLastSavedBy()
```


Obtient le nom du dernier auteur.

**Remarks**

Aspose.Cells ne met pas à jour cette propriété lorsque vous modifiez le document.

**Returns:**
java.lang.String
### getLastSavedTime() {#getLastSavedTime--}
```
public DateTime getLastSavedTime()
```


Obtient l'heure de la dernière sauvegarde dans le fuseau horaire local.

**Remarks**

Aspose.Cells ne met pas à jour cette propriété lorsque vous modifiez le document.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLastSavedUniversalTime() {#getLastSavedUniversalTime--}
```
public DateTime getLastSavedUniversalTime()
```


Obtient l'heure universelle de la dernière sauvegarde.

**Remarks**

Aspose.Cells ne met pas à jour cette propriété lorsque vous modifiez le document.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLines() {#getLines--}
```
public int getLines()
```


Représente une estimation du nombre de lignes dans le document.

**Remarks**

Aspose.Cells ne met pas à jour cette propriété lorsque vous modifiez le document.

**Returns:**
int
### getLinksUpToDate() {#getLinksUpToDate--}
```
public boolean getLinksUpToDate()
```


Indique si les hyperliens dans un document sont à jour.

**Returns:**
boolean
### getManager() {#getManager--}
```
public String getManager()
```


Obtient la propriété manager.

**Returns:**
java.lang.String
### getNameOfApplication() {#getNameOfApplication--}
```
public String getNameOfApplication()
```


Obtient le nom de l'application.

**Returns:**
java.lang.String
### getPages() {#getPages--}
```
public int getPages()
```


Représente une estimation du nombre de pages dans le document.

**Returns:**
int
### getParagraphs() {#getParagraphs--}
```
public int getParagraphs()
```


Représente une estimation du nombre de paragraphes dans le document.

**Returns:**
int
### getRevisionNumber() {#getRevisionNumber--}
```
public String getRevisionNumber()
```


Obtient le numéro de révision du document.

**Remarks**

Aspose.Cells ne met pas à jour cette propriété lorsque vous modifiez le document.

**Returns:**
java.lang.String
### getScaleCrop() {#getScaleCrop--}
```
public boolean getScaleCrop()
```


Indique le mode d'affichage de la vignette du document.

**Returns:**
boolean
### getSubject() {#getSubject--}
```
public String getSubject()
```


Obtient le sujet du document.

**Returns:**
java.lang.String
### getTemplate() {#getTemplate--}
```
public String getTemplate()
```


Obtient le nom informatif du modèle de document.

**Returns:**
java.lang.String
### getTitle() {#getTitle--}
```
public String getTitle()
```


Obtient le titre du document.

**Returns:**
java.lang.String
### getTotalEditingTime() {#getTotalEditingTime--}
```
public double getTotalEditingTime()
```


Obtient le temps total d'édition en minutes.

**Returns:**
double
### getVersion() {#getVersion--}
```
public String getVersion()
```


Représente le numéro de version de l'application qui a créé le document.

**Remarks**

Son format est "00.0000", par exemple : 12.0000

**Returns:**
java.lang.String
### getWords() {#getWords--}
```
public int getWords()
```


Représente une estimation du nombre de mots dans le document.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Détermine l'index d'un élément spécifique dans l'instance CollectionBase.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | Détermine l'index d'un élément spécifique dans l'instance CollectionBase. |

**Returns:**
int - L'index de la valeur si elle est trouvée dans la liste ; sinon, -1.
### indexOf(String name) {#indexOf-java.lang.String-}
```
public int indexOf(String name)
```


Obtient l'indice d'une propriété par son nom.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de la propriété, insensible à la casse. |

**Returns:**
int - L'index basé sur zéro. Valeur négative si non trouvé.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Renvoie un énumérateur qui parcourt l'instance CollectionBase.

**Returns:**
java.util.Iterator - Un itérateur pour l'instance CollectionBase.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove(String name) {#remove-java.lang.String-}
```
public void remove(String name)
```


Supprime une propriété portant le nom spécifié de la collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de la propriété, insensible à la casse. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Supprime une propriété à l'indice spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index basé sur zéro. |

### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Définit le nom de l'auteur du document.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setBytes(int value) {#setBytes-int-}
```
public void setBytes(int value)
```


Représente une estimation du nombre d'octets dans le document.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setCategory(String value) {#setCategory-java.lang.String-}
```
public void setCategory(String value)
```


Définit la catégorie du document.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setCharacters(int value) {#setCharacters-int-}
```
public void setCharacters(int value)
```


Représente une estimation du nombre de caractères dans le document.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setCharactersWithSpaces(int value) {#setCharactersWithSpaces-int-}
```
public void setCharactersWithSpaces(int value)
```


Représente une estimation du nombre de caractères (espaces inclus) dans le document.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setComments(String value) {#setComments-java.lang.String-}
```
public void setComments(String value)
```


Définit les commentaires du document.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setCompany(String value) {#setCompany-java.lang.String-}
```
public void setCompany(String value)
```


Définit la propriété company.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setContentStatus(String value) {#setContentStatus-java.lang.String-}
```
public void setContentStatus(String value)
```


Définit l'état du contenu du document.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setContentType(String value) {#setContentType-java.lang.String-}
```
public void setContentType(String value)
```


Définit le type de contenu du document.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setCreatedTime(DateTime value) {#setCreatedTime-com.aspose.cells.DateTime-}
```
public void setCreatedTime(DateTime value)
```


Définit la date de création du document dans le fuseau horaire local.

**Remarks**

Aspose.Cells ne met pas à jour cette propriété lorsque vous modifiez le document.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setCreatedUniversalTime(DateTime value) {#setCreatedUniversalTime-com.aspose.cells.DateTime-}
```
public void setCreatedUniversalTime(DateTime value)
```


Définit l'heure universelle de création du document.

**Remarks**

Aspose.Cells ne met pas à jour cette propriété lorsque vous modifiez le document.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setDocumentVersion(String value) {#setDocumentVersion-java.lang.String-}
```
public void setDocumentVersion(String value)
```


Représente la version du fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setHyperlinkBase(String value) {#setHyperlinkBase-java.lang.String-}
```
public void setHyperlinkBase(String value)
```


Définit la propriété hyperlinkbase.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setKeywords(String value) {#setKeywords-java.lang.String-}
```
public void setKeywords(String value)
```


Définit les mots-clés du document.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setLanguage(String value) {#setLanguage-java.lang.String-}
```
public void setLanguage(String value)
```


Définit la langue du document.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setLastPrinted(DateTime value) {#setLastPrinted-com.aspose.cells.DateTime-}
```
public void setLastPrinted(DateTime value)
```


Définit la date à laquelle le document a été imprimé pour la dernière fois dans le fuseau horaire local.

**Remarks**

Si le document n'a jamais été imprimé, cette propriété renverra DateTime.MinValue.

Aspose.Cells ne met pas à jour cette propriété lorsque vous modifiez le document.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLastPrintedUniversalTime(DateTime value) {#setLastPrintedUniversalTime-com.aspose.cells.DateTime-}
```
public void setLastPrintedUniversalTime(DateTime value)
```


Définit l'heure universelle à laquelle le document a été imprimé pour la dernière fois.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLastSavedBy(String value) {#setLastSavedBy-java.lang.String-}
```
public void setLastSavedBy(String value)
```


Définit le nom du dernier auteur.

**Remarks**

Aspose.Cells ne met pas à jour cette propriété lorsque vous modifiez le document.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setLastSavedTime(DateTime value) {#setLastSavedTime-com.aspose.cells.DateTime-}
```
public void setLastSavedTime(DateTime value)
```


Définit l'heure de la dernière sauvegarde dans le fuseau horaire local.

**Remarks**

Aspose.Cells ne met pas à jour cette propriété lorsque vous modifiez le document.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLastSavedUniversalTime(DateTime value) {#setLastSavedUniversalTime-com.aspose.cells.DateTime-}
```
public void setLastSavedUniversalTime(DateTime value)
```


Définit l'heure universelle de la dernière sauvegarde.

**Remarks**

Aspose.Cells ne met pas à jour cette propriété lorsque vous modifiez le document.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLines(int value) {#setLines-int-}
```
public void setLines(int value)
```


Représente une estimation du nombre de lignes dans le document.

**Remarks**

Aspose.Cells ne met pas à jour cette propriété lorsque vous modifiez le document.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setLinksUpToDate(boolean value) {#setLinksUpToDate-boolean-}
```
public void setLinksUpToDate(boolean value)
```


Indique si les hyperliens dans un document sont à jour.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setManager(String value) {#setManager-java.lang.String-}
```
public void setManager(String value)
```


Définit la propriété manager.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setNameOfApplication(String value) {#setNameOfApplication-java.lang.String-}
```
public void setNameOfApplication(String value)
```


Définit le nom de l'application.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setPages(int value) {#setPages-int-}
```
public void setPages(int value)
```


Représente une estimation du nombre de pages dans le document.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setParagraphs(int value) {#setParagraphs-int-}
```
public void setParagraphs(int value)
```


Représente une estimation du nombre de paragraphes dans le document.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setRevisionNumber(String value) {#setRevisionNumber-java.lang.String-}
```
public void setRevisionNumber(String value)
```


Définit le numéro de révision du document.

**Remarks**

Aspose.Cells ne met pas à jour cette propriété lorsque vous modifiez le document.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setScaleCrop(boolean value) {#setScaleCrop-boolean-}
```
public void setScaleCrop(boolean value)
```


Indique le mode d'affichage de la vignette du document.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSubject(String value) {#setSubject-java.lang.String-}
```
public void setSubject(String value)
```


Définit le sujet du document.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setTemplate(String value) {#setTemplate-java.lang.String-}
```
public void setTemplate(String value)
```


Définit le nom informatif du modèle de document.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


Définit le titre du document.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setTotalEditingTime(double value) {#setTotalEditingTime-double-}
```
public void setTotalEditingTime(double value)
```


Définit le temps total d'édition en minutes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setVersion(String value) {#setVersion-java.lang.String-}
```
public void setVersion(String value)
```


Représente le numéro de version de l'application qui a créé le document.

**Remarks**

Son format est "00.0000", par exemple : 12.0000

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setWords(int value) {#setWords-int-}
```
public void setWords(int value)
```


Représente une estimation du nombre de mots dans le document.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

