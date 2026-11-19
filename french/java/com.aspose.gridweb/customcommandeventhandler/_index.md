---
title: "CustomCommandEventHandler"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente l'interface qui a pour but de gérer les événements Custom Command."
type: docs
url: /fr/java/com.aspose.gridweb/customcommandeventhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CustomCommandEventHandler extends Serializable
```

Représente l'interface qui a pour but de gérer les événements Custom Command.

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
## Méthodes

| Méthode | Description |
| --- | --- |
| [handleCellEvent(Object sender, String command)](#handleCellEvent-java.lang.Object-java.lang.String-) | gérer l'événement Cell associé. |
### handleCellEvent(Object sender, String command) {#handleCellEvent-java.lang.Object-java.lang.String-}
```
public abstract void handleCellEvent(Object sender, String command)
```


gérer l'événement Cell associé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sender | java.lang.Object | La grille source de l'événement. Si l'événement est déclenché par la cellule d'une grille enfant en mode d'affichage hiérarchique, le paramètre sender représente l'objet de la grille enfant. |
| commande | java.lang.String | La chaîne de commande envoyée par l'utilisateur. |

