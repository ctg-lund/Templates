# All PEP
Fork of Seq Only PEP
Adds a projects.csv to the specification
Can contain annotation of any bioinformatic workflow due to the super_table abstraction
which describes the project at the project level
samples.csv corresponds to the \[Data] section of a sample sheet
projects.csv corresponds to \[Project_Data]

For particular workflows we need optional corresponding csv sheets
eg when we write a new DNA_dragen pipeline, the All PEP specification
needs to be extended to take pipeline specific parameters.

This is a 2 step process - first the config.yaml needs to be extended with
the path to the new table.csv:
```
new_table: new_table.csv # just the file name
new_properties:
    samples: # or projects depending on the level of annotation
    	type: array
    	items:
    		type: object
    		properties: # columns go here
    			sample_name: # key can be sample_name or project_id
    				type: string
    				description: lots of words
    				pattern: ^regexp$
    				default: true
```
Then the samplesheet generator can be extended to read the resulting table.
I will try to start simply by reading the table name to decide what information is there.

    	
