# map_PGS_to_disease_category

This script loads metadata from PGS catalog and from EFO database, and maps PGS to more general disease categories (e.g., melanoma -> cancer, obesity -> metabolic disorder).

The first step after loading the data is to create a dictionary structure (key -> value) mapping PGS as keys and the most general EFO category names as values.

After that, the script loads your typical PGSwas or PRSwas results (p-values or betas), parses the PGS ids from the PRS_name column, and creates a new column in your data called "Trait_category" with the more general disease category names.
