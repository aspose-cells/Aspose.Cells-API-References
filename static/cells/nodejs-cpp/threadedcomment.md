##ThreadedComment
Represents the threaded comment.
## ThreadedComment class
Represents the threaded comment.
```javascript
class ThreadedComment;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [row](#row--)| number | Readonly. Gets the row index of the comment. |
| [column](#column--)| number | Readonly. Gets the column index of the comment. |
| [notes](#notes--)| string | Gets and sets the text of the comment. |
| [author](#author--)| ThreadedCommentAuthor | Gets the author of the comment. |
| [createdTime](#createdTime--)| Date | Gets and sets the created time of this threaded comment. |
## Methods
| Method | Description |
| --- | --- |
| [getRow()](#getRow--)| <b>@deprecated.</b> Please use the 'row' property instead. Gets the row index of the comment. |
| [getColumn()](#getColumn--)| <b>@deprecated.</b> Please use the 'column' property instead. Gets the column index of the comment. |
| [getNotes()](#getNotes--)| <b>@deprecated.</b> Please use the 'notes' property instead. Gets and sets the text of the comment. |
| [setNotes(string)](#setNotes-string-)| <b>@deprecated.</b> Please use the 'notes' property instead. Gets and sets the text of the comment. |
| [getAuthor()](#getAuthor--)| <b>@deprecated.</b> Please use the 'author' property instead. Gets the author of the comment. |
| [setAuthor(ThreadedCommentAuthor)](#setAuthor-threadedcommentauthor-)| <b>@deprecated.</b> Please use the 'author' property instead. Gets the author of the comment. |
| [getCreatedTime()](#getCreatedTime--)| <b>@deprecated.</b> Please use the 'createdTime' property instead. Gets and sets the created time of this threaded comment. |
| [setCreatedTime(Date)](#setCreatedTime-date-)| <b>@deprecated.</b> Please use the 'createdTime' property instead. Gets and sets the created time of this threaded comment. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### row {#row--}
Readonly. Gets the row index of the comment.
```javascript
row : number;
```
### column {#column--}
Readonly. Gets the column index of the comment.
```javascript
column : number;
```
### notes {#notes--}
Gets and sets the text of the comment.
```javascript
notes : string;
```
### author {#author--}
Gets the author of the comment.
```javascript
author : ThreadedCommentAuthor;
```
### createdTime {#createdTime--}
Gets and sets the created time of this threaded comment.
```javascript
createdTime : Date;
```
### getRow() {#getRow--}
```javascript
getRow() : number;
```
### getColumn() {#getColumn--}
```javascript
getColumn() : number;
```
### getNotes() {#getNotes--}
```javascript
getNotes() : string;
```
### setNotes(string) {#setNotes-string-}
```javascript
setNotes(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getAuthor() {#getAuthor--}
```javascript
getAuthor() : ThreadedCommentAuthor;
```
**Returns**
[ThreadedCommentAuthor](../threadedcommentauthor/)
### setAuthor(ThreadedCommentAuthor) {#setAuthor-threadedcommentauthor-}
```javascript
setAuthor(value: ThreadedCommentAuthor) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ThreadedCommentAuthor](../threadedcommentauthor/) | The value to set. |
### getCreatedTime() {#getCreatedTime--}
```javascript
getCreatedTime() : Date;
```
### setCreatedTime(Date) {#setCreatedTime-date-}
```javascript
setCreatedTime(value: Date) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Date | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
