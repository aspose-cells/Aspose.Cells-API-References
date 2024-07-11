---
title: ThreadedCommentAuthorCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents all persons who .
type: docs
url: /nodejs-cpp/threadedcommentauthorcollection/
---

## ThreadedCommentAuthorCollection class

Represents all persons who .

```javascript
class ThreadedCommentAuthorCollection;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the person who create threaded comments. |
| [getCurrentPerson()](#getCurrentPerson--)| Gets and sets the current user. |
| [setCurrentPerson(ThreadedCommentAuthor)](#setCurrentPerson-threadedcommentauthor-)| Gets and sets the current user. |
| [indexOf(ThreadedCommentAuthor)](#indexOf-threadedcommentauthor-)| Gets the index of ThreadedCommentAuthor object |
| [add(string, string, string)](#add-string-string-string-)| Adds one thread comment person. |
| [getCount()](#getCount--)| Gets the number of elements contained in. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### get(number) {#get-number-}

Gets the person who create threaded comments.

```javascript
get(index: number) : ThreadedCommentAuthor;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index |

**Returns**

[ThreadedCommentAuthor](./threadedcommentauthor/)

### getCurrentPerson() {#getCurrentPerson--}

Gets and sets the current user.

```javascript
getCurrentPerson() : ThreadedCommentAuthor;
```


**Returns**

[ThreadedCommentAuthor](./threadedcommentauthor/)

### setCurrentPerson(ThreadedCommentAuthor) {#setCurrentPerson-threadedcommentauthor-}

Gets and sets the current user.

```javascript
setCurrentPerson(value: ThreadedCommentAuthor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ThreadedCommentAuthor](./threadedcommentauthor/) | The value to set. |

### indexOf(ThreadedCommentAuthor) {#indexOf-threadedcommentauthor-}

Gets the index of ThreadedCommentAuthor object

```javascript
indexOf(author: ThreadedCommentAuthor) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| author | [ThreadedCommentAuthor](./threadedcommentauthor/) | The ThreadedCommentAuthor object |

**Returns**

The index in the ThreadedCommentAuthor collection

### add(string, string, string) {#add-string-string-string-}

Adds one thread comment person.

```javascript
add(name: string, userId: string, providerId: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of the person. |
| userId | string |  |
| providerId | string | The id of the provider |

### getCount() {#getCount--}

Gets the number of elements contained in.

```javascript
getCount() : number;
```



