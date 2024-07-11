---
title: CommentCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates a collection of [Comment](./comment/) objects.
type: docs
url: /nodejs-cpp/commentcollection/
---

## CommentCollection class

Encapsulates a collection of [Comment](./comment/) objects.

```javascript
class CommentCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [Comment](./comment/) element at the specified index. |
| [addThreadedComment(number, number, string, ThreadedCommentAuthor)](#addThreadedComment-number-number-string-threadedcommentauthor-)| Adds a threaded comment. |
| [addThreadedComment(string, string, ThreadedCommentAuthor)](#addThreadedComment-string-string-threadedcommentauthor-)| Adds a threaded comment. |
| [getThreadedComments(number, number)](#getThreadedComments-number-number-)| Gets the threaded comments by row and column index. |
| [getThreadedComments(string)](#getThreadedComments-string-)| Gets the threaded comments by cell name. |
| [add(number, number)](#add-number-number-)| Adds a comment to the collection. |
| [add(string)](#add-string-)| Adds a comment to the collection. |
| [removeAt(string)](#removeAt-string-)| Removes the comment of the specific cell. |
| [removeAt(number, number)](#removeAt-number-number-)| Removes the comment of the specific cell. |
| [clear()](#clear--)| Removes all comments; |
| [getCount()](#getCount--)| Gets the number of elements contained in. |


### get(number) {#get-number-}

Gets the [Comment](./comment/) element at the specified index.

```javascript
get(index: number) : Comment;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |

**Returns**

The element at the specified index.

### addThreadedComment(number, number, string, ThreadedCommentAuthor) {#addThreadedComment-number-number-string-threadedcommentauthor-}

Adds a threaded comment.

```javascript
addThreadedComment(row: number, column: number, text: string, author: ThreadedCommentAuthor) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | Cell row index. |
| column | number | Cell column index. |
| text | string | The text of the comment |
| author | [ThreadedCommentAuthor](./threadedcommentauthor/) | The user of this threaded comment. |

**Returns**

[ThreadedComment](./threadedcomment/) object index.

### addThreadedComment(string, string, ThreadedCommentAuthor) {#addThreadedComment-string-string-threadedcommentauthor-}

Adds a threaded comment.

```javascript
addThreadedComment(cellName: string, text: string, author: ThreadedCommentAuthor) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | string | The name of the cell. |
| text | string | The text of the comment |
| author | [ThreadedCommentAuthor](./threadedcommentauthor/) | The user of this threaded comment. |

**Returns**

[ThreadedComment](./threadedcomment/) object index.

### getThreadedComments(number, number) {#getThreadedComments-number-number-}

Gets the threaded comments by row and column index.

```javascript
getThreadedComments(row: number, column: number) : ThreadedCommentCollection;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | The row index. |
| column | number | The column index. |

**Returns**

[ThreadedCommentCollection](./threadedcommentcollection/)

### getThreadedComments(string) {#getThreadedComments-string-}

Gets the threaded comments by cell name.

```javascript
getThreadedComments(cellName: string) : ThreadedCommentCollection;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | string | The name of the cell. |

**Returns**

[ThreadedCommentCollection](./threadedcommentcollection/)

### add(number, number) {#add-number-number-}

Adds a comment to the collection.

```javascript
add(row: number, column: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | Cell row index. |
| column | number | Cell column index. |

**Returns**

[Comment](./comment/) object index.

### add(string) {#add-string-}

Adds a comment to the collection.

```javascript
add(cellName: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | string | Cell name. |

**Returns**

[Comment](./comment/) object index.

### removeAt(string) {#removeAt-string-}

Removes the comment of the specific cell.

```javascript
removeAt(cellName: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | string | The name of cell which contains a comment. |

### removeAt(number, number) {#removeAt-number-number-}

Removes the comment of the specific cell.

```javascript
removeAt(row: number, column: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | The row index. |
| column | number | the column index. |

### clear() {#clear--}

Removes all comments;

```javascript
clear() : void;
```


### getCount() {#getCount--}

Gets the number of elements contained in.

```javascript
getCount() : number;
```



