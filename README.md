# lv-unit-conversion

lv-unit-conversion is a library that can convert from one unit to another. It uses the energistics unit of measure standard (https://www.energistics.org/energistics-unit-of-measure-standard/) in place of constants stored in memory. This library ONLY supports double data type and doesn't have any built in error handling when you attempt to convert between units that don't match.

This library was designed to be used in-memory to perform conversions that don't take a lot of time (hence the dictionary using variant attributes). The expectation is that reading from the XML file for each read (or even at startup with a sufficient number of units) can be pretty intensive, so you can create a dictionary from an xml file and then save that dictionary to a json file.

