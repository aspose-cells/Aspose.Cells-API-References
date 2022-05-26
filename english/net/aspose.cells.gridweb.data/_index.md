---
title: Aspose.Cells.GridWeb.Data
second_title: Aspose.Cells for .NET API Reference
description: The namespace of basic data represented classes of GridWeb.
type: docs
weight: 20
url: /net/aspose.cells.gridweb.data/
---
The namespace of basic data represented classes of GridWeb.

## Classes

| Class | Description |
| --- | --- |
| [CellErrorHandler](./cellerrorhandler) | Represents the interface that intend to handle cell error events. |
| [CellEventHandler](./celleventhandler) | Represents the interface that intend to handle cell events. |
| [CellEventStringHandler](./celleventstringhandler) | Represents the method that intend to handle cell events. same as CellEventHandler interface,but return string result |
| [CellImage](./cellimage) |  |
| [CustomCommandEventHandler](./customcommandeventhandler) | Represents the interface that intend to handle Custom Command events. |
| [GridAbstractCalculationEngine](./gridabstractcalculationengine) | Represents user's custom calculation engine to extend the default calculation engine of Aspose.Cells. |
| [GridCalculationData](./gridcalculationdata) | Represents the required data when calculating one function, such as function name, parameters, ...etc. |
| [GridCell](./gridcell) | Represents a cell object. |
| [GridCellArea](./gridcellarea) | Represents an area of cells. |
| [GridCellException](./gridcellexception) | Represents a cell operation error. |
| [GridCells](./gridcells) | Encapsulates a collection of Cell objects. |
| [GridColumn](./gridcolumn) | Represents a single column in a worksheet. |
| [GridColumnCollection](./gridcolumncollection) | Collects the  objects that represent the individual columns in a worksheet. |
| [GridComment](./gridcomment) | Encapsulates the object that represents a cell comment. |
| [GridCommentCollection](./gridcommentcollection) | Encapsulates a collection of Comment objects. |
| [GridHtmlSaveOptions](./gridhtmlsaveoptions) | Represents the options for saving html file. |
| [GridHyperlink](./gridhyperlink) | Encapsulates the object that represents a hyperlink. |
| [GridHyperlinkCollection](./gridhyperlinkcollection) | Encapsulates a collection of Hyperlink objects. |
| [GridName](./gridname) | Encapsulates the object that represents a name object. |
| [GridNameCollection](./gridnamecollection) | Encapsulates a collection of Name objects. |
| [GridPicture](./gridpicture) | Encapsulates the object that represents a single picture in a spreadsheet. |
| [GridPictureCollection](./gridpicturecollection) | Encapsulates a collection of Picture objects. |
| [GridPivotField](./gridpivotfield) | Represents a field in a PivotTable report. |
| [GridPivotFieldCollection](./gridpivotfieldcollection) | Encapsulates a collection of PivotField objects. |
| [GridPivotItem](./gridpivotitem) | Represents a item in a PivotField report. |
| [GridPivotItemCollection](./gridpivotitemcollection) | Encapsulates a collection of PivotItem objects. |
| [GridPivotTable](./gridpivottable) | Represents a PivotTable report on a worksheet. The PivotTable object is a member of the PivotTables collection. The PivotTables collection contains all the PivotTable objects on a control. |
| [GridPivotTableCollection](./gridpivottablecollection) | Encapsulates a collection of PivotTable objects. |
| [GridReferredArea](./gridreferredarea) | Represents a referred objcet by the formula. |
| [GridRow](./gridrow) | Encapsulates the object that represents a single picture in a spreadsheet. |
| [GridRowCollection](./gridrowcollection) | Encapsulates a collection of [`GridRow`](../aspose.cells.gridweb.data/gridrow) objects. |
| [GridSaveOptions](./gridsaveoptions) | Represents all save options |
| [GridShape](./gridshape) | Represents a shape object. |
| [GridShapeCollection](./gridshapecollection) | Encapsulates a collection of [`GridShape`](../aspose.cells.gridweb.data/gridshape) objects. |
| [GridValidation](./gridvalidation) | Represents data validation.settings. |
| [GridValidationCollection](./gridvalidationcollection) | Encapsulates a collection of [`GridValidation`](../aspose.cells.gridweb.data/gridvalidation) objects. |
| [GridWebException](./gridwebexception) | The exception that is thrown when Aspose.Cells.GridWeb specified error occurs. |
| [GridWorkbook](./gridworkbook) | Represents a root object to create an Excel spreadsheet. |
| [GridWorkbookSettings](./gridworkbooksettings) | Represents settings of the workbook. |
| [GridWorksheet](./gridworksheet) | Encapsulates the object that represents a single worksheet. |
| [GridWorksheetCollection](./gridworksheetcollection) | Collects the  objects that represent the individual rows in a worksheet. |
| [InitializeNewBindRowHandler](./initializenewbindrowhandler) | Represents the method that intend to handle InitializeNewBindRow event. sender: The worksheet object. bindObject: The new created bind object. Generally it's a DataRowView object. |
| [OnErrorActionQuery](./onerroractionquery) | Used in the CellError event of the GridWeb. |
| [RowColumnEventHandler](./rowcolumneventhandler) | Represents the interface that intend to handle row/column events. |
| [SheetEventHandler](./sheeteventhandler) | Represents the interface that intend to handle sheet events. |
| [WebCellException](./webcellexception) | Represents a cell operation error. |
| [WorkbookEventHandler](./workbookeventhandler) | Represents the interface that intend to handle workbook events. |
## Interfaces

