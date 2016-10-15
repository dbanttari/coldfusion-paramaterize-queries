# coldfusion-paramaterize-queries

_ParameterizeQueries.cfm v1.5 (20080721)

Written by Daryl Banttari dbanttari@gmail.com
RELEASED TO THE PUBLIC DOMAIN.  But feel free to credit me with original authorship if you release it with modifications.


## Purpose:

	Seek out unparamaterized queries in ColdFusion templates and, at user's option, 
	parameterize them.

## Use:

	Place _ParameterizeQueries.cfm in a document directory and load.
	Template will start from its current directory and proceed to read all .cfm documents in that 
	directory, find and report all <CFQUERY>s found, and, if it looks like there's a spot that
	<CFQUERYPARAM> can be used, give you the option to parameterize the query.

	If "beRecursive" is set to True (just after these comments), it will recursively
	search all subdirectories, too.

	If "overwriteInPlace" is set to True (just after these comments), it will replace the files
	in place, and save a copy of the "before" file as ".old".  If false, changes will be saved in
	files with ".new" appended.

	To parameterize, click the "Parameterize!" button at the bottom, and all selected queries
	will be parameterized, and the resulting template saved.
	Be sure to test the changes before placing the new code into production!!!

	Templates beginning with an underscore character ("_") will be skipped.
	If working recursively, directories starting with a period (".") will be skipped.
	
	Do NOT leave this on production servers..!
	
## Legal:

	Furnished without warranty of ANY KIND including merchantability
	or fitness for any particular purpose.  Use at your own exclusive risk.
