##RowColumnEventHandler
Represents the interface that intend to handle row/column events.
**All Implemented Interfaces:**
java.io.Serializable
```
public interface RowColumnEventHandler extends Serializable
```
Represents the interface that intend to handle row/column events.
## Methods
| Method | Description |
| --- | --- |
| [handleCellEvent(Object sender, RowColumnEventArgs e)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.RowColumnEventArgs-) | handle the related Cell Event. |
### handleCellEvent(Object sender, RowColumnEventArgs e) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.RowColumnEventArgs-}
```
public abstract void handleCellEvent(Object sender, RowColumnEventArgs e)
```
handle the related Cell Event.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sender | java.lang.Object | The source of the event. |
| e | [RowColumnEventArgs](../../com.aspose.gridweb/rowcolumneventargs) | The event argument. Call e.RejectOperation() if you want to cancel the deleting operation in RowDeleting or ColumnDeleting event handlers. |
