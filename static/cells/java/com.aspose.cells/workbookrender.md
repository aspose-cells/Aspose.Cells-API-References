##WorkbookRender
Represents a Workbook render.
**Inheritance:**
java.lang.Object
```
public class WorkbookRender
```
Represents a Workbook render. The constructor of this class , must be used after modification of pagesetup, cell style.
**Remarks**
## Constructors
| Constructor | Description |
| --- | --- |
| [WorkbookRender(Workbook workbook, ImageOrPrintOptions options)](#WorkbookRender-com.aspose.cells.Workbook-com.aspose.cells.ImageOrPrintOptions-) | The construct of WorkbookRender |
## Methods
| Method | Description |
| --- | --- |
| [dispose()](#dispose--) | Releases resources created and used for rendering. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPageCount()](#getPageCount--) | Gets the total page count of workbook. |
| [getPageSizeInch(int pageIndex)](#getPageSizeInch-int-) | Get page size in inch of output image. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toImage(int pageIndex, InputStream stream)](#toImage-int-java.io.InputStream-) | Render certain page to a stream. |
| [toImage(int pageIndex, OutputStream stream)](#toImage-int-java.io.OutputStream-) | Render certain page to a stream. |
| [toImage(int pageIndex, String fileName)](#toImage-int-java.lang.String-) | Render certain page to a file. |
| [toImage(OutputStream stream)](#toImage-java.io.OutputStream-) | Render whole workbook as Tiff Image to stream. |
| [toImage(String filename)](#toImage-java.lang.String-) | Render whole workbook as Tiff Image to a file. |
| [toPrinter(String printerName)](#toPrinter-java.lang.String-) | Render workbook to Printer |
| [toPrinter(String printerName, int printPageIndex, int printPageCount)](#toPrinter-java.lang.String-int-int-) | Render workbook to Printer |
| [toPrinter(String printerName, String jobName)](#toPrinter-java.lang.String-java.lang.String-) | Render workbook to Printer |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorkbookRender(Workbook workbook, ImageOrPrintOptions options) {#WorkbookRender-com.aspose.cells.Workbook-com.aspose.cells.ImageOrPrintOptions-}
```
public WorkbookRender(Workbook workbook, ImageOrPrintOptions options)
```
The construct of WorkbookRender
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | Indicate which workbook to be rendered. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | ImageOrPrintOptions contains some property of output image |
### dispose() {#dispose--}
```
public void dispose()
```
Releases resources created and used for rendering.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |
**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getPageCount() {#getPageCount--}
```
public int getPageCount()
```
Gets the total page count of workbook.
**Returns:**
int
### getPageSizeInch(int pageIndex) {#getPageSizeInch-int-}
```
public float[] getPageSizeInch(int pageIndex)
```
Get page size in inch of output image.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | int | The page index is based on zero. |
**Returns:**
float[] - Page size of image, [0] for width and [1] for height
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### toImage(int pageIndex, InputStream stream) {#toImage-int-java.io.InputStream-}
```
public void toImage(int pageIndex, InputStream stream)
```
Render certain page to a stream.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | int | indicate which page is to be converted |
| stream | java.io.InputStream | the stream of the output image |
### toImage(int pageIndex, OutputStream stream) {#toImage-int-java.io.OutputStream-}
```
public void toImage(int pageIndex, OutputStream stream)
```
Render certain page to a stream.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | int | indicate which page is to be converted |
| stream | java.io.OutputStream | the stream of the output image |
### toImage(int pageIndex, String fileName) {#toImage-int-java.lang.String-}
```
public void toImage(int pageIndex, String fileName)
```
Render certain page to a file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | int | indicate which page is to be converted |
| fileName | java.lang.String | filename of the output image |
### toImage(OutputStream stream) {#toImage-java.io.OutputStream-}
```
public void toImage(OutputStream stream)
```
Render whole workbook as Tiff Image to stream.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | the stream of the output image |
### toImage(String filename) {#toImage-java.lang.String-}
```
public void toImage(String filename)
```
Render whole workbook as Tiff Image to a file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | the filename of the output image |
### toPrinter(String printerName) {#toPrinter-java.lang.String-}
```
public void toPrinter(String printerName)
```
Render workbook to Printer
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String | the name of the printer , for example: "Microsoft Office Document Image Writer" |
### toPrinter(String printerName, int printPageIndex, int printPageCount) {#toPrinter-java.lang.String-int-int-}
```
public void toPrinter(String printerName, int printPageIndex, int printPageCount)
```
Render workbook to Printer
**Remarks**
NOTE: This method is now obsolete. Instead, please use ToPrinter(string PrinterName) and ImageOrPrintOptions.PageIndex, PageCount to set the first page and the number of pages to print. This property will be removed 12 months later since December 2021. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String | the name of the printer , for example: "Microsoft Office Document Image Writer" |
| printPageIndex | int | the 0-based index of the first page to print, it must be in Range [0, WorkbookRender.PageCount-1] |
| printPageCount | int | the number of pages to print, it must be greater than zero |
### toPrinter(String printerName, String jobName) {#toPrinter-java.lang.String-java.lang.String-}
```
public void toPrinter(String printerName, String jobName)
```
Render workbook to Printer
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String | the name of the printer , for example: "Microsoft Office Document Image Writer" |
| jobName | java.lang.String | set the print job name |
### toString() {#toString--}
```
public String toString()
```
**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```
### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |
