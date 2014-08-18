eXtended PGN
============

**eXtended PGN** (XPGN, .xpgn; note that other file extensions, including .pgnx, are defined within this project) is an attempt to extend the Portable Game Notation (PGN) format used to record chess games in computer software since 1993.  The aim is to provide greater data which can be more readily utilised between files, databases or systems as well as enabling the extended rules or styles of play in many chess variants.

This project draws from the following existing work or projects:

* PGN; obviously XPGN will need to incorporate the entire PGN specifications, including the supplemental specifications for time controls and time keeping.
* ChessGML; an attempt to bring PGN forward with the aide of XML to bring greater consistency to game data and facilitate the transition of that data between multiple file formats (especially PGN, HTML and other printable formats).
* ePub and/or ODF; XPGN files will be significantly larger than PGN files and these two file formats have a solution involving interelated XML or XHTML files contained within a compressed container file.

File types and extensions defined in this specification:

* XPGN: .xpgn; a container file or file/directory structure containing CGML/XML files (and possibly other open standard file types) for storing one or more chess games.  May contain standard PGN files, HTML files and/or XHTML files.  May contain other file formats if specified within XML files (e.g. pictures of players).
* XPGNZ: .xpgnz, .xpgz; a compressed PGN file using a free and open lossless compression algorithm as well as incorporating an archiver.  The two most likely candidates for this being 7-Zip (.7z), GNU Tar and xz (.txz), and Zip/WinZip/etc. (.zip).
* CGML: .cgml; An XML version 1.0 compliant markup language for storing data relating to chess games, both standard and variant, as well as matters relating to those games (e.g. tournament information, federation information, etc.).  The first version of CGML is Andreas Saremba's [ChessGML](http://www.saremba.de/chessgml/why.htm), with later versions building on that solid foundation (but not including any of the Java scripts and batch files because forcing Java on people is just unconscionable).
* PGNX: .pgnx; an ASCII text file containing PGN and additional data for displaying or recording special moves in chess variants.  File format is generated from data found in XPGN[Z].

Other file types used or not:

* Pretty much anything you want (at this stage).
* Should avoid including javascript or other scripting languages inside the file format as that's just asking for an exploit to hit some unsuspecting chess GUI developer's pet project.
* Adding .js PGN viewers to HTML being generated from the file format should be handled by other scripts or tools accessing the file format, not launched from inside the thing (that's when it stops being useful and starts being a Trojan)..
