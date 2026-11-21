---
title: "IndividualFontConfigs"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Configuraciones de fuente para cada objeto."
type: docs
url: /es/java/com.aspose.cells/individualfontconfigs/
---

**Inheritance:**
java.lang.Object
```
public class IndividualFontConfigs
```

Configuraciones de fuente para cada objeto [Workbook](../../com.aspose.cells/workbook).
## Constructores

| Constructor | Descripción |
| --- | --- |
| [IndividualFontConfigs()](#IndividualFontConfigs--) | Ctor. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFontSources()](#getFontSources--) | Obtiene una copia del arreglo que contiene la lista de fuentes |
| [getFontSubstitutes(String originalFontName)](#getFontSubstitutes-java.lang.String-) | Devuelve una matriz que contiene nombres de fuentes sustitutas que se usarán si la fuente original no está presente. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFontExclusiveSources(FontSourceBase[] exclusiveSources)](#setFontExclusiveSources-com.aspose.cells.FontSourceBase---) | Establece las fuentes exclusivas de fuentes. |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | Establece la carpeta de fuentes |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Establece las carpetas de fuentes |
| [setFontSources(FontSourceBase[] sources)](#setFontSources-com.aspose.cells.FontSourceBase---) | Establece las fuentes de fuentes. |
| [setFontSubstitutes(String originalFontName, String[] substituteFontNames)](#setFontSubstitutes-java.lang.String-java.lang.String---) | Establece nombres de fuentes sustitutas para un nombre de fuente original dado. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### IndividualFontConfigs() {#IndividualFontConfigs--}
```
public IndividualFontConfigs()
```


Ctor.

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFontSources() {#getFontSources--}
```
public FontSourceBase[] getFontSources()
```


Obtiene una copia del arreglo que contiene la lista de fuentes

**Returns:**
com.aspose.cells.FontSourceBase[] -
### getFontSubstitutes(String originalFontName) {#getFontSubstitutes-java.lang.String-}
```
public String[] getFontSubstitutes(String originalFontName)
```


Devuelve una matriz que contiene nombres de fuentes sustitutas que se usarán si la fuente original no está presente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| originalFontName | java.lang.String | originalFontName |

**Returns:**
java.lang.String[] - Una matriz que contiene nombres de sustitución de fuentes para usar si la fuente original no está presente.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setFontExclusiveSources(FontSourceBase[] exclusiveSources) {#setFontExclusiveSources-com.aspose.cells.FontSourceBase---}
```
public void setFontExclusiveSources(FontSourceBase[] exclusiveSources)
```


Establece las fuentes exclusivas de fuentes. Solo se usarán las fuentes en las fuentes.

**Remarks**

System.setProperty(\"Aspose.Cells.FontDirExc\", \"fontExclusiveFolder\") será ignorado si esto está configurado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| exclusiveSources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | Una matriz de fuentes que contienen fuentes TrueType. |

### setFontFolder(String fontFolder, boolean recursive) {#setFontFolder-java.lang.String-boolean-}
```
public void setFontFolder(String fontFolder, boolean recursive)
```


Establece la carpeta de fuentes

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fontFolder | java.lang.String | La carpeta que contiene fuentes TrueType. |
| recursive | boolean | Determina si se deben escanear o no las subcarpetas. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public void setFontFolders(String[] fontFolders, boolean recursive)
```


Establece las carpetas de fuentes

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fontFolders | java.lang.String[] | Las carpetas que contienen fuentes TrueType. |
| recursive | boolean | Determina si se deben escanear o no las subcarpetas. |

### setFontSources(FontSourceBase[] sources) {#setFontSources-com.aspose.cells.FontSourceBase---}
```
public void setFontSources(FontSourceBase[] sources)
```


Establece las fuentes de fuentes.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | Una matriz de fuentes que contienen fuentes TrueType. |

### setFontSubstitutes(String originalFontName, String[] substituteFontNames) {#setFontSubstitutes-java.lang.String-java.lang.String---}
```
public void setFontSubstitutes(String originalFontName, String[] substituteFontNames)
```


Establece nombres de fuentes sustitutas para un nombre de fuente original dado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| originalFontName | java.lang.String | Nombre de fuente original. |
| substituteFontNames | java.lang.String[] | Lista de nombres de fuentes sustitutas que se usarán si la fuente original no está presente. |

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

