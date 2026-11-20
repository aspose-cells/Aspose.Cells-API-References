---
title: "CustomCommandEventHandler"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Schnittstelle dar, die dazu gedacht ist, Custom Command-Ereignisse zu behandeln."
type: docs
url: /de/java/com.aspose.gridweb/customcommandeventhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CustomCommandEventHandler extends Serializable
```

Stellt die Schnittstelle dar, die dazu gedacht ist, Custom Command-Ereignisse zu behandeln.

**Example**

```
         class MyCustomCommandEventHandler implements  CustomCommandEventHandler,Serializable{
          	 public void handleCellEvent(Object sender, String command){
                         GridWebBean gridweb=(GridWebBean)sender;
          			  GridWorksheet sheet = gridweb.getActiveSheet();
         	 //Identifying a specific button by checking its command
            if (command.equals("MyButton"))
             {
                 //Accessing the cells collection of the worksheet that is currently active
                 //Putting value to "A1" cell
                  sheet.getCells().get("A1").putValue("My Custom Command Button is Clicked.");
                // System.out.println("My Custom Command Button is Clicked:"+sheet.getName()+" "+sheet.getCells().get("A1").getValue());
             }	
         }
          }
         GridWebBean gridweb=ExtPage.getInstance().getBean();
         gridweb.CustomCommand = new MyCustomCommandEventHandler();
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [handleCellEvent(Object sender, String command)](#handleCellEvent-java.lang.Object-java.lang.String-) | Verarbeiten Sie das zugehörige Zellenereignis. |
### handleCellEvent(Object sender, String command) {#handleCellEvent-java.lang.Object-java.lang.String-}
```
public abstract void handleCellEvent(Object sender, String command)
```


Verarbeiten Sie das zugehörige Zellenereignis.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sender | java.lang.Object | Das Quell‑Raster des Ereignisses. Wenn das Ereignis von einer Zelle eines untergeordneten Rasters im hierarchischen Anzeigemodus ausgelöst wird, stellt der Parameter sender das untergeordnete Rasterobjekt dar. |
| command | java.lang.String | Der Befehlsstring, den der Benutzer sendet. |

