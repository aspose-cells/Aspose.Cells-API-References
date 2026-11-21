---
title: "FontSettingCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la lista de ."
type: docs
url: /es/java/com.aspose.cells/fontsettingcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class FontSettingCollection extends CollectionBase
```

Representa la lista de [FontSetting](../../com.aspose.cells/fontsetting).
## Métodos

| Método | Descripción |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Agrega un elemento a la instancia de CollectionBase. |
| [appendText(String text)](#appendText-java.lang.String-) | Añade el texto. |
| [clear()](#clear--) | Borra todas las configuraciones. |
| [contains(Object o)](#contains-java.lang.Object-) | Devuelve si la instancia contiene este objeto |
| [deleteText(int index, int count)](#deleteText-int-int-) | Eliminar algunos caracteres. |
| [equals(Object obj)](#equals-java.lang.Object-) |  |
| [format(int startIndex, int length, Font font, StyleFlag flag)](#format-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-) | Formatear el texto con la configuración de fuente. |
| [get(int index)](#get-int-) | Obtiene el [FontSetting](../../com.aspose.cells/fontsetting) por el índice. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtiene el número de elementos contenidos en la instancia de CollectionBase. |
| [getHtmlString()](#getHtmlString--) | Obtiene la cadena html que contiene datos y algunos formatos en esta forma. |
| [getParagraphEnumerator()](#getParagraphEnumerator--) | Obtiene el enumerador de los párrafos. |
| [getText()](#getText--) | Obtiene el texto de la forma. |
| [getTextAlignment()](#getTextAlignment--) | Representa la configuración de alineación del cuerpo del texto. |
| [getTextParagraphs()](#getTextParagraphs--) | Obtiene todos los párrafos. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina el índice de un elemento específico en la instancia de CollectionBase. |
| [insertText(int index, String text)](#insertText-int-java.lang.String-) | Insertar índice en la posición. |
| [iterator()](#iterator--) | Devuelve un enumerador que recorre la instancia de CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Elimina el elemento en el índice especificado. |
| [replace(int index, int count, String text)](#replace-int-int-java.lang.String-) | Reemplazar el texto. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | Reemplazar el texto. |
| [setHtmlString(String value)](#setHtmlString-java.lang.String-) | Establece la cadena html que contiene datos y algunos formatos en esta forma. |
| [setText(String value)](#setText-java.lang.String-) | Establece el texto de la forma. |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | Establece el estilo WordArt predefinido. |
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
### appendText(String text) {#appendText-java.lang.String-}
```
public void appendText(String text)
```


Añade el texto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| texto | java.lang.String | El texto. |

### clear() {#clear--}
```
public void clear()
```


Borra todas las configuraciones.

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
### deleteText(int index, int count) {#deleteText-int-int-}
```
public void deleteText(int index, int count)
```


Eliminar algunos caracteres.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice de inicio. |
| recuento | int | El recuento de caracteres. |

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### format(int startIndex, int length, Font font, StyleFlag flag) {#format-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-}
```
public void format(int startIndex, int length, Font font, StyleFlag flag)
```


Formatear el texto con la configuración de fuente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startIndex | int | El índice de inicio. |
| length | int | La longitud. |
| font | [Font](../../com.aspose.cells/font) | La fuente. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Las banderas de la fuente. |

### get(int index) {#get-int-}
```
public FontSetting get(int index)
```


Obtiene el [FontSetting](../../com.aspose.cells/fontsetting) por el índice.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - 
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Obtiene el número de elementos contenidos en la instancia de CollectionBase.

**Returns:**
int - El número de elementos contenidos en la instancia de CollectionBase.
### getHtmlString() {#getHtmlString--}
```
public String getHtmlString()
```


Obtiene la cadena html que contiene datos y algunos formatos en esta forma.

**Returns:**
java.lang.String
### getParagraphEnumerator() {#getParagraphEnumerator--}
```
public Iterator getParagraphEnumerator()
```


Obtiene el enumerador de los párrafos.

**Returns:**
java.util.Iterator -
### getText() {#getText--}
```
public String getText()
```


Obtiene el texto de la forma.

**Returns:**
java.lang.String
### getTextAlignment() {#getTextAlignment--}
```
public ShapeTextAlignment getTextAlignment()
```


Representa la configuración de alineación del cuerpo del texto.

**Returns:**
[ShapeTextAlignment](../../com.aspose.cells/shapetextalignment)
### getTextParagraphs() {#getTextParagraphs--}
```
public TextParagraphCollection getTextParagraphs()
```


Obtiene todos los párrafos.

**Returns:**
[TextParagraphCollection](../../com.aspose.cells/textparagraphcollection)
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int -
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
### insertText(int index, String text) {#insertText-int-java.lang.String-}
```
public void insertText(int index, String text)
```


Insertar índice en la posición.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice de inicio. |
| texto | java.lang.String | El texto. |

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




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Elimina el elemento en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice basado en cero del elemento a eliminar. |

### replace(int index, int count, String text) {#replace-int-int-java.lang.String-}
```
public void replace(int index, int count, String text)
```


Reemplazar el texto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice de inicio. |
| recuento | int | El recuento de caracteres. |
| texto | java.lang.String | El texto. |

### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public void replace(String oldValue, String newValue)
```


Reemplazar el texto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valorAntiguo | java.lang.String | El texto antiguo. |
| newValue | java.lang.String | El texto nuevo. |

### setHtmlString(String value) {#setHtmlString-java.lang.String-}
```
public void setHtmlString(String value)
```


Establece la cadena html que contiene datos y algunos formatos en esta forma.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Establece el texto de la forma.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setWordArtStyle(int style) {#setWordArtStyle-int-}
```
public void setWordArtStyle(int style)
```


Establece el estilo WordArt predefinido.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). El estilo WordArt predefinido. |

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

