# Report Viewed

### This event is part of the page load sequence, including virtual page loads in the case of single page apps, and must be pushed between the `Page Load Started` and `Page Load Completed` events.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Report Viewed",
    "reportAction": {
        "reports": [
            {
                "reportID": "<reportID>",
                "reportType": "<reportType>"
            }
        ]
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|reportAction.reports[n].reportID|string|Unique ID for a Report||||||||
|reportAction.reports[n].reportType|string|The type of the report|Transactions, Financial|||||||




