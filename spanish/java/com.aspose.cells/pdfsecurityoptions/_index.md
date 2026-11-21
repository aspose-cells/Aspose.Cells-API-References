---
title: "PdfSecurityOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Opciones para encriptar y permisos de acceso para un documento PDF."
type: docs
url: /es/java/com.aspose.cells/pdfsecurityoptions/
---

**Inheritance:**
java.lang.Object
```
public class PdfSecurityOptions
```

Opciones para cifrar y los permisos de acceso de un documento PDF. PDF/A no permite configuraciones de seguridad.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [PdfSecurityOptions()](#PdfSecurityOptions--) | El constructor de PdfSecurityOptions |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAccessibilityExtractContent()](#getAccessibilityExtractContent--) | Indica si se permite extraer texto y gráficos (para apoyar la accesibilidad a usuarios con discapacidades o para otros propósitos). |
| [getAnnotationsPermission()](#getAnnotationsPermission--) | Indica si se permite agregar o modificar anotaciones de texto, rellenar campos de formulario interactivo. |
| [getAssembleDocumentPermission()](#getAssembleDocumentPermission--) | Indica si se permite ensamblar el documento (insertar, rotar o eliminar páginas y crear marcadores o imágenes en miniatura), incluso si [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) está habilitado. |
| [getClass()](#getClass--) |  |
| [getExtractContentPermission()](#getExtractContentPermission--) | Indica si se permite copiar o extraer de otro modo texto y gráficos del documento mediante operaciones distintas a las controladas por [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--). |
| [getExtractContentPermissionObsolete()](#getExtractContentPermissionObsolete--) | Permiso para copiar o extraer contenido obsoleto según la referencia PDF. |
| [getFillFormsPermission()](#getFillFormsPermission--) | Indica si se permite rellenar campos de formulario interactivo existentes (incluidos los campos de firma), incluso si [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) está habilitado. |
| [getFullQualityPrintPermission()](#getFullQualityPrintPermission--) | Indica si se permite imprimir el documento a una representación a partir de la cual se pueda generar una copia digital fiel del contenido PDF. |
| [getModifyDocumentPermission()](#getModifyDocumentPermission--) | Indica si se permite modificar el contenido del documento mediante operaciones distintas a las controladas por [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) y [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--). |
| [getOwnerPassword()](#getOwnerPassword--) | Obtiene la contraseña del propietario para el documento PDF cifrado. |
| [getPrintPermission()](#getPrintPermission--) | Indica si se permite imprimir el documento. |
| [getUserPassword()](#getUserPassword--) | Obtiene la contraseña de usuario requerida para abrir el documento PDF cifrado. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAccessibilityExtractContent(boolean value)](#setAccessibilityExtractContent-boolean-) | Indica si se permite extraer texto y gráficos (para apoyar la accesibilidad a usuarios con discapacidades o para otros propósitos). |
| [setAnnotationsPermission(boolean value)](#setAnnotationsPermission-boolean-) | Indica si se permite agregar o modificar anotaciones de texto, rellenar campos de formulario interactivo. |
| [setAssembleDocumentPermission(boolean value)](#setAssembleDocumentPermission-boolean-) | Indica si se permite ensamblar el documento (insertar, rotar o eliminar páginas y crear marcadores o imágenes en miniatura), incluso si [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) está habilitado. |
| [setExtractContentPermission(boolean value)](#setExtractContentPermission-boolean-) | Indica si se permite copiar o extraer de otro modo texto y gráficos del documento mediante operaciones distintas a las controladas por [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--). |
| [setExtractContentPermissionObsolete(boolean value)](#setExtractContentPermissionObsolete-boolean-) | Permiso para copiar o extraer contenido obsoleto según la referencia PDF. |
| [setFillFormsPermission(boolean value)](#setFillFormsPermission-boolean-) | Indica si se permite rellenar campos de formulario interactivo existentes (incluidos los campos de firma), incluso si [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) está habilitado. |
| [setFullQualityPrintPermission(boolean value)](#setFullQualityPrintPermission-boolean-) | Indica si se permite imprimir el documento a una representación a partir de la cual se pueda generar una copia digital fiel del contenido PDF. |
| [setModifyDocumentPermission(boolean value)](#setModifyDocumentPermission-boolean-) | Indica si se permite modificar el contenido del documento mediante operaciones distintas a las controladas por [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) y [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--). |
| [setOwnerPassword(String value)](#setOwnerPassword-java.lang.String-) | Establece la contraseña del propietario para el documento PDF cifrado. |
| [setPrintPermission(boolean value)](#setPrintPermission-boolean-) | Indica si se permite imprimir el documento. |
| [setUserPassword(String value)](#setUserPassword-java.lang.String-) | Establece la contraseña de usuario requerida para abrir el documento PDF cifrado. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PdfSecurityOptions() {#PdfSecurityOptions--}
```
public PdfSecurityOptions()
```


El constructor de PdfSecurityOptions

**Example**

El siguiente código establece permiso de impresión de alta resolución para el PDF de salida.

```
         Workbook wb = new Workbook();
         wb.getWorksheets().get(0).getCells().get("A1").setValue("Aspose");
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
 
 
         PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();
 
         //set owner password
         pdfSecurityOptions.setOwnerPassword("YourOwnerPassword");
 
         //set user password
         pdfSecurityOptions.setUserPassword("YourUserPassword");
 
         //set print permisson
         pdfSecurityOptions.setPrintPermission(true);
 
         //set high resolution for print
         pdfSecurityOptions.setFullQualityPrintPermission(true);
 
 
         pdfSaveOptions.setSecurityOptions(pdfSecurityOptions);
 
         wb.save("output.pdf", pdfSaveOptions);
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
### getAccessibilityExtractContent() {#getAccessibilityExtractContent--}
```
public boolean getAccessibilityExtractContent()
```


Indica si se permite extraer texto y gráficos (para apoyar la accesibilidad a usuarios con discapacidades o para otros propósitos).

**Returns:**
boolean
### getAnnotationsPermission() {#getAnnotationsPermission--}
```
public boolean getAnnotationsPermission()
```


Indica si se permite agregar o modificar anotaciones de texto, rellenar campos de formulario interactivo.

**Remarks**

si [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) también está habilitado, cree o modifique campos de formulario interactivo (incluidos los campos de firma).

**Returns:**
boolean
### getAssembleDocumentPermission() {#getAssembleDocumentPermission--}
```
public boolean getAssembleDocumentPermission()
```


Indica si se permite ensamblar el documento (insertar, rotar o eliminar páginas y crear marcadores o imágenes en miniatura), incluso si [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) está habilitado.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getExtractContentPermission() {#getExtractContentPermission--}
```
public boolean getExtractContentPermission()
```


Indica si se permite copiar o extraer de otro modo texto y gráficos del documento mediante operaciones distintas a las controladas por [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--).

**Returns:**
boolean
### getExtractContentPermissionObsolete() {#getExtractContentPermissionObsolete--}
```
public boolean getExtractContentPermissionObsolete()
```


Permiso para copiar o extraer contenido obsoleto según la referencia PDF.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad ExtractContentPermission. Esta propiedad será eliminada 12 meses después, a partir de septiembre de 2023. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
boolean
### getFillFormsPermission() {#getFillFormsPermission--}
```
public boolean getFillFormsPermission()
```


Indica si se permite rellenar campos de formulario interactivo existentes (incluidos los campos de firma), incluso si [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) está habilitado.

**Returns:**
boolean
### getFullQualityPrintPermission() {#getFullQualityPrintPermission--}
```
public boolean getFullQualityPrintPermission()
```


Indica si se permite imprimir el documento a una representación a partir de la cual se pueda generar una copia digital fiel del contenido PDF.

**Remarks**

Cuando está habilitado (y [getPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getPrintPermission--) está establecido), la impresión se limita a una representación de bajo nivel de la apariencia, posiblemente de calidad degradada.

**Returns:**
boolean
### getModifyDocumentPermission() {#getModifyDocumentPermission--}
```
public boolean getModifyDocumentPermission()
```


Indica si se permite modificar el contenido del documento mediante operaciones distintas a las controladas por [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) y [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--).

**Returns:**
boolean
### getOwnerPassword() {#getOwnerPassword--}
```
public String getOwnerPassword()
```


Obtiene la contraseña del propietario para el documento PDF cifrado.

**Remarks**

La contraseña del propietario permite al usuario abrir un documento PDF cifrado sin ninguna restricción de acceso especificada.

**Returns:**
java.lang.String
### getPrintPermission() {#getPrintPermission--}
```
public boolean getPrintPermission()
```


Indica si se permite imprimir el documento.

**Remarks**

Posiblemente no al nivel de mayor calidad, dependiendo de si [getFullQualityPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFullQualityPrintPermission--) también está configurado.

**Returns:**
boolean
### getUserPassword() {#getUserPassword--}
```
public String getUserPassword()
```


Obtiene la contraseña de usuario requerida para abrir el documento PDF cifrado.

**Remarks**

Se requerirá la contraseña de propietario o la contraseña de usuario para abrir un documento PDF cifrado para su visualización.

La contraseña de usuario puede ser nula o una cadena vacía; en este caso no se requerirá ninguna contraseña al usuario al abrir el documento PDF.

Abrir el documento con la contraseña de propietario correcta permite acceso total al documento.

Abrir el documento con la contraseña de usuario correcta (o abrir un documento que no tiene contraseña de usuario) permite acceso limitado según los permisos especificados.

**Returns:**
java.lang.String
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




### setAccessibilityExtractContent(boolean value) {#setAccessibilityExtractContent-boolean-}
```
public void setAccessibilityExtractContent(boolean value)
```


Indica si se permite extraer texto y gráficos (para apoyar la accesibilidad a usuarios con discapacidades o para otros propósitos).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAnnotationsPermission(boolean value) {#setAnnotationsPermission-boolean-}
```
public void setAnnotationsPermission(boolean value)
```


Indica si se permite agregar o modificar anotaciones de texto, rellenar campos de formulario interactivo.

**Remarks**

si [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) también está habilitado, cree o modifique campos de formulario interactivo (incluidos los campos de firma).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAssembleDocumentPermission(boolean value) {#setAssembleDocumentPermission-boolean-}
```
public void setAssembleDocumentPermission(boolean value)
```


Indica si se permite ensamblar el documento (insertar, rotar o eliminar páginas y crear marcadores o imágenes en miniatura), incluso si [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) está habilitado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExtractContentPermission(boolean value) {#setExtractContentPermission-boolean-}
```
public void setExtractContentPermission(boolean value)
```


Indica si se permite copiar o extraer de otro modo texto y gráficos del documento mediante operaciones distintas a las controladas por [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExtractContentPermissionObsolete(boolean value) {#setExtractContentPermissionObsolete-boolean-}
```
public void setExtractContentPermissionObsolete(boolean value)
```


Permiso para copiar o extraer contenido obsoleto según la referencia PDF.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad ExtractContentPermission. Esta propiedad será eliminada 12 meses después, a partir de septiembre de 2023. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFillFormsPermission(boolean value) {#setFillFormsPermission-boolean-}
```
public void setFillFormsPermission(boolean value)
```


Indica si se permite rellenar campos de formulario interactivo existentes (incluidos los campos de firma), incluso si [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) está habilitado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFullQualityPrintPermission(boolean value) {#setFullQualityPrintPermission-boolean-}
```
public void setFullQualityPrintPermission(boolean value)
```


Indica si se permite imprimir el documento a una representación a partir de la cual se pueda generar una copia digital fiel del contenido PDF.

**Remarks**

Cuando está habilitado (y [getPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getPrintPermission--) está establecido), la impresión se limita a una representación de bajo nivel de la apariencia, posiblemente de calidad degradada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setModifyDocumentPermission(boolean value) {#setModifyDocumentPermission-boolean-}
```
public void setModifyDocumentPermission(boolean value)
```


Indica si se permite modificar el contenido del documento mediante operaciones distintas a las controladas por [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) y [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setOwnerPassword(String value) {#setOwnerPassword-java.lang.String-}
```
public void setOwnerPassword(String value)
```


Establece la contraseña del propietario para el documento PDF cifrado.

**Remarks**

La contraseña del propietario permite al usuario abrir un documento PDF cifrado sin ninguna restricción de acceso especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setPrintPermission(boolean value) {#setPrintPermission-boolean-}
```
public void setPrintPermission(boolean value)
```


Indica si se permite imprimir el documento.

**Remarks**

Posiblemente no al nivel de mayor calidad, dependiendo de si [getFullQualityPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFullQualityPrintPermission--) también está configurado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setUserPassword(String value) {#setUserPassword-java.lang.String-}
```
public void setUserPassword(String value)
```


Establece la contraseña de usuario requerida para abrir el documento PDF cifrado.

**Remarks**

Se requerirá la contraseña de propietario o la contraseña de usuario para abrir un documento PDF cifrado para su visualización.

La contraseña de usuario puede ser nula o una cadena vacía; en este caso no se requerirá ninguna contraseña al usuario al abrir el documento PDF.

Abrir el documento con la contraseña de propietario correcta permite acceso total al documento.

Abrir el documento con la contraseña de usuario correcta (o abrir un documento que no tiene contraseña de usuario) permite acceso limitado según los permisos especificados.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

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

