---
title: "IExportObjectListener"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Permite a los usuarios manipular objetos durante la exportación."
type: docs
url: /es/java/com.aspose.cells/iexportobjectlistener/
---
```
public interface IExportObjectListener
```

Permite a los usuarios manipular objetos durante la exportación.

**Example**

El siguiente ejemplo crea un Workbook, abre un archivo llamado designer.xls en él y hace que las barras de desplazamiento horizontal y vertical sean invisibles para el Workbook. Luego reemplaza dos valores de cadena con un valor entero y un valor de cadena respectivamente dentro de la hoja de cálculo y finalmente envía el archivo actualizado al navegador del cliente.

```
             class CustomExportObjectListener implements IExportObjectListener
             {
                 private int imgIdx = 0;
                 public Object exportObject(ExportObjectEvent e)
                 {
                     Object source = e.getSource();
                     if (source instanceof Shape)
                     {
                         Shape shape = (Shape)source;
                         String url = null;
                         switch (shape.getMsoDrawingType())
                         {
                             case MsoDrawingType.PICTURE:
                             {
                                 url = saveImage(((Picture)shape).getData(), imgIdx, ((Picture)shape).getImageType());
                                 break;
                              }
                         }
                         if (url != null)
                         {
                             imgIdx++;
                         }
                         return url;
                     }
                     return null;
                 }
                 private String saveImage(byte[] data, int imgIdx, /*ImageType*/int format)
                 {
                     //here save the image to any location, then return the url(relative or absolute) that the generated html can get the image
                     return "temp1/temp2.png";
                 }
              }
             //custom implementation of IExportObjectListener
 
                 //Save html file with custom listener
                 Workbook book = null; //build your workbook here
                 HtmlSaveOptions saveOptions = new HtmlSaveOptions();
                 saveOptions.setExportObjectListener(new CustomExportObjectListener());
                 java.io.InputStream stream = null; //build your stream here
                 book.save("res.html", saveOptions); //or here you can build your out put stream and save the workbook to stream
```
## Métodos

| Método | Descripción |
| --- | --- |
| [exportObject(ExportObjectEvent e)](#exportObject-com.aspose.cells.ExportObjectEvent-) | Exportar un objeto. |
### exportObject(ExportObjectEvent e) {#exportObject-com.aspose.cells.ExportObjectEvent-}
```
public abstract Object exportObject(ExportObjectEvent e)
```


Exportar un objeto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| e | [ExportObjectEvent](../../com.aspose.cells/exportobjectevent) | El evento que se dispara cuando se necesita exportar un objeto. |

**Returns:**
java.lang.Object - La información sobre el resultado de la exportación del objeto.

 *  For exporting objects when export workbook to HTML format, the result is URL string to access the saved Image from the html file which contains this exported object.
