---
title: ThreadedCommentAuthorCollection
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents all persons.
type: docs
url: /javascript-cpp/threadedcommentauthorcollection/
---

## ThreadedCommentAuthorCollection class

Represents all persons.

```javascript
class ThreadedCommentAuthorCollection;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [currentPerson](#currentPerson--)| ThreadedCommentAuthor | Gets and sets the current user. |

## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the person who create threaded comments. |
| [get(string)](#get-string-)| Gets the person who create threaded comments. |
| [indexOf(ThreadedCommentAuthor)](#indexOf-threadedcommentauthor-)| Gets the index of ThreadedCommentAuthor object |
| [add(string, string, string)](#add-string-string-string-)| Adds one thread comment person. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### currentPerson {#currentPerson--}

Gets and sets the current user.

```javascript
currentPerson : ThreadedCommentAuthor;
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

[ThreadedCommentAuthor](../threadedcommentauthor/)

### get(string) {#get-string-}

Gets the person who create threaded comments.

```javascript
get(name: string) : ThreadedCommentAuthor;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of the author. |

**Returns**

[ThreadedCommentAuthor](../threadedcommentauthor/)

### indexOf(ThreadedCommentAuthor) {#indexOf-threadedcommentauthor-}

Gets the index of ThreadedCommentAuthor object

```javascript
indexOf(author: ThreadedCommentAuthor) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| author | [ThreadedCommentAuthor](../threadedcommentauthor/) | The ThreadedCommentAuthor object |

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


