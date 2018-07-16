# MDeval
Python module for xml metadata analysis and reporting

Written by Sean Gordon, Aleksandar Jelenek, and Ted Habermann.
Based on the NOAA rubrics Dr Habermann created, and his work
conceptualizing the documentation language so that rubrics using
recommendations from other earth science communities can be applied
to multiple metadata dialects as a part of the USGeo BEDI and
NSF DIBBs projects. This python module as an outcome of DIBBs allows
a user to initiate an evaluation of valid XML. If it is not a metadata
standard that has not been ingested as a documentation language dialect
in AllCrosswalks.xml, this XML can be evaluated using the XPath dataframe
functions. Other metadata standards can be
conceptualized and added to the Concepts Evaluator. Then the module can be
rebuilt and the recommendations analysis functions can be run anew.

The basic workflow is to retrieve records, evaluate for concept and xpath content,
run concept/xpath counts and occurrence functions on csv output of evaluation,
create collectionspreadsheet with the outputs, if you want to compare between
collections, combine csv outputs with appropriate combination functions, create
organizationSpreadsheet. Finally run WriteGoogleSheets on any xlsx outputs
you want to share.
