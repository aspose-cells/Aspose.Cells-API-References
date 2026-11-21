---
title: "CustomCommandEventHandler"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la interfaz que pretende manejar eventos de Comando Personalizado."
type: docs
url: /es/java/com.aspose.gridweb/customcommandeventhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CustomCommandEventHandler extends Serializable
```

Representa la interfaz que pretende manejar eventos de Comando Personalizado.

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
## Métodos

| Método | Descripción |
| --- | --- |
| [handleCellEvent(Object sender, String command)](#handleCellEvent-java.lang.Object-java.lang.String-) | manejar el evento de celda relacionado. |
### handleCellEvent(Object sender, String command) {#handleCellEvent-java.lang.Object-java.lang.String-}
```
public abstract void handleCellEvent(Object sender, String command)
```


manejar el evento de celda relacionado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| remitente | java.lang.Object | La cuadrícula origen del evento. Si el evento se dispara por una celda de la cuadrícula hija en modo de visualización jerárquica, el parámetro sender representa el objeto de la cuadrícula hija. |
| comando | java.lang.String | La cadena de comando que el usuario envía. |

