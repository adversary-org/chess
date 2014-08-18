CGML
====

Takes the current version of [ChessGML](http://www.saremba.de/chessgml/why.htm), which has been the current version for nearly a decade and a half, and builds on it using the XML it is, to bring chess notation and file formats into the 21st century.

The name and acronym is obviously derived from ChessGML and CXML is well and truly taken.  Since I am not yet sure what, if anything, the original author intends regarding the development of ChessGML, CGML is a fork.  Given the stated end goal, however, I doubt there will be much conflict as long as both remain within the confines of XML (which they will need to).

As a result of former employment with Sun and certain other things, I have developed a healthy distrust of Java.  Therefore I do not recommend the Java tools on the ChessGML website as fit for purpose (I'm sure they were fine 14 years ago, but I'm just as sure that there are better ways now).  The CGML specification will define the processes which developers will need to implement in the language(s) of their choice to use or convert the data recorDed in CGML.

ChessGML utilises old-style DTDs rather than current XML Schemas, this is because ChessGML was published in 2000 and the XSD was not established until 2001.  Thus the first major component of this project is to convert from DTD to XSD (i.e. effectively rewrite it).  Which is more than ample reason for the name change.

Now if only there was a non-Java, open source XML/XSD/XSLT WYSIWY[G|M] editor ... anywhere ... at all.

Since there's not this might take a while considering other commitments.

