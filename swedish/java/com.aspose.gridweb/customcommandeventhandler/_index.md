---
title: "CustomCommandEventHandler"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar gränssnittet som är avsett att hantera anpassade kommandohändelser."
type: docs
url: /sv/java/com.aspose.gridweb/customcommandeventhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CustomCommandEventHandler extends Serializable
```

Representerar gränssnittet som är avsett att hantera anpassade kommandohändelser.

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
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [handleCellEvent(Object sender, String command)](#handleCellEvent-java.lang.Object-java.lang.String-) | hantera den relaterade Cell-händelsen. |
### handleCellEvent(Object sender, String command) {#handleCellEvent-java.lang.Object-java.lang.String-}
```
public abstract void handleCellEvent(Object sender, String command)
```


hantera den relaterade Cell-händelsen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| avsändare | java.lang.Object | Källrutnätet för händelsen. Om händelsen utlöses av en cell i ett underordnat rutnät i hierarkiskt visningsläge, representerar parametern sender det underordnade rutnätet. |
| kommando | java.lang.String | Kommandosträngen som användaren skickar. |

