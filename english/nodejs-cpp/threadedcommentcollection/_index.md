---
title: ThreadedCommentCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the list of threaded comments.
type: docs
url: /nodejs-cpp/threadedcommentcollection/
---

## ThreadedCommentCollection class

Represents the list of threaded comments.

```javascript
class ThreadedCommentCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the threaded comment by the specific index. |
| [add(string, ThreadedCommentAuthor)](#add-string-threadedcommentauthor-)| Adds a threaded comment; |
| [getCount()](#getCount--)| Gets the number of elements contained in. |


### get(number) {#get-number-}

Gets the threaded comment by the specific index.

```javascript
get(index: number) : ThreadedComment;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index |

**Returns**

[ThreadedComment](/nodejs-cpp/threadedcomment/)

### add(string, ThreadedCommentAuthor) {#add-string-threadedcommentauthor-}

Adds a threaded comment;

```javascript
add(text: string, author: ThreadedCommentAuthor) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | string | The text of the threaded comment. |
| author | [ThreadedCommentAuthor](/nodejs-cpp/threadedcommentauthor/) | The author of the threaded comment |

### getCount() {#getCount--}

Gets the number of elements contained in.

```javascript
getCount() : number;
```



