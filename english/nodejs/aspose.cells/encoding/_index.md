---
title: "Encoding"
linktitle: "Encoding"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents a character encoding."
type: docs
weight: 1290
url: /nodejs/aspose.cells/encoding/
---

## Encoding class

Represents a character encoding.

## Methods

| Name | Description |
| --- | --- |
| [equals(o)](#equals) | Determines whether the specified Object is equal to the current instance. |
| [equals(other)](#equals-1) | Determines whether the specified Encoding object is equal to the current instance. |
| [getASCII()](#getascii) *(static)* | Gets an encoding for the ASCII (7-bit) character set. |
| [getBigEndianUnicode()](#getbigendianunicode) *(static)* | Gets an encoding for the UTF-16 format using the big endian byte order. |
| [getDefault()](#getdefault) *(static)* | Gets an encoding for the operating system's current ANSI code page. |
| [getEncoding(codePage)](#getencoding) *(static)* | Returns the encoding associated with the specified code page identifier. |
| [getEncoding(charsetName)](#getencoding-1) *(static)* | Returns an encoding associated with the specified charset name. |
| [getEncoding(charset)](#getencoding-2) *(static)* | Returns an encoding associated with the specified charset object. |
| [getUTF7()](#getutf7) *(static)* | Gets an encoding for the UTF-7 format. |
| [getUTF8()](#getutf8) *(static)* | Gets an encoding for the UTF-8 format. |
| [getUTF8NoBOM()](#getutf8nobom) *(static)* | Gets an encoding for the UTF-8 format without the UTF-8 identifier. |
| [getUnicode()](#getunicode) *(static)* | Gets an encoding for the UTF-16 format using the little endian byte order. |

### equals(o) {#equals}

Determines whether the specified Object is equal to the current instance.

| Parameter | Type | Description |
| --- | --- | --- |
| o | Object | The Object to compare with the current instance. |

**Returns:** boolean — `boolean` true if value is an instance of Encoding and is equal to the current instance; otherwise, false.

### equals(other) {#equals-1}

Determines whether the specified Encoding object is equal to the current instance.

| Parameter | Type | Description |
| --- | --- | --- |
| other | Encoding | The Encoding object to compare with the current instance. |

**Returns:** boolean — `boolean` true if value is equal to the current instance; otherwise, false.

### getASCII() (static) {#getascii}

Gets an encoding for the ASCII (7-bit) character set.

**Returns:** Encoding — `Encoding` A Encoding object for the ASCII (7-bit) character set.

### getBigEndianUnicode() (static) {#getbigendianunicode}

Gets an encoding for the UTF-16 format using the big endian byte order.

**Returns:** Encoding — `Encoding` A Encoding object for the UTF-16 format using the big endian byte

### getDefault() (static) {#getdefault}

Gets an encoding for the operating system's current ANSI code page.

**Returns:** Encoding — `Encoding` An encoding for the operating system's current ANSI code page.

### getEncoding(codePage) (static) {#getencoding}

Returns the encoding associated with the specified code page identifier.

| Parameter | Type | Description |
| --- | --- | --- |
| codePage | Number | The code page identifier of the preferred encoding. -or- 0, to use the default encoding. |

**Returns:** Encoding — `Encoding` The Encoding object associated with the specified code page.

### getEncoding(charsetName) (static) {#getencoding-1}

Returns an encoding associated with the specified charset name.

| Parameter | Type | Description |
| --- | --- | --- |
| charsetName | String | specified charset name |

**Returns:** Encoding — `Encoding` The Encoding object associated with the specified charset name.

### getEncoding(charset) (static) {#getencoding-2}

Returns an encoding associated with the specified charset object.

| Parameter | Type | Description |
| --- | --- | --- |
| charset | Charset | specified charset object |

**Returns:** Encoding — `Encoding` The Encoding object associated with the specified charset object.

### getUTF7() (static) {#getutf7}

Gets an encoding for the UTF-7 format.

**Returns:** Encoding — `Encoding` A Encoding object for the UTF-7 format.

### getUTF8() (static) {#getutf8}

Gets an encoding for the UTF-8 format.

**Returns:** Encoding — `Encoding` A Encoding object for the UTF-8 format.

### getUTF8NoBOM() (static) {#getutf8nobom}

Gets an encoding for the UTF-8 format without the UTF-8 identifier.

**Returns:** Encoding — `Encoding` A Encoding object for the UTF-8 format without UTF-8 identifier.

### getUnicode() (static) {#getunicode}

Gets an encoding for the UTF-16 format using the little endian byte order.

**Returns:** Encoding — `Encoding` A Encoding object for the UTF-16 format using the little endian byte
