---
title: "TickLabels"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa las etiquetas de marcas asociadas con las marcas de escala en el eje de un gráfico."
type: docs
url: /es/java/com.aspose.cells/ticklabels/
---

**Inheritance:**
java.lang.Object
```
public class TickLabels
```

Representa las etiquetas de marcas asociadas con las marcas de escala en el eje de un gráfico.
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlignmentType()](#getAlignmentType--) | Obtiene la alineación de texto para las etiquetas de marcas en el eje. |
| [getAutoScaleFont()](#getAutoScaleFont--) | Verdadero si el texto en el objeto cambia el tamaño de fuente cuando el tamaño del objeto cambia. |
| [getBackgroundMode()](#getBackgroundMode--) | Obtiene el modo de visualización del fondo |
| [getClass()](#getClass--) |  |
| [getDirectionType()](#getDirectionType--) | Obtiene la dirección del texto. |
| [getDisplayNumberFormat()](#getDisplayNumberFormat--) | Obtiene el formato numérico de visualización de las etiquetas de marcas. |
| [getFont()](#getFont--) | Devuelve un objeto [getFont()](../../com.aspose.cells/ticklabels\#getFont--) que representa la fuente del objeto TickLabels especificado. |
| [getNumber()](#getNumber--) | Representa el número de formato para el objeto TickLabels. |
| [getNumberFormat()](#getNumberFormat--) | Representa la cadena de formato para el objeto TickLabels. |
| [getNumberFormatLinked()](#getNumberFormatLinked--) | Verdadero si el formato numérico está vinculado a las celdas (de modo que el formato numérico cambie en las etiquetas cuando cambie en las celdas). |
| [getOffset()](#getOffset--) | Obtiene la distancia de las etiquetas del eje de categorías. |
| [getReadingOrder()](#getReadingOrder--) | Representa el orden de lectura del texto. |
| [getRotationAngle()](#getRotationAngle--) | Representa el ángulo de rotación del texto en sentido horario. |
| [getTextDirection()](#getTextDirection--) | Representa el orden de lectura del texto. |
| [getTickLabelItems()](#getTickLabelItems--) | Obtiene las etiquetas de marcas de visualización del eje. |
| [hashCode()](#hashCode--) |  |
| [isAutomaticRotation()](#isAutomaticRotation--) | Indica si el ángulo de rotación es automático |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlignmentType(int value)](#setAlignmentType-int-) | Establece la alineación del texto para las etiquetas de marcas en el eje. |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | Verdadero si el texto en el objeto cambia el tamaño de fuente cuando el tamaño del objeto cambia. |
| [setAutomaticRotation(boolean value)](#setAutomaticRotation-boolean-) | Indica si el ángulo de rotación es automático |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Establece el modo de visualización del fondo |
| [setDirectionType(int value)](#setDirectionType-int-) | Establece la dirección del texto. |
| [setNumber(int value)](#setNumber-int-) | Representa el número de formato para el objeto TickLabels. |
| [setNumberFormat(String value)](#setNumberFormat-java.lang.String-) | Representa la cadena de formato para el objeto TickLabels. |
| [setNumberFormatLinked(boolean value)](#setNumberFormatLinked-boolean-) | Verdadero si el formato numérico está vinculado a las celdas (de modo que el formato numérico cambie en las etiquetas cuando cambie en las celdas). |
| [setOffset(int value)](#setOffset-int-) | Establece la distancia de las etiquetas respecto al eje de categorías. |
| [setReadingOrder(int value)](#setReadingOrder-int-) | Representa el orden de lectura del texto. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Representa el ángulo de rotación del texto en sentido horario. |
| [setTextDirection(int value)](#setTextDirection-int-) | Representa el orden de lectura del texto. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getAlignmentType() {#getAlignmentType--}
```
public int getAlignmentType()
```


Obtiene la alineación de texto para las etiquetas de marcas en el eje.

Ver [TickLabelAlignmentType](../../com.aspose.cells/ticklabelalignmenttype).

**Returns:**
int
### getAutoScaleFont() {#getAutoScaleFont--}
```
public boolean getAutoScaleFont()
```


Verdadero si el texto en el objeto cambia el tamaño de fuente cuando el tamaño del objeto cambia. El valor predeterminado es Verdadero.

**Returns:**
boolean
### getBackgroundMode() {#getBackgroundMode--}
```
public int getBackgroundMode()
```


Obtiene el modo de visualización del fondo

Ver [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDirectionType() {#getDirectionType--}
```
public int getDirectionType()
```


Obtiene la dirección del texto.

Ver [ChartTextDirectionType](../../com.aspose.cells/charttextdirectiontype).

**Returns:**
int
### getDisplayNumberFormat() {#getDisplayNumberFormat--}
```
public String getDisplayNumberFormat()
```


Obtiene el formato numérico de visualización de las etiquetas de marcas.

**Returns:**
java.lang.String
### getFont() {#getFont--}
```
public Font getFont()
```


Devuelve un objeto [getFont()](../../com.aspose.cells/ticklabels\#getFont--) que representa la fuente del objeto TickLabels especificado.

**Returns:**
[Font](../../com.aspose.cells/font)
### getNumber() {#getNumber--}
```
public int getNumber()
```


Representa el número de formato para el objeto TickLabels.

**Returns:**
int
### getNumberFormat() {#getNumberFormat--}
```
public String getNumberFormat()
```


Representa la cadena de formato para el objeto TickLabels.

**Remarks**

La cadena de formato es la misma que una cadena de formato personalizado asignada a una celda. Por ejemplo, \"$0\".

**Returns:**
java.lang.String
### getNumberFormatLinked() {#getNumberFormatLinked--}
```
public boolean getNumberFormatLinked()
```


Verdadero si el formato numérico está vinculado a las celdas (de modo que el formato numérico cambie en las etiquetas cuando cambie en las celdas).

**Returns:**
boolean
### getOffset() {#getOffset--}
```
public int getOffset()
```


Obtiene la distancia de las etiquetas respecto al eje de categorías. Esto se aplica solo al eje de categorías (x).

**Remarks**

La distancia predeterminada es 100 por ciento, lo que representa el espaciado predeterminado entre las etiquetas del eje y la línea del eje. El valor puede ser un porcentaje entero de 0 a 1000, relativo al tamaño de fuente de la etiqueta del eje.

**Returns:**
int
### getReadingOrder() {#getReadingOrder--}
```
public int getReadingOrder()
```


Representa el orden de lectura del texto.

Ver [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


Representa el ángulo de rotación del texto en sentido horario.

**Remarks**


0: No rotado.

255: De arriba a abajo.

\-90: Hacia abajo.

90: Hacia arriba.


**Returns:**
int
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```


Representa el orden de lectura del texto.

Ver [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad TickLabels.ReadingOrder. Esta propiedad será eliminada 12 meses después desde marzo de 2020. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
### getTickLabelItems() {#getTickLabelItems--}
```
public TickLabelItem[] getTickLabelItems()
```


Obtiene las etiquetas de marcas de visualización del eje.

**Remarks**

Solo disponible después de llamar al método [Chart.calculate()](../../com.aspose.cells/chart\\#calculate--).

**Returns:**
com.aspose.cells.TickLabelItem[]
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutomaticRotation() {#isAutomaticRotation--}
```
public boolean isAutomaticRotation()
```


Indica si el ángulo de rotación es automático

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAlignmentType(int value) {#setAlignmentType-int-}
```
public void setAlignmentType(int value)
```


Establece la alineación del texto para las etiquetas de marcas en el eje.

Ver [TickLabelAlignmentType](../../com.aspose.cells/ticklabelalignmenttype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setAutoScaleFont(boolean value) {#setAutoScaleFont-boolean-}
```
public void setAutoScaleFont(boolean value)
```


Verdadero si el texto en el objeto cambia el tamaño de fuente cuando el tamaño del objeto cambia. El valor predeterminado es Verdadero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAutomaticRotation(boolean value) {#setAutomaticRotation-boolean-}
```
public void setAutomaticRotation(boolean value)
```


Indica si el ángulo de rotación es automático

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setBackgroundMode(int value) {#setBackgroundMode-int-}
```
public void setBackgroundMode(int value)
```


Establece el modo de visualización del fondo

Ver [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setDirectionType(int value) {#setDirectionType-int-}
```
public void setDirectionType(int value)
```


Establece la dirección del texto.

Ver [ChartTextDirectionType](../../com.aspose.cells/charttextdirectiontype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
```


Representa el número de formato para el objeto TickLabels.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setNumberFormat(String value) {#setNumberFormat-java.lang.String-}
```
public void setNumberFormat(String value)
```


Representa la cadena de formato para el objeto TickLabels.

**Remarks**

La cadena de formato es la misma que una cadena de formato personalizado asignada a una celda. Por ejemplo, \"$0\".

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setNumberFormatLinked(boolean value) {#setNumberFormatLinked-boolean-}
```
public void setNumberFormatLinked(boolean value)
```


Verdadero si el formato numérico está vinculado a las celdas (de modo que el formato numérico cambie en las etiquetas cuando cambie en las celdas).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setOffset(int value) {#setOffset-int-}
```
public void setOffset(int value)
```


Establece la distancia de las etiquetas respecto al eje de categorías. Esto se aplica solo al eje de categorías (x).

**Remarks**

La distancia predeterminada es 100 por ciento, lo que representa el espaciado predeterminado entre las etiquetas del eje y la línea del eje. El valor puede ser un porcentaje entero de 0 a 1000, relativo al tamaño de fuente de la etiqueta del eje.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setReadingOrder(int value) {#setReadingOrder-int-}
```
public void setReadingOrder(int value)
```


Representa el orden de lectura del texto.

Ver [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


Representa el ángulo de rotación del texto en sentido horario.

**Remarks**


0: No rotado.

255: De arriba a abajo.

\-90: Hacia abajo.

90: Hacia arriba.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


Representa el orden de lectura del texto.

Ver [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad TickLabels.ReadingOrder. Esta propiedad será eliminada 12 meses después desde marzo de 2020. Aspose se disculpa por cualquier inconveniente que haya experimentado.

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

