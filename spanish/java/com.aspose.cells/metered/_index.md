---
title: "Medido"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Proporciona métodos para establecer la clave medida."
type: docs
url: /es/java/com.aspose.cells/metered/
---

**Inheritance:**
java.lang.Object
```
public class Metered
```

Proporciona métodos para establecer la clave medida.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [Metered()](#Metered--) | Inicializa una nueva instancia de esta clase. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getConsumptionCredit()](#getConsumptionCredit--) | Obtiene el crédito de consumo |
| [getConsumptionQuantity()](#getConsumptionQuantity--) | Obtiene el tamaño del archivo de consumo |
| [getProductName()](#getProductName--) | Obtiene el nombre del producto |
| [hashCode()](#hashCode--) |  |
| [isMeteredLicensed()](#isMeteredLicensed--) | Compruebe si la medida está licenciada |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Establece la clave pública y privada medida. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Metered() {#Metered--}
```
public Metered()
```


Inicializa una nueva instancia de esta clase.

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
### getConsumptionCredit() {#getConsumptionCredit--}
```
public static double getConsumptionCredit()
```


Obtiene el crédito de consumo

**Returns:**
double - cantidad de consumo
### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static double getConsumptionQuantity()
```


Obtiene el tamaño del archivo de consumo

**Returns:**
double - cantidad de consumo
### getProductName() {#getProductName--}
```
public String getProductName()
```


Obtiene el nombre del producto

**Returns:**
java.lang.String - nombre del producto
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isMeteredLicensed() {#isMeteredLicensed--}
```
public static boolean isMeteredLicensed()
```


Compruebe si la medida está licenciada

**Returns:**
boolean - Verdadero o falso
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public void setMeteredKey(String publicKey, String privateKey)
```


Establece la clave pública y privada medida. Si compra una licencia medida, al iniciar la aplicación, esta API debe ser llamada; normalmente, esto es suficiente. Sin embargo, si siempre falla la carga de datos de consumo y supera las 24 horas, la licencia se establecerá en estado de evaluación; para evitar tal caso, debe comprobar regularmente el estado de la licencia, y si está en estado de evaluación, llamar a esta API nuevamente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| publicKey | java.lang.String | clave pública |
| privateKey | java.lang.String | clave privada |

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

