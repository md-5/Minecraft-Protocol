Minecraft Protocol
==================

Packet Format
-------------

Each packet in the Minecraft protocol comes sent in a vary distinct data format.
First, each frame begins with a varint that signifies the entire length of the following data.
This varint contains both the length of the `Packet ID` and the length of the `Packet Data`.

Field Name    | Type
------------- |-------
Length        | varint
Packet ID     | varint
Packet Data   | varies
