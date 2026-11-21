---
title: "CellEventHandler"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la interfaz que pretende manejar eventos de celda."
type: docs
url: /es/java/com.aspose.gridweb/celleventhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CellEventHandler extends Serializable
```

Representa la interfaz que pretende manejar eventos de celda.

**Example**

```
         class SortEventHandler implements   CellEventHandler,Serializable{
 
          	public void handleCellEvent(Object sender, CellEventArgs e) {
          		//System.out.println("handleCellEvent  ....");
          		GridWebBean gridweb=(GridWebBean)sender;
            		  GridWorksheet sheet = gridweb.getWorkSheets().get(0);
            		  GridWorksheet sheet1 = gridweb.getWorkSheets().get(1);
            		if (e.getArgument().toString().equals("A1")) {
            			sheet.getCells().sort(1, 0, 20, 4, 0, true,true,false);         
            		} else if (e.getArgument().toString().equals("B1")) {                   
            			sheet.getCells().sort(1, 0, 20, 4, 1, true,true,false);         
            		} else if (e.getArgument().toString().equals("C1")) {                   
            			sheet.getCells().sort(1, 0, 20, 4, 2, true,true,false);         
            		} else if (e.getArgument().toString().equals("D1")) {                   
            			sheet.getCells().sort(1, 0, 20, 4, 3, true,true,false);         
            		} else if (e.getArgument().toString().equals("1A1")) {                  
            			sheet1.getCells().sort(0, 1, 4, 7, 0, true,true,true);          
            		} else if (e.getArgument().toString().equals("1A2")) {                  
            			sheet1.getCells().sort(0, 1, 4, 7, 1, true,true,true);          
            		} else if (e.getArgument().toString().equals("1A3")) {                  
            			sheet1.getCells().sort(0, 1, 4, 7, 2, true,true,true);          
            		} else if (e.getArgument().toString().equals("1A4")) {                  
            			sheet1.getCells().sort(0, 1, 4, 7, 3, true,true,true);          
          		}
          	}
          }                                                                                      
         GridWebBean gridweb=ExtPage.getInstance().getBean();
         gridweb.CellCommand = new SortEventHandler();
```
## Métodos

| Método | Descripción |
| --- | --- |
| [handleCellEvent(Object sender, CellEventArgs e)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-) | manejar el evento de celda relacionado. |
### handleCellEvent(Object sender, CellEventArgs e) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-}
```
public abstract void handleCellEvent(Object sender, CellEventArgs e)
```


manejar el evento de celda relacionado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| remitente | java.lang.Object | La cuadrícula origen del evento. Si el evento se dispara por una celda de la cuadrícula hija en modo de visualización jerárquica, el parámetro sender representa el objeto de la cuadrícula hija. |
| e | [CellEventArgs](../../com.aspose.gridweb/celleventargs) | El argumento del evento. e.Cell es la celda que dispara el evento. e.Argument contiene el argumento del evento. |

