##Outline
Represents an outline on a worksheet.
## Outline class
Represents an outline on a worksheet.
```javascript
class Outline;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [summaryRowBelow](#summaryRowBelow--)| boolean | Indicates if the summary row will be positioned below the detail rows in the outline. |
| [summaryColumnRight](#summaryColumnRight--)| boolean | Indicates if the summary column will be positioned to the right of the detail columns in the outline. |
## Methods
| Method | Description |
| --- | --- |
| [getSummaryRowBelow()](#getSummaryRowBelow--)| <b>@deprecated.</b> Please use the 'summaryRowBelow' property instead. Indicates if the summary row will be positioned below the detail rows in the outline. |
| [setSummaryRowBelow(boolean)](#setSummaryRowBelow-boolean-)| <b>@deprecated.</b> Please use the 'summaryRowBelow' property instead. Indicates if the summary row will be positioned below the detail rows in the outline. |
| [getSummaryColumnRight()](#getSummaryColumnRight--)| <b>@deprecated.</b> Please use the 'summaryColumnRight' property instead. Indicates if the summary column will be positioned to the right of the detail columns in the outline. |
| [setSummaryColumnRight(boolean)](#setSummaryColumnRight-boolean-)| <b>@deprecated.</b> Please use the 'summaryColumnRight' property instead. Indicates if the summary column will be positioned to the right of the detail columns in the outline. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### summaryRowBelow {#summaryRowBelow--}
Indicates if the summary row will be positioned below the detail rows in the outline.
```javascript
summaryRowBelow : boolean;
```
### summaryColumnRight {#summaryColumnRight--}
Indicates if the summary column will be positioned to the right of the detail columns in the outline.
```javascript
summaryColumnRight : boolean;
```
### getSummaryRowBelow() {#getSummaryRowBelow--}
```javascript
getSummaryRowBelow() : boolean;
```
### setSummaryRowBelow(boolean) {#setSummaryRowBelow-boolean-}
```javascript
setSummaryRowBelow(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getSummaryColumnRight() {#getSummaryColumnRight--}
```javascript
getSummaryColumnRight() : boolean;
```
### setSummaryColumnRight(boolean) {#setSummaryColumnRight-boolean-}
```javascript
setSummaryColumnRight(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
