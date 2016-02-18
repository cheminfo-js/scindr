# SCINDER

Javascript library allowing to retrieve, combine and rank various information from the web

A practical example is the possibility to retrieve "similar" molecules.

* You have different source of information
* You need to format the result so that they can be combined
* You could make the result "unique"
* You could rate the result

## Pubchem

https://pubchem.ncbi.nlm.nih.gov/pug_rest/PUG_REST.html

https://pubchem.ncbi.nlm.nih.gov/pug_rest/PUG_REST.html#_Toc409516770

https://pubchem.ncbi.nlm.nih.gov/rest/pug/compound/fastsimilarity_2d/smiles/CCCCC/property/MolecularFormula,InChI,CanonicalSMILES,IUPACName/JSON

## ChemSpider

Seems very very slow ... Should check how to make a query in a reasonnable time

http://www.chemspider.com/JSON.ashx

Seems ChemSpier query has to be done in 2 steps

http://www.chemspider.com/JSON.ashx?op=SimpleSearch&searchOptions.QueryText=Aspirin


http://www.chemspider.com/JSON.ashx?op=SimilaritySearch&searchOptions.Molecule=C1CCCCC1&searchResultOptions.Limit=10

Get search status:
http://www.chemspider.com/JSON.ashx?op=GetSearchStatus&rid=41d45ec0-75e3-40c6-8764-a76ff939889b
Status is one of the following:0: Unknown
* 1: Created
* 2: Scheduled
* 3: Processing
* 4: Suspended
* 5: PartialResultReady
* 6: ResultReady
* 7: Failed
* 8: TooManyRecords



Get search result:
http://www.chemspider.com/JSON.ashx?op=GetSearchResult&rid=41d45ec0-75e3-40c6-8764-a76ff939889b




