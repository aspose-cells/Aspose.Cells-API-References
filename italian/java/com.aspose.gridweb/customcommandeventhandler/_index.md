---
title: "CustomCommandEventHandler"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta l'interfaccia che intende gestire gli eventi di Comandi Personalizzati."
type: docs
url: /it/java/com.aspose.gridweb/customcommandeventhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CustomCommandEventHandler extends Serializable
```

Rappresenta l'interfaccia che intende gestire gli eventi di Comandi Personalizzati.

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
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [handleCellEvent(Object sender, String command)](#handleCellEvent-java.lang.Object-java.lang.String-) | Gestisci l'evento Cell correlato. |
### handleCellEvent(Object sender, String command) {#handleCellEvent-java.lang.Object-java.lang.String-}
```
public abstract void handleCellEvent(Object sender, String command)
```


Gestisci l'evento Cell correlato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sender | java.lang.Object | La griglia di origine dell'evento. Se l'evento è generato da una cella della griglia figlia in modalità di visualizzazione gerarchica, il parametro sender rappresenta l'oggetto della griglia figlia. |
| comando | java.lang.String | La stringa di comando inviata dall'utente. |

