---
title: "CommentCollection"
linktitle: "CommentCollection"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Encapsulates a collection of Comment objects."
type: docs
weight: 740
url: /nodejs/aspose.cells/commentcollection/
---

## CommentCollection class

Encapsulates a collection of Comment objects.

## Methods

| Name | Description |
| --- | --- |
| [add(row, column)](#add) | Adds a comment to the collection. |
| [add(cellName)](#add-1) | Adds a comment to the collection. |
| [add()](#add-2) | Reserved for internal use. |
| [addThreadedComment(row, column, text, author)](#addthreadedcomment) | Adds a threaded comment. |
| [addThreadedComment(cellName, text, author)](#addthreadedcomment-1) | Adds a threaded comment. |
| [clear()](#clear) | Removes all comments; |
| [contains()](#contains) | Reserved for internal use. |
| [get(index)](#get) | Gets the Comment element at the specified index. |
| [get(cellName)](#get-1) | Gets the Comment element at the specified cell. |
| [get(row, column)](#get-2) | Gets the Comment element at the specified row index and column index. |
| [get()](#get-3) | Reserved for internal use. |
| [getCount()](#getcount) |  |
| [getThreadedComments(row, column)](#getthreadedcomments) | Gets the threaded comments by row and column index. |
| [getThreadedComments(cellName)](#getthreadedcomments-1) | Gets the threaded comments by cell name. |
| [indexOf()](#indexof) | Reserved for internal use. |
| [iterator()](#iterator) |  |
| [removeAt(cellName)](#removeat) | Removes the comment of the specific cell. |
| [removeAt(row, column)](#removeat-1) | Removes the comment of the specific cell. |
| [removeAt()](#removeat-2) |  |

### add(row, column) {#add}

Adds a comment to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Cell row index. |
| column | Number | Cell column index. |

**Returns:** Number — `Number` Comment object index.

### add(cellName) {#add-1}

Adds a comment to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Cell name. |

**Returns:** Number — `Number` Comment object index.

### add() {#add-2}

Reserved for internal use.

### addThreadedComment(row, column, text, author) {#addthreadedcomment}

Adds a threaded comment.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Cell row index. |
| column | Number | Cell column index. |
| text | String | The text of the comment |
| author | ThreadedCommentAuthor | The user of this threaded comment. |

**Returns:** Number — `Number` ThreadedComment object index.

### addThreadedComment(cellName, text, author) {#addthreadedcomment-1}

Adds a threaded comment.

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | The name of the cell. |
| text | String | The text of the comment |
| author | ThreadedCommentAuthor | The user of this threaded comment. |

**Returns:** Number — `Number` ThreadedComment object index.

### clear() {#clear}

Removes all comments;

### contains() {#contains}

Reserved for internal use.

### get(index) {#get}

Gets the Comment element at the specified index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The zero based index of the element. |

**Returns:** Comment — `Comment` The element at the specified index.

### get(cellName) {#get-1}

Gets the Comment element at the specified cell.

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Cell name. |

**Returns:** Comment — `Comment` The element at the specified cell.

### get(row, column) {#get-2}

Gets the Comment element at the specified row index and column index.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index. |
| column | Number | Column index. |

**Returns:** Comment — `Comment` The element at the specified cell.

### get() {#get-3}

Reserved for internal use.

### getCount() {#getcount}

### getThreadedComments(row, column) {#getthreadedcomments}

Gets the threaded comments by row and column index.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | The row index. |
| column | Number | The column index. |

**Returns:** ThreadedCommentCollection — `ThreadedCommentCollection`

### getThreadedComments(cellName) {#getthreadedcomments-1}

Gets the threaded comments by cell name.

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | The name of the cell. |

**Returns:** ThreadedCommentCollection — `ThreadedCommentCollection`

### indexOf() {#indexof}

Reserved for internal use.

### iterator() {#iterator}

### removeAt(cellName) {#removeat}

Removes the comment of the specific cell.

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | The name of cell which contains a comment. |

### removeAt(row, column) {#removeat-1}

Removes the comment of the specific cell.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | The row index. |
| column | Number | the column index. |

### removeAt() {#removeat-2}
