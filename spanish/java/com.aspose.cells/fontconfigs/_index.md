---
title: "FontConfigs"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Especifica la configuración de fuente"
type: docs
url: /es/java/com.aspose.cells/fontconfigs/
---

**Inheritance:**
java.lang.Object
```
public class FontConfigs
```

Especifica la configuración de fuente
## Constructores

| Constructor | Descripción |
| --- | --- |
| [FontConfigs()](#FontConfigs--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDefaultFontName()](#getDefaultFontName--) | Obtiene el nombre de fuente predeterminado. |
| [getFontFileDataInfo(String fontName, boolean isBold, boolean isItalic, boolean isExactStyle)](#getFontFileDataInfo-java.lang.String-boolean-boolean-boolean-) | Obtiene información de datos del archivo de fuente. |
| [getFontSources()](#getFontSources--) | Obtiene una copia del arreglo que contiene la lista de fuentes |
| [getFontSubstitutes(String originalFontName)](#getFontSubstitutes-java.lang.String-) | Devuelve un arreglo que contiene nombres de fuentes sustitutas que se usarán si la fuente original no está presente. |
| [hashCode()](#hashCode--) |  |
| [isFontAvailable(String fontName)](#isFontAvailable-java.lang.String-) | Indica si la fuente está disponible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Establece el nombre de fuente predeterminado. |
| [setFontExclusiveSources(FontSourceBase[] exclusiveSources)](#setFontExclusiveSources-com.aspose.cells.FontSourceBase---) | Establece las fuentes exclusivas de fuentes. |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | Establece la carpeta de fuentes |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Establece la carpeta de fuentes |
| [setFontSources(FontSourceBase[] sources)](#setFontSources-com.aspose.cells.FontSourceBase---) | Establece las fuentes de fuentes. |
| [setFontSubstitutes(String originalFontName, String[] substituteFontNames)](#setFontSubstitutes-java.lang.String-java.lang.String---) | Nombres de sustitución de fuentes para el nombre de fuente original dado. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FontConfigs() {#FontConfigs--}
```
public FontConfigs()
```


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
### getDefaultFontName() {#getDefaultFontName--}
```
public static String getDefaultFontName()
```


Obtiene el nombre de fuente predeterminado.

**Returns:**
java.lang.String
### getFontFileDataInfo(String fontName, boolean isBold, boolean isItalic, boolean isExactStyle) {#getFontFileDataInfo-java.lang.String-boolean-boolean-boolean-}
```
public static FontFileDataInfo getFontFileDataInfo(String fontName, boolean isBold, boolean isItalic, boolean isExactStyle)
```


Obtiene información de datos del archivo de fuente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fontName | java.lang.String | nombre de fuente |
| isBold | boolean | el estilo de fuente es negrita o no |
| isItalic | boolean | el estilo de fuente es cursiva o no |
| isExactStyle | boolean | si coincidir exactamente con el estilo negrita/cursiva dado |

**Returns:**
[FontFileDataInfo](../../com.aspose.cells/fontfiledatainfo) - Data infomation of font file data.
### getFontSources() {#getFontSources--}
```
public static FontSourceBase[] getFontSources()
```


Obtiene una copia del arreglo que contiene la lista de fuentes

**Returns:**
com.aspose.cells.FontSourceBase[] -
### getFontSubstitutes(String originalFontName) {#getFontSubstitutes-java.lang.String-}
```
public static String[] getFontSubstitutes(String originalFontName)
```


Devuelve un arreglo que contiene nombres de fuentes sustitutas que se usarán si la fuente original no está presente.

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
### isFontAvailable(String fontName) {#isFontAvailable-java.lang.String-}
```
public static boolean isFontAvailable(String fontName)
```


Indica si la fuente está disponible.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fontName | java.lang.String | nombre de fuente |

**Returns:**
boolean - verdadero si la fuente está disponible, de lo contrario falso.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public static void setDefaultFontName(String value)
```


Establece el nombre de fuente predeterminado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setFontExclusiveSources(FontSourceBase[] exclusiveSources) {#setFontExclusiveSources-com.aspose.cells.FontSourceBase---}
```
public static void setFontExclusiveSources(FontSourceBase[] exclusiveSources)
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
public static void setFontFolder(String fontFolder, boolean recursive)
```


Establece la carpeta de fuentes

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fontFolder | java.lang.String | La carpeta que contiene fuentes TrueType. |
| recursive | boolean | Determina si se deben escanear o no las subcarpetas. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public static void setFontFolders(String[] fontFolders, boolean recursive)
```


Establece la carpeta de fuentes

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fontFolders | java.lang.String[] | Las carpetas que contienen fuentes TrueType. |
| recursive | boolean | Determina si se deben escanear o no las subcarpetas. |

### setFontSources(FontSourceBase[] sources) {#setFontSources-com.aspose.cells.FontSourceBase---}
```
public static void setFontSources(FontSourceBase[] sources)
```


Establece las fuentes de fuentes.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | Una matriz de fuentes que contienen fuentes TrueType. |

### setFontSubstitutes(String originalFontName, String[] substituteFontNames) {#setFontSubstitutes-java.lang.String-java.lang.String---}
```
public static void setFontSubstitutes(String originalFontName, String[] substituteFontNames)
```


Nombres de sustitución de fuentes para el nombre de fuente original dado.

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

