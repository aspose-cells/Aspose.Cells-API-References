---
title: "CellEventHandler"
second_title: "Aspose.Cells for Java API Referansı"
description: "Hücre olaylarını ele almayı amaçlayan arayüzü temsil eder."
type: docs
url: /tr/java/com.aspose.gridweb/celleventhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CellEventHandler extends Serializable
```

Hücre olaylarını ele almayı amaçlayan arayüzü temsil eder.

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
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [handleCellEvent(Object sender, CellEventArgs e)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-) | İlgili Cell Event'i ele al. |
### handleCellEvent(Object sender, CellEventArgs e) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-}
```
public abstract void handleCellEvent(Object sender, CellEventArgs e)
```


İlgili Cell Event'i ele al.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sender | java.lang.Object | Olayın kaynak ızgarası. Olay, hiyerarşik gösterim modunda bir alt ızgara hücresi tarafından tetiklenirse, sender parametresi alt ızgara nesnesini temsil eder. |
| e | [CellEventArgs](../../com.aspose.gridweb/celleventargs) | Olay argümanı. e.Cell, olayı tetikleyen hücredir. e.Argument, olayın argümanını içerir. |

