---
title: "CommentCollection Class"
linktitle: "CommentCollection"
articleTitle: "CommentCollection"
second_title: "Aspose.Cells for Python via Java"
description: "Encapsulates a collection of Comment objects."
type: docs
weight: 1060
url: /python-java/asposecells.api/commentcollection/
---

## CommentCollection class

Encapsulates a collection of Comment objects.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Count](#count) | int |  |
| [Item (int)](#itemint) | Comment | Gets the Comment element at the specified index. |
| [Item (java.lang.String)](#itemjavalangstring) | Comment | Gets the Comment element at the specified cell. |
| [Item (int, int)](#itemintint) | Comment | Gets the Comment element at the specified row index and column index. |

## Methods

| Name | Description |
| --- | --- |
| [addThreadedComment](#addthreadedcomment) | Adds a threaded comment. |
| [getThreadedComments](#getthreadedcomments) | Gets the threaded comments by row and column index. |
| [add](#add) | Adds a comment to the collection. |
| [removeAt](#removeat) | Removes the comment of the specific cell. |
| [clear](#clear) | Removes all comments; |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |
| [contains](#contains) | Reserved for internal use. |
| [indexOf](#indexof) | Reserved for internal use. |

### CommentCollection.Count property {#count}

**Type:** int

### CommentCollection.Item (int) property {#itemint}

Gets the Comment element at the specified index.

**Type:** Comment

### CommentCollection.Item (java.lang.String) property {#itemjavalangstring}

Gets the Comment element at the specified cell.

**Type:** Comment

### CommentCollection.Item (int, int) property {#itemintint}

Gets the Comment element at the specified row index and column index.

**Type:** Comment

### addThreadedComment(row, column, text, author) (1 of 2) {#addthreadedcomment}

Adds a threaded comment.

| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Cell row index. |
| column | int | Cell column index. |
| text | String | The text of the comment |
| author | ThreadedCommentAuthor | The user of this threaded comment. |

**Returns:** ThreadedComment object index.

---

### addThreadedComment(cellName, text, author) (2 of 2) {#addthreadedcomment-1}

Adds a threaded comment.

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | The name of the cell. |
| text | String | The text of the comment |
| author | ThreadedCommentAuthor | The user of this threaded comment. |

**Returns:** ThreadedComment object index.

### getThreadedComments(row, column) (1 of 2) {#getthreadedcomments}

Gets the threaded comments by row and column index.

| Parameter | Type | Description |
| --- | --- | --- |
| row | int | The row index. |
| column | int | The column index. |

---

### getThreadedComments(cellName) (2 of 2) {#getthreadedcomments-1}

Gets the threaded comments by cell name.

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | The name of the cell. |

### add(row, column) (1 of 3) {#add}

Adds a comment to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Cell row index. |
| column | int | Cell column index. |

**Returns:** Comment object index.

---

### add(cellName) (2 of 3) {#add-1}

Adds a comment to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Cell name. |

**Returns:** Comment object index.

---

### add(value) (3 of 3) {#add-2}

Reserved for internal use.

### removeAt(cellName) (1 of 3) {#removeat}

Removes the comment of the specific cell.

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | The name of cell which contains a comment. |

---

### removeAt(row, column) (2 of 3) {#removeat-1}

Removes the comment of the specific cell.

| Parameter | Type | Description |
| --- | --- | --- |
| row | int | The row index. |
| column | int | the column index. |

---

### removeAt(index) (3 of 3) {#removeat-2}

### clear() {#clear}

Removes all comments;

### iterator() {#iterator}

### get(index) {#get}

Reserved for internal use.

### contains(value) {#contains}

Reserved for internal use.

### indexOf(value) {#indexof}

Reserved for internal use.
