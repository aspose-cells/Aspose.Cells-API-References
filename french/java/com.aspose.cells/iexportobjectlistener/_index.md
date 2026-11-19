---
title: "IExportObjectListener"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Permet aux utilisateurs de manipuler des objets lors de l'exportation."
type: docs
url: /fr/java/com.aspose.cells/iexportobjectlistener/
---
```
public interface IExportObjectListener
```

Permet aux utilisateurs de manipuler des objets lors de l'exportation.

**Example**

L'exemple suivant crée un Workbook, ouvre un fichier nommé designer.xls à l'intérieur et rend les barres de défilement horizontales et verticales invisibles pour le Workbook. Il remplace ensuite deux valeurs de chaîne par une valeur entière et une valeur de chaîne respectivement dans la feuille de calcul et envoie finalement le fichier mis à jour au navigateur du client.

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
## Méthodes

| Méthode | Description |
| --- | --- |
| [exportObject(ExportObjectEvent e)](#exportObject-com.aspose.cells.ExportObjectEvent-) | Exporter un objet. |
### exportObject(ExportObjectEvent e) {#exportObject-com.aspose.cells.ExportObjectEvent-}
```
public abstract Object exportObject(ExportObjectEvent e)
```


Exporter un objet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| e | [ExportObjectEvent](../../com.aspose.cells/exportobjectevent) | L'événement déclenché lorsqu'un objet doit être exporté. |

**Returns:**
java.lang.Object - Les informations sur le résultat de l'exportation de l'objet.

 *  For exporting objects when export workbook to HTML format, the result is URL string to access the saved Image from the html file which contains this exported object.