| Interface | Description |
| --- | --- |
| [GridCustomServerValidation](./gridcustomservervalidation) | the interface you need to implement when use server side validation. CustomServerFunction. |
| [ICustomFilter](./icustomfilter) | Summary description for ICustomFilter. |
## Enumeration

| Enumeration | Description |
| --- | --- |
| [GridCellErrorType](./gridcellerrortype) | Used in WebCellException. Represents the cell error type. |
| [GridImageType](./gridimagetype) | Specifies the type (format) of an image. |
| [GridMsoDrawingType](./gridmsodrawingtype) | Represents office drawing objects type. |
| [GridOperatorType](./gridoperatortype) | Represents the operator type of conditional format and data validation. |
| [GridPivotFieldFunction](./gridpivotfieldfunction) | Represents consolidation function. |
| [GridPivotFieldType](./gridpivotfieldtype) | Represents PivotTable field type. |
| [GridSaveFormat](./gridsaveformat) | Enumerates supported file format types. |
| [GridShiftType](./gridshifttype) | Represent the shift options when deleting a range of cells. |
| [GridValidationType](./gridvalidationtype) | Represents data validation type. |
| [HyperlinkActionType](./hyperlinkactiontype) | Hyperlink has two action type: UrlLink and CellCommand. UrlLink type hyperlink is an anchor in a cell, click it will navigate to another page or open a new browser window. CellCommand type hyperlink is an command button in a cell, click it will generate a server side event. |
| [NumberType](./numbertype) | Represents the number or datetime format type. |
| [OnErrorActionType](./onerroractiontype) | Used in CellError event of the GridWeb. User set the OnErrorActionQuery.OnErrorAction to tell the control Stop processing or Ignore error. |
| [PivotFieldSort](./pivotfieldsort) | Represents the order used to sort the specified PivotTable field. |
| [PivotSourceType](./pivotsourcetype) | Represents the source data type. |
| [SortOrder](./sortorder) | Represents what order the data sort by. |
| [SortOrientation](./sortorientation) | Represents sorting orientation |
| [SubtotalFunction](./subtotalfunction) | Represents subtotal function type. Used in the GridWorksheet.CreateSubtotal method. |
| [WebCellErrorType](./webcellerrortype) | Used in WebCellException. Represents the cell error type. |

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
