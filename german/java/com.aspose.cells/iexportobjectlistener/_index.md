---
title: "IExportObjectListener"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Ermöglicht Benutzern, Objekte beim Exportieren zu manipulieren."
type: docs
url: /de/java/com.aspose.cells/iexportobjectlistener/
---
```
public interface IExportObjectListener
```

Ermöglicht Benutzern, Objekte beim Exportieren zu manipulieren.

**Example**

Das folgende Beispiel erstellt ein Workbook, öffnet darin eine Datei namens designer.xls und macht die horizontalen und vertikalen Bildlaufleisten für das Workbook unsichtbar. Anschließend ersetzt es zwei Zeichenkettenwerte durch jeweils einen Integer‑Wert und einen Zeichenkettenwert im Tabellenblatt und sendet schließlich die aktualisierte Datei an den Browser des Clients.

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
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [exportObject(ExportObjectEvent e)](#exportObject-com.aspose.cells.ExportObjectEvent-) | Ein Objekt exportieren. |
### exportObject(ExportObjectEvent e) {#exportObject-com.aspose.cells.ExportObjectEvent-}
```
public abstract Object exportObject(ExportObjectEvent e)
```


Ein Objekt exportieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| e | [ExportObjectEvent](../../com.aspose.cells/exportobjectevent) | Das Ereignis, das ausgelöst wird, wenn ein Objekt exportiert werden muss. |

**Returns:**
java.lang.Object - Die Informationen über das Ergebnis des Objektexports.

 *  For exporting objects when export workbook to HTML format, the result is URL string to access the saved Image from the html file which contains this exported object.
