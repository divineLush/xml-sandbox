DTD (Document Type Declaration)


Specifies the name of the document element.
Specifies an internal/external DTD.
The purpose of DTD is to define the legal building blocks of an XML document.
Not the best solution for describing XML documents as they limit our expressiveness in describing the XML data.

An internal DTD id declared inside the XML file within a DOCTYPE definition:
<!DOCTYPE customer[
    <!ELEMENT customer (firstname, lastname)>
    <!ELEMENT firstname (#PCDATA)>
    <!ELEMENT lastname (#PCDATA)>
]>

An externally defined DTD is declared within a DOCTYPE definition:
<?xml version="1.0"?>
<!DOCTYPE CATALOG SYSTEM "catalog.dtd">

DTD element operators allow file-grain control of the XML document's definition:
- +  one or more occurences of child
- *  zero or more occurences of child
- ?  zero or one occurences of child
- |  either/or one of the listed child elements
- ,  used to separate elements in a sequence

An XML element may be defined:
- to be EMPTY
- to be ANY
- as containing parsed container data with #PCDATA (parsed character data)
