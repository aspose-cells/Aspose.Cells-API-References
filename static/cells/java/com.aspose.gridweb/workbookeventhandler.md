##WorkbookEventHandler
Represents the interface that intend to handle workbook events.
**All Implemented Interfaces:**
java.io.Serializable
```
public interface WorkbookEventHandler extends Serializable
```
Represents the interface that intend to handle workbook events.
## Methods
| Method | Description |
| --- | --- |
| [handleCellEvent(Object sender, CellEventArgs e)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-) | handle the related Cell Event. |
### handleCellEvent(Object sender, CellEventArgs e) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-}
```
public abstract void handleCellEvent(Object sender, CellEventArgs e)
```
handle the related Cell Event.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sender | java.lang.Object | The source of the event. |
| e | [CellEventArgs](../../com.aspose.gridweb/celleventargs) | The event argument. |
