---
title: "BuiltInDocumentPropertyCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Una colección de propiedades de documento incorporadas."
type: docs
url: /es/java/com.aspose.cells/builtindocumentpropertycollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase), [com.aspose.cells.DocumentPropertyCollection](../../com.aspose.cells/documentpropertycollection)
```
public class BuiltInDocumentPropertyCollection extends DocumentPropertyCollection
```

Una colección de propiedades de documento incorporadas.

**Remarks**

Proporciona acceso a objetos por sus nombres (usando un indexador) y mediante un conjunto de propiedades tipadas que devuelven valores de los tipos apropiados.
## Métodos

| Método | Descripción |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Agrega un elemento a la instancia de CollectionBase. |
| [clear()](#clear--) | Elimina todos los objetos de la instancia de CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Devuelve si la instancia contiene este objeto |
| [contains(String name)](#contains-java.lang.String-) | Devuelve true si una propiedad con el nombre especificado existe en la colección. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Devuelve un objeto [DocumentProperty](../../com.aspose.cells/documentproperty) por índice. |
| [get(String name)](#get-java.lang.String-) | Devuelve un objeto [DocumentProperty](../../com.aspose.cells/documentproperty) por el nombre de la propiedad. |
| [getAuthor()](#getAuthor--) | Obtiene el nombre del autor del documento. |
| [getBytes()](#getBytes--) | Representa una estimación del número de bytes en el documento. |
| [getCategory()](#getCategory--) | Obtiene la categoría del documento. |
| [getCharacters()](#getCharacters--) | Representa una estimación del número de caracteres en el documento. |
| [getCharactersWithSpaces()](#getCharactersWithSpaces--) | Representa una estimación del número de caracteres (incluidos los espacios) en el documento. |
| [getClass()](#getClass--) |  |
| [getComments()](#getComments--) | Obtiene los comentarios del documento. |
| [getCompany()](#getCompany--) | Obtiene la propiedad de la empresa. |
| [getContentStatus()](#getContentStatus--) | Obtiene el estado del contenido del documento. |
| [getContentType()](#getContentType--) | Obtiene el tipo de contenido del documento. |
| [getCount()](#getCount--) | Obtiene el número de elementos contenidos en la instancia de CollectionBase. |
| [getCreatedTime()](#getCreatedTime--) | Obtiene la fecha de creación del documento en la zona horaria local. |
| [getCreatedUniversalTime()](#getCreatedUniversalTime--) | Obtiene la hora universal de la creación del documento. |
| [getDocumentVersion()](#getDocumentVersion--) | Representa la versión del archivo. |
| [getHyperlinkBase()](#getHyperlinkBase--) | Obtiene la propiedad hyperlinkbase. |
| [getKeywords()](#getKeywords--) | Obtiene las palabras clave del documento. |
| [getLanguage()](#getLanguage--) | Obtiene el idioma del documento. |
| [getLastPrinted()](#getLastPrinted--) | Obtiene la fecha en que el documento se imprimió por última vez en la zona horaria local. |
| [getLastPrintedUniversalTime()](#getLastPrintedUniversalTime--) | Obtiene la hora universal en que el documento se imprimió por última vez. |
| [getLastSavedBy()](#getLastSavedBy--) | Obtiene el nombre del último autor. |
| [getLastSavedTime()](#getLastSavedTime--) | Obtiene la hora del último guardado en la zona horaria local. |
| [getLastSavedUniversalTime()](#getLastSavedUniversalTime--) | Obtiene la hora universal del último guardado. |
| [getLines()](#getLines--) | Representa una estimación del número de líneas en el documento. |
| [getLinksUpToDate()](#getLinksUpToDate--) | Indica si los hipervínculos en un documento están actualizados. |
| [getManager()](#getManager--) | Obtiene la propiedad manager. |
| [getNameOfApplication()](#getNameOfApplication--) | Obtiene el nombre de la aplicación. |
| [getPages()](#getPages--) | Representa una estimación del número de páginas en el documento. |
| [getParagraphs()](#getParagraphs--) | Representa una estimación del número de párrafos en el documento. |
| [getRevisionNumber()](#getRevisionNumber--) | Obtiene el número de revisión del documento. |
| [getScaleCrop()](#getScaleCrop--) | Indica el modo de visualización de la miniatura del documento. |
| [getSubject()](#getSubject--) | Obtiene el asunto del documento. |
| [getTemplate()](#getTemplate--) | Obtiene el nombre informativo de la plantilla del documento. |
| [getTitle()](#getTitle--) | Obtiene el título del documento. |
| [getTotalEditingTime()](#getTotalEditingTime--) | Obtiene el tiempo total de edición en minutos. |
| [getVersion()](#getVersion--) | Representa el número de versión de la aplicación que creó el documento. |
| [getWords()](#getWords--) | Representa una estimación del número de palabras en el documento. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina el índice de un elemento específico en la instancia de CollectionBase. |
| [indexOf(String name)](#indexOf-java.lang.String-) | Obtiene el índice de una propiedad por nombre. |
| [iterator()](#iterator--) | Devuelve un enumerador que recorre la instancia de CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String name)](#remove-java.lang.String-) | Elimina una propiedad con el nombre especificado de la colección. |
| [removeAt(int index)](#removeAt-int-) | Elimina una propiedad en el índice especificado. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Establece el nombre del autor del documento. |
| [setBytes(int value)](#setBytes-int-) | Representa una estimación del número de bytes en el documento. |
| [setCategory(String value)](#setCategory-java.lang.String-) | Establece la categoría del documento. |
| [setCharacters(int value)](#setCharacters-int-) | Representa una estimación del número de caracteres en el documento. |
| [setCharactersWithSpaces(int value)](#setCharactersWithSpaces-int-) | Representa una estimación del número de caracteres (incluidos los espacios) en el documento. |
| [setComments(String value)](#setComments-java.lang.String-) | Establece los comentarios del documento. |
| [setCompany(String value)](#setCompany-java.lang.String-) | Establece la propiedad company. |
| [setContentStatus(String value)](#setContentStatus-java.lang.String-) | Establece el estado del contenido del documento. |
| [setContentType(String value)](#setContentType-java.lang.String-) | Establece el tipo de contenido del documento. |
| [setCreatedTime(DateTime value)](#setCreatedTime-com.aspose.cells.DateTime-) | Establece la fecha de creación del documento en la zona horaria local. |
| [setCreatedUniversalTime(DateTime value)](#setCreatedUniversalTime-com.aspose.cells.DateTime-) | Establece la hora universal de la creación del documento. |
| [setDocumentVersion(String value)](#setDocumentVersion-java.lang.String-) | Representa la versión del archivo. |
| [setHyperlinkBase(String value)](#setHyperlinkBase-java.lang.String-) | Establece la propiedad hyperlinkbase. |
| [setKeywords(String value)](#setKeywords-java.lang.String-) | Establece las palabras clave del documento. |
| [setLanguage(String value)](#setLanguage-java.lang.String-) | Establece el idioma del documento. |
| [setLastPrinted(DateTime value)](#setLastPrinted-com.aspose.cells.DateTime-) | Establece la fecha en que el documento se imprimió por última vez en la zona horaria local. |
| [setLastPrintedUniversalTime(DateTime value)](#setLastPrintedUniversalTime-com.aspose.cells.DateTime-) | Establece la hora universal en que el documento se imprimió por última vez. |
| [setLastSavedBy(String value)](#setLastSavedBy-java.lang.String-) | Establece el nombre del último autor. |
| [setLastSavedTime(DateTime value)](#setLastSavedTime-com.aspose.cells.DateTime-) | Establece la hora de la última guardada en la zona horaria local. |
| [setLastSavedUniversalTime(DateTime value)](#setLastSavedUniversalTime-com.aspose.cells.DateTime-) | Establece la hora universal de la última guardada. |
| [setLines(int value)](#setLines-int-) | Representa una estimación del número de líneas en el documento. |
| [setLinksUpToDate(boolean value)](#setLinksUpToDate-boolean-) | Indica si los hipervínculos en un documento están actualizados. |
| [setManager(String value)](#setManager-java.lang.String-) | Establece la propiedad manager. |
| [setNameOfApplication(String value)](#setNameOfApplication-java.lang.String-) | Establece el nombre de la aplicación. |
| [setPages(int value)](#setPages-int-) | Representa una estimación del número de páginas en el documento. |
| [setParagraphs(int value)](#setParagraphs-int-) | Representa una estimación del número de párrafos en el documento. |
| [setRevisionNumber(String value)](#setRevisionNumber-java.lang.String-) | Establece el número de revisión del documento. |
| [setScaleCrop(boolean value)](#setScaleCrop-boolean-) | Indica el modo de visualización de la miniatura del documento. |
| [setSubject(String value)](#setSubject-java.lang.String-) | Establece el asunto del documento. |
| [setTemplate(String value)](#setTemplate-java.lang.String-) | Establece el nombre informativo de la plantilla del documento. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Establece el título del documento. |
| [setTotalEditingTime(double value)](#setTotalEditingTime-double-) | Establece el tiempo total de edición en minutos. |
| [setVersion(String value)](#setVersion-java.lang.String-) | Representa el número de versión de la aplicación que creó el documento. |
| [setWords(int value)](#setWords-int-) | Representa una estimación del número de palabras en el documento. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Agrega un elemento a la instancia de CollectionBase.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | El objeto a agregar a la instancia de CollectionBase. |

**Returns:**
int - La posición en la que se insertó el nuevo elemento.
### clear() {#clear--}
```
public void clear()
```


Elimina todos los objetos de la instancia de CollectionBase.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Devuelve si la instancia contiene este objeto

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | objeto de prueba |

**Returns:**
boolean - Si la instancia contiene este objeto
### contains(String name) {#contains-java.lang.String-}
```
public boolean contains(String name)
```


Devuelve true si una propiedad con el nombre especificado existe en la colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre de la propiedad sin distinción de mayúsculas. |

**Returns:**
boolean - True si la propiedad existe en la colección; false de lo contrario.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int index) {#get-int-}
```
public DocumentProperty get(int index)
```


Devuelve un objeto [DocumentProperty](../../com.aspose.cells/documentproperty) por índice.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| index | int | Índice basado en cero del [DocumentProperty](../../com.aspose.cells/documentproperty) a recuperar. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
### get(String name) {#get-java.lang.String-}
```
public DocumentProperty get(String name)
```


Devuelve un objeto [DocumentProperty](../../com.aspose.cells/documentproperty) por el nombre de la propiedad.

**Remarks**

Los nombres de cadena de las propiedades corresponden a los nombres de las propiedades tipadas disponibles desde .

Si solicita una propiedad que no está presente en el documento, pero el nombre de la propiedad se reconoce como un nombre incorporado válido, se crea una nueva  , se agrega a la colección y se devuelve. La propiedad recién creada se asigna con un valor predeterminado (cadena vacía, cero, falso o DateTime.MinValue según el tipo de la propiedad incorporada).

Si solicita una propiedad que no está presente en el documento y el nombre no se reconoce como un nombre incorporado, se devuelve null.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre de la propiedad sin distinción de mayúsculas a recuperar. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Obtiene el nombre del autor del documento.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public int getBytes()
```


Representa una estimación del número de bytes en el documento.

**Returns:**
int
### getCategory() {#getCategory--}
```
public String getCategory()
```


Obtiene la categoría del documento.

**Returns:**
java.lang.String
### getCharacters() {#getCharacters--}
```
public int getCharacters()
```


Representa una estimación del número de caracteres en el documento.

**Returns:**
int
### getCharactersWithSpaces() {#getCharactersWithSpaces--}
```
public int getCharactersWithSpaces()
```


Representa una estimación del número de caracteres (incluidos los espacios) en el documento.

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


Obtiene los comentarios del documento.

**Returns:**
java.lang.String
### getCompany() {#getCompany--}
```
public String getCompany()
```


Obtiene la propiedad de la empresa.

**Returns:**
java.lang.String
### getContentStatus() {#getContentStatus--}
```
public String getContentStatus()
```


Obtiene el estado del contenido del documento.

**Returns:**
java.lang.String
### getContentType() {#getContentType--}
```
public String getContentType()
```


Obtiene el tipo de contenido del documento.

**Returns:**
java.lang.String
### getCount() {#getCount--}
```
public int getCount()
```


Obtiene el número de elementos contenidos en la instancia de CollectionBase.

**Returns:**
int - El número de elementos contenidos en la instancia de CollectionBase.
### getCreatedTime() {#getCreatedTime--}
```
public DateTime getCreatedTime()
```


Obtiene la fecha de creación del documento en la zona horaria local.

**Remarks**

Aspose.Cells no actualiza esta propiedad cuando modifica el documento.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getCreatedUniversalTime() {#getCreatedUniversalTime--}
```
public DateTime getCreatedUniversalTime()
```


Obtiene la hora universal de la creación del documento.

**Remarks**

Aspose.Cells no actualiza esta propiedad cuando modifica el documento.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getDocumentVersion() {#getDocumentVersion--}
```
public String getDocumentVersion()
```


Representa la versión del archivo.

**Returns:**
java.lang.String
### getHyperlinkBase() {#getHyperlinkBase--}
```
public String getHyperlinkBase()
```


Obtiene la propiedad hyperlinkbase.

**Returns:**
java.lang.String
### getKeywords() {#getKeywords--}
```
public String getKeywords()
```


Obtiene las palabras clave del documento.

**Returns:**
java.lang.String
### getLanguage() {#getLanguage--}
```
public String getLanguage()
```


Obtiene el idioma del documento.

**Returns:**
java.lang.String
### getLastPrinted() {#getLastPrinted--}
```
public DateTime getLastPrinted()
```


Obtiene la fecha en que el documento se imprimió por última vez en la zona horaria local.

**Remarks**

Si el documento nunca se imprimió, esta propiedad devolverá DateTime.MinValue.

Aspose.Cells no actualiza esta propiedad cuando modifica el documento.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLastPrintedUniversalTime() {#getLastPrintedUniversalTime--}
```
public DateTime getLastPrintedUniversalTime()
```


Obtiene la hora universal en que el documento se imprimió por última vez.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLastSavedBy() {#getLastSavedBy--}
```
public String getLastSavedBy()
```


Obtiene el nombre del último autor.

**Remarks**

Aspose.Cells no actualiza esta propiedad cuando modifica el documento.

**Returns:**
java.lang.String
### getLastSavedTime() {#getLastSavedTime--}
```
public DateTime getLastSavedTime()
```


Obtiene la hora del último guardado en la zona horaria local.

**Remarks**

Aspose.Cells no actualiza esta propiedad cuando modifica el documento.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLastSavedUniversalTime() {#getLastSavedUniversalTime--}
```
public DateTime getLastSavedUniversalTime()
```


Obtiene la hora universal del último guardado.

**Remarks**

Aspose.Cells no actualiza esta propiedad cuando modifica el documento.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLines() {#getLines--}
```
public int getLines()
```


Representa una estimación del número de líneas en el documento.

**Remarks**

Aspose.Cells no actualiza esta propiedad cuando modifica el documento.

**Returns:**
int
### getLinksUpToDate() {#getLinksUpToDate--}
```
public boolean getLinksUpToDate()
```


Indica si los hipervínculos en un documento están actualizados.

**Returns:**
boolean
### getManager() {#getManager--}
```
public String getManager()
```


Obtiene la propiedad manager.

**Returns:**
java.lang.String
### getNameOfApplication() {#getNameOfApplication--}
```
public String getNameOfApplication()
```


Obtiene el nombre de la aplicación.

**Returns:**
java.lang.String
### getPages() {#getPages--}
```
public int getPages()
```


Representa una estimación del número de páginas en el documento.

**Returns:**
int
### getParagraphs() {#getParagraphs--}
```
public int getParagraphs()
```


Representa una estimación del número de párrafos en el documento.

**Returns:**
int
### getRevisionNumber() {#getRevisionNumber--}
```
public String getRevisionNumber()
```


Obtiene el número de revisión del documento.

**Remarks**

Aspose.Cells no actualiza esta propiedad cuando modifica el documento.

**Returns:**
java.lang.String
### getScaleCrop() {#getScaleCrop--}
```
public boolean getScaleCrop()
```


Indica el modo de visualización de la miniatura del documento.

**Returns:**
boolean
### getSubject() {#getSubject--}
```
public String getSubject()
```


Obtiene el asunto del documento.

**Returns:**
java.lang.String
### getTemplate() {#getTemplate--}
```
public String getTemplate()
```


Obtiene el nombre informativo de la plantilla del documento.

**Returns:**
java.lang.String
### getTitle() {#getTitle--}
```
public String getTitle()
```


Obtiene el título del documento.

**Returns:**
java.lang.String
### getTotalEditingTime() {#getTotalEditingTime--}
```
public double getTotalEditingTime()
```


Obtiene el tiempo total de edición en minutos.

**Returns:**
double
### getVersion() {#getVersion--}
```
public String getVersion()
```


Representa el número de versión de la aplicación que creó el documento.

**Remarks**

Su formato es "00.0000", por ejemplo: 12.0000.

**Returns:**
java.lang.String
### getWords() {#getWords--}
```
public int getWords()
```


Representa una estimación del número de palabras en el documento.

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


Determina el índice de un elemento específico en la instancia de CollectionBase.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | Determina el índice de un elemento específico en la instancia de CollectionBase. |

**Returns:**
int - El índice del valor si se encuentra en la lista; de lo contrario, -1.
### indexOf(String name) {#indexOf-java.lang.String-}
```
public int indexOf(String name)
```


Obtiene el índice de una propiedad por nombre.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre de la propiedad sin distinción de mayúsculas. |

**Returns:**
int - El índice basado en cero. Valor negativo si no se encuentra.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Devuelve un enumerador que recorre la instancia de CollectionBase.

**Returns:**
java.util.Iterator - Un iterador para la instancia de CollectionBase.
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


Elimina una propiedad con el nombre especificado de la colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre de la propiedad sin distinción de mayúsculas. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Elimina una propiedad en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice basado en cero. |

### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Establece el nombre del autor del documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setBytes(int value) {#setBytes-int-}
```
public void setBytes(int value)
```


Representa una estimación del número de bytes en el documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setCategory(String value) {#setCategory-java.lang.String-}
```
public void setCategory(String value)
```


Establece la categoría del documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setCharacters(int value) {#setCharacters-int-}
```
public void setCharacters(int value)
```


Representa una estimación del número de caracteres en el documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setCharactersWithSpaces(int value) {#setCharactersWithSpaces-int-}
```
public void setCharactersWithSpaces(int value)
```


Representa una estimación del número de caracteres (incluidos los espacios) en el documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setComments(String value) {#setComments-java.lang.String-}
```
public void setComments(String value)
```


Establece los comentarios del documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setCompany(String value) {#setCompany-java.lang.String-}
```
public void setCompany(String value)
```


Establece la propiedad company.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setContentStatus(String value) {#setContentStatus-java.lang.String-}
```
public void setContentStatus(String value)
```


Establece el estado del contenido del documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setContentType(String value) {#setContentType-java.lang.String-}
```
public void setContentType(String value)
```


Establece el tipo de contenido del documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setCreatedTime(DateTime value) {#setCreatedTime-com.aspose.cells.DateTime-}
```
public void setCreatedTime(DateTime value)
```


Establece la fecha de creación del documento en la zona horaria local.

**Remarks**

Aspose.Cells no actualiza esta propiedad cuando modifica el documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setCreatedUniversalTime(DateTime value) {#setCreatedUniversalTime-com.aspose.cells.DateTime-}
```
public void setCreatedUniversalTime(DateTime value)
```


Establece la hora universal de la creación del documento.

**Remarks**

Aspose.Cells no actualiza esta propiedad cuando modifica el documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setDocumentVersion(String value) {#setDocumentVersion-java.lang.String-}
```
public void setDocumentVersion(String value)
```


Representa la versión del archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setHyperlinkBase(String value) {#setHyperlinkBase-java.lang.String-}
```
public void setHyperlinkBase(String value)
```


Establece la propiedad hyperlinkbase.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setKeywords(String value) {#setKeywords-java.lang.String-}
```
public void setKeywords(String value)
```


Establece las palabras clave del documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setLanguage(String value) {#setLanguage-java.lang.String-}
```
public void setLanguage(String value)
```


Establece el idioma del documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setLastPrinted(DateTime value) {#setLastPrinted-com.aspose.cells.DateTime-}
```
public void setLastPrinted(DateTime value)
```


Establece la fecha en que el documento se imprimió por última vez en la zona horaria local.

**Remarks**

Si el documento nunca se imprimió, esta propiedad devolverá DateTime.MinValue.

Aspose.Cells no actualiza esta propiedad cuando modifica el documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLastPrintedUniversalTime(DateTime value) {#setLastPrintedUniversalTime-com.aspose.cells.DateTime-}
```
public void setLastPrintedUniversalTime(DateTime value)
```


Establece la hora universal en que el documento se imprimió por última vez.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLastSavedBy(String value) {#setLastSavedBy-java.lang.String-}
```
public void setLastSavedBy(String value)
```


Establece el nombre del último autor.

**Remarks**

Aspose.Cells no actualiza esta propiedad cuando modifica el documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setLastSavedTime(DateTime value) {#setLastSavedTime-com.aspose.cells.DateTime-}
```
public void setLastSavedTime(DateTime value)
```


Establece la hora de la última guardada en la zona horaria local.

**Remarks**

Aspose.Cells no actualiza esta propiedad cuando modifica el documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLastSavedUniversalTime(DateTime value) {#setLastSavedUniversalTime-com.aspose.cells.DateTime-}
```
public void setLastSavedUniversalTime(DateTime value)
```


Establece la hora universal de la última guardada.

**Remarks**

Aspose.Cells no actualiza esta propiedad cuando modifica el documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLines(int value) {#setLines-int-}
```
public void setLines(int value)
```


Representa una estimación del número de líneas en el documento.

**Remarks**

Aspose.Cells no actualiza esta propiedad cuando modifica el documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setLinksUpToDate(boolean value) {#setLinksUpToDate-boolean-}
```
public void setLinksUpToDate(boolean value)
```


Indica si los hipervínculos en un documento están actualizados.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setManager(String value) {#setManager-java.lang.String-}
```
public void setManager(String value)
```


Establece la propiedad manager.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setNameOfApplication(String value) {#setNameOfApplication-java.lang.String-}
```
public void setNameOfApplication(String value)
```


Establece el nombre de la aplicación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setPages(int value) {#setPages-int-}
```
public void setPages(int value)
```


Representa una estimación del número de páginas en el documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setParagraphs(int value) {#setParagraphs-int-}
```
public void setParagraphs(int value)
```


Representa una estimación del número de párrafos en el documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setRevisionNumber(String value) {#setRevisionNumber-java.lang.String-}
```
public void setRevisionNumber(String value)
```


Establece el número de revisión del documento.

**Remarks**

Aspose.Cells no actualiza esta propiedad cuando modifica el documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setScaleCrop(boolean value) {#setScaleCrop-boolean-}
```
public void setScaleCrop(boolean value)
```


Indica el modo de visualización de la miniatura del documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSubject(String value) {#setSubject-java.lang.String-}
```
public void setSubject(String value)
```


Establece el asunto del documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setTemplate(String value) {#setTemplate-java.lang.String-}
```
public void setTemplate(String value)
```


Establece el nombre informativo de la plantilla del documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


Establece el título del documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setTotalEditingTime(double value) {#setTotalEditingTime-double-}
```
public void setTotalEditingTime(double value)
```


Establece el tiempo total de edición en minutos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setVersion(String value) {#setVersion-java.lang.String-}
```
public void setVersion(String value)
```


Representa el número de versión de la aplicación que creó el documento.

**Remarks**

Su formato es "00.0000", por ejemplo: 12.0000.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setWords(int value) {#setWords-int-}
```
public void setWords(int value)
```


Representa una estimación del número de palabras en el documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

