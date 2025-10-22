##CommentCollection
Encapsulates a collection of  objects.
**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class CommentCollection extends CollectionBase
```
Encapsulates a collection of [Comment](../../com.aspose.cells/comment) objects.
**Example**
```
Workbook workbook = new Workbook();
CommentCollection comments = workbook.getWorksheets().get(0).getComments();
//do your business
```
## Methods
| Method | Description |
| --- | --- |
| [add(int row, int column)](#add-int-int-) | Adds a comment to the collection. |
| [add(Object o)](#add-java.lang.Object-) | Adds an item to the CollectionBase instance. |
| [add(String cellName)](#add-java.lang.String-) | Adds a comment to the collection. |
| [addThreadedComment(int row, int column, String text, ThreadedCommentAuthor author)](#addThreadedComment-int-int-java.lang.String-com.aspose.cells.ThreadedCommentAuthor-) | Adds a threaded comment. |
| [addThreadedComment(String cellName, String text, ThreadedCommentAuthor author)](#addThreadedComment-java.lang.String-java.lang.String-com.aspose.cells.ThreadedCommentAuthor-) | Adds a threaded comment. |
| [clear()](#clear--) | Removes all comments; |
| [contains(Object o)](#contains-java.lang.Object-) | Return whether instance contains this object |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the [Comment](../../com.aspose.cells/comment) element at the specified index. |
| [get(int row, int column)](#get-int-int-) | Gets the [Comment](../../com.aspose.cells/comment) element at the specified row index and column index. |
| [get(String cellName)](#get-java.lang.String-) | Gets the [Comment](../../com.aspose.cells/comment) element at the specified cell. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the number of elements contained in the CollectionBase instance. |
| [getThreadedComments(int row, int column)](#getThreadedComments-int-int-) | Gets the threaded comments by row and column index. |
| [getThreadedComments(String cellName)](#getThreadedComments-java.lang.String-) | Gets the threaded comments by cell name. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determines the index of a specific item in the CollectionBase instance. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through the CollectionBase instance. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Removes the item at the specified index. |
| [removeAt(int row, int column)](#removeAt-int-int-) | Removes the comment of the specific cell. |
| [removeAt(String cellName)](#removeAt-java.lang.String-) | Removes the comment of the specific cell. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int row, int column) {#add-int-int-}
```
public int add(int row, int column)
```
Adds a comment to the collection.
**Example**
```
int commentIndex1 = comments.add(0, 0);
Comment comment1 = comments.get(commentIndex1);
comment1.setNote("First note.");
comment1.getFont().setName("Times New Roman");
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Cell row index. |
| column | int | Cell column index. |
**Returns:**
int - [Comment](../../com.aspose.cells/comment) object index.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```
Adds an item to the CollectionBase instance.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | The Object to add to the CollectionBase instance. |
**Returns:**
int - The position into which the new element was inserted.
### add(String cellName) {#add-java.lang.String-}
```
public int add(String cellName)
```
Adds a comment to the collection.
**Example**
```
int commentIndex2 = comments.add("B2");
Comment comment2 = comments.get(commentIndex2);
comment2.setNote("Second note.");
comment2.getFont().setName("Times New Roman");
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | Cell name. |
**Returns:**
int - [Comment](../../com.aspose.cells/comment) object index.
### addThreadedComment(int row, int column, String text, ThreadedCommentAuthor author) {#addThreadedComment-int-int-java.lang.String-com.aspose.cells.ThreadedCommentAuthor-}
```
public int addThreadedComment(int row, int column, String text, ThreadedCommentAuthor author)
```
Adds a threaded comment.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Cell row index. |
| column | int | Cell column index. |
| text | java.lang.String | The text of the comment |
| author | [ThreadedCommentAuthor](../../com.aspose.cells/threadedcommentauthor) | The user of this threaded comment. |
**Returns:**
int - [ThreadedComment](../../com.aspose.cells/threadedcomment) object index.
### addThreadedComment(String cellName, String text, ThreadedCommentAuthor author) {#addThreadedComment-java.lang.String-java.lang.String-com.aspose.cells.ThreadedCommentAuthor-}
```
public int addThreadedComment(String cellName, String text, ThreadedCommentAuthor author)
```
Adds a threaded comment.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | The name of the cell. |
| text | java.lang.String | The text of the comment |
| author | [ThreadedCommentAuthor](../../com.aspose.cells/threadedcommentauthor) | The user of this threaded comment. |
**Returns:**
int - [ThreadedComment](../../com.aspose.cells/threadedcomment) object index.
### clear() {#clear--}
```
public void clear()
```
Removes all comments;
**Example**
```
comments.clear();
```
### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```
Return whether instance contains this object
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | test object |
**Returns:**
boolean - Whether instance contains this object
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
### get(int index) {#get-int-}
```
public Comment get(int index)
```
Gets the [Comment](../../com.aspose.cells/comment) element at the specified index.
**Example**
```
Comment comment3 = comments.get(0);
comment3.setNote("Three note.");
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero based index of the element. |
**Returns:**
[Comment](../../com.aspose.cells/comment) - The element at the specified index.
### get(int row, int column) {#get-int-int-}
```
public Comment get(int row, int column)
```
Gets the [Comment](../../com.aspose.cells/comment) element at the specified row index and column index.
**Example**
```
Comment comment5 = comments.get(1,1);
comment5.setNote("Five note.");
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index. |
| column | int | Column index. |
**Returns:**
[Comment](../../com.aspose.cells/comment) - The element at the specified cell.
### get(String cellName) {#get-java.lang.String-}
```
public Comment get(String cellName)
```
Gets the [Comment](../../com.aspose.cells/comment) element at the specified cell.
**Example**
```
Comment comment4 = comments.get("B2");
comment4.setNote("Four note.");
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | Cell name. |
**Returns:**
[Comment](../../com.aspose.cells/comment) - The element at the specified cell.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```
Gets the number of elements contained in the CollectionBase instance.
**Returns:**
int - The number of elements contained in the CollectionBase instance.
### getThreadedComments(int row, int column) {#getThreadedComments-int-int-}
```
public ThreadedCommentCollection getThreadedComments(int row, int column)
```
Gets the threaded comments by row and column index.
**Example**
```
ThreadedCommentCollection threadedComments1 = comments.getThreadedComments(1, 1);
for (int i = 0; i <threadedComments1.getCount(); ++i)
{
ThreadedComment tc = threadedComments1.get(i);
String note = tc.getNotes();
}
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | The row index. |
| column | int | The column index. |
**Returns:**
[ThreadedCommentCollection](../../com.aspose.cells/threadedcommentcollection) -
### getThreadedComments(String cellName) {#getThreadedComments-java.lang.String-}
```
public ThreadedCommentCollection getThreadedComments(String cellName)
```
Gets the threaded comments by cell name.
**Example**
```
ThreadedCommentCollection threadedComments2 = comments.getThreadedComments("B2");
for (int i = 0; i <threadedComments2.getCount(); ++i)
{
ThreadedComment tc = threadedComments2.get(i);
String note = tc.getNotes();
}
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | The name of the cell. |
**Returns:**
[ThreadedCommentCollection](../../com.aspose.cells/threadedcommentcollection) -
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```
Determines the index of a specific item in the CollectionBase instance.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | Determines the index of a specific item in the CollectionBase instance. |
**Returns:**
int - The index of value if found in the list; otherwise, -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```
Returns an enumerator that iterates through the CollectionBase instance.
**Returns:**
java.util.Iterator - An iterator for the CollectionBase instance.
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```
Removes the item at the specified index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero-based index of the item to remove. |
### removeAt(int row, int column) {#removeAt-int-int-}
```
public void removeAt(int row, int column)
```
Removes the comment of the specific cell.
**Example**
```
comments.removeAt(1,1);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | The row index. |
| column | int | the column index. |
### removeAt(String cellName) {#removeAt-java.lang.String-}
```
public void removeAt(String cellName)
```
Removes the comment of the specific cell.
**Example**
```
comments.removeAt("B2");
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | The name of cell which contains a comment. |
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
