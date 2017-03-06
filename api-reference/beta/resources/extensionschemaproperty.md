# ExtensionSchemaProperty resource type

Use the extensionSchemaProperty resource to define a property's name and its type, as part of a schema extension definition.


### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|name|String| Name of the strongly typed property defined as part of a schema extension.|
|type|String| Type of the property that is defined as part of a schema extension.  Allowed values are *Binary, Boolean, DateTime, Integer* or *String*.  See the table below for more details.|

#### Supported property data types 
The following data types are supported when defining a property in a schema extension:

| Property Type | Remarks |
|-------------|------------|
| Binary | 256 bytes maximum. |
| Boolean | Not supported for messages, events and posts. |
| DateTime | Must be specified in ISO 8601 format. Will be stored in UTC. |
| Integer | 32-bit value. Not supported for messages, events and posts. |
| String | 256 characters maximum. |

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extensionSchemaProperty"
}-->

```json
{
  "name": "StockKeepingUnits",
  "type": "Integer"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extensionSchemaProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->