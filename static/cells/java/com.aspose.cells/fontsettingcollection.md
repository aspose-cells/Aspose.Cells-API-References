##FontSettingCollection
Represents the list of .
**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class FontSettingCollection extends CollectionBase
```
Represents the list of [FontSetting](../../com.aspose.cells/fontsetting).
## Methods
| Method | Description |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Adds an item to the CollectionBase instance. |
| [appendText(String text)](#appendText-java.lang.String-) | Appends the text. |
| [clear()](#clear--) | Clear all setting. |
| [contains(Object o)](#contains-java.lang.Object-) | Return whether instance contains this object |
| [deleteText(int index, int count)](#deleteText-int-int-) | Delete some characters. |
| [equals(Object obj)](#equals-java.lang.Object-) |  |
| [format(int startIndex, int length, Font font, StyleFlag flag)](#format-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-) | Format the text with font setting. |
| [get(int index)](#get-int-) | Gets the [FontSetting](../../com.aspose.cells/fontsetting) by the index. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the number of elements contained in the CollectionBase instance. |
| [getHtmlString()](#getHtmlString--) | Gets the html string which contains data and some formats in this shape. |
| [getParagraphEnumerator()](#getParagraphEnumerator--) | Gets the enumerator of the paragraphs. |
| [getText()](#getText--) | Gets the text of the shape. |
| [getTextAlignment()](#getTextAlignment--) | Represents the alignment setting of the text body. |
| [getTextParagraphs()](#getTextParagraphs--) | Gets all paragraphs. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determines the index of a specific item in the CollectionBase instance. |
| [insertText(int index, String text)](#insertText-int-java.lang.String-) | Insert index at the position. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through the CollectionBase instance. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Removes the item at the specified index. |
| [replace(int index, int count, String text)](#replace-int-int-java.lang.String-) | Replace the text. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | Replace the text. |
| [setHtmlString(String value)](#setHtmlString-java.lang.String-) | Sets the html string which contains data and some formats in this shape. |
| [setText(String value)](#setText-java.lang.String-) | Sets the text of the shape. |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | Sets the preset WordArt style. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### appendText(String text) {#appendText-java.lang.String-}
```
public void appendText(String text)
```
Appends the text.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | java.lang.String | The text. |
### clear() {#clear--}
```
public void clear()
```
Clear all setting.
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
### deleteText(int index, int count) {#deleteText-int-int-}
```
public void deleteText(int index, int count)
```
Delete some characters.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The start index. |
| count | int | The count of characters. |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object |  |
**Returns:**
boolean -
### format(int startIndex, int length, Font font, StyleFlag flag) {#format-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-}
```
public void format(int startIndex, int length, Font font, StyleFlag flag)
```
Format the text with font setting.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | int | The start index. |
| length | int | The length. |
| font | [Font](../../com.aspose.cells/font) | The font. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | The flags of the font. |
### get(int index) {#get-int-}
```
public FontSetting get(int index)
```
Gets the [FontSetting](../../com.aspose.cells/fontsetting) by the index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index. |
**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) -
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
### getHtmlString() {#getHtmlString--}
```
public String getHtmlString()
```
Gets the html string which contains data and some formats in this shape.
**Returns:**
java.lang.String
### getParagraphEnumerator() {#getParagraphEnumerator--}
```
public Iterator getParagraphEnumerator()
```
Gets the enumerator of the paragraphs.
**Returns:**
java.util.Iterator -
### getText() {#getText--}
```
public String getText()
```
Gets the text of the shape.
**Returns:**
java.lang.String
### getTextAlignment() {#getTextAlignment--}
```
public ShapeTextAlignment getTextAlignment()
```
Represents the alignment setting of the text body.
**Returns:**
[ShapeTextAlignment](../../com.aspose.cells/shapetextalignment)
### getTextParagraphs() {#getTextParagraphs--}
```
public TextParagraphCollection getTextParagraphs()
```
Gets all paragraphs.
**Returns:**
[TextParagraphCollection](../../com.aspose.cells/textparagraphcollection)
### hashCode() {#hashCode--}
```
public int hashCode()
```
**Returns:**
int -
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
### insertText(int index, String text) {#insertText-int-java.lang.String-}
```
public void insertText(int index, String text)
```
Insert index at the position.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The start index. |
| text | java.lang.String | The text. |
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
### replace(int index, int count, String text) {#replace-int-int-java.lang.String-}
```
public void replace(int index, int count, String text)
```
Replace the text.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The start index. |
| count | int | The count of characters. |
| text | java.lang.String | The text. |
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public void replace(String oldValue, String newValue)
```
Replace the text.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| oldValue | java.lang.String | The old text. |
| newValue | java.lang.String | The new text. |
### setHtmlString(String value) {#setHtmlString-java.lang.String-}
```
public void setHtmlString(String value)
```
Sets the html string which contains data and some formats in this shape.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```
Sets the text of the shape.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setWordArtStyle(int style) {#setWordArtStyle-int-}
```
public void setWordArtStyle(int style)
```
Sets the preset WordArt style.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). The preset WordArt style. |
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
