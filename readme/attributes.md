ATTRIBUTES


XML attributes allow  us to include additional info about an element.
The info included in an attribute should describe or augment the data.
It is best practice to avoid using attributes.
Attributes are great for describing metadata.

Attributes are name-value pairs:
<customer id="12345">

To declare attributes in DTD use ATTLIST declaration:
<!ATTLIST element-name attribute-name attribute-type attribute-value>

The attribute-type field can be set to one of the following value types:
- an actual value enclosed in quotes
- #IMPLIED  specifies no default value is provided; but the attribute is optional
- #REQUIRED  specifies no default value is provided; therefore, a value must be provided
- #FIXED  specifies that a value is provided and represents the only value that may be used

Attribute types include:
- CDATA  character data
- ENTITY  the name of an entity declared within DTD
- ENTITIES  a list of entity names
- Enumerated  a list of values
- ID
etc.

Reserved attribute-names:
- lang  classifies an element by the language of its content
- space  specifies whether whitespace should be preserved in element content
- link  specifies an element as a link
- attribute  allows remapping of attribute names
