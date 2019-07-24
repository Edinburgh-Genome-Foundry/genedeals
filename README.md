# Genedeals

Genedeals aims at making it easier to compare commercial DNA (with a focus on
gene-sized DNA, from 500bp to 10kb). Right now it simply consists in a spreadsheet
aggregating data from public online catalogs.

**Disclaimer:** this project has indicative value only and does not guarantee
that all the information is 100% correct and up to date (last update on July 24
2019). Each entry contains a link to the supplier's webpage and you are
encouraged to check the information at the source.

## Contribute

Genedeals is a project originally started at the Edinburgh Genome Foundry by [Zulko](https://github.com/Zulko) and the data spreadsheet is released [on Github](https://github.com/Edinburgh-Genome-Foundry/genedeals) under a Public Domain licence. Everyone is welcome to contribute, add offers, correct errors, propose improvements, etc.

## Future plans

The repository may also host a Python library in the future to ease the integration of the data into Python workflows, as part of the  `EGF Codons <https://edinburgh-genome-foundry.github.io/>`_
synthetic biology software suite for DNA design, manufacturing and validation.

## Table columns

- **offer_name**: A unique identifier from the offer (arbitrarily chosen by us)

- **company**: The company making the offer (IDT, TWIST)

- **min_sequence_size**: Minimum accepted sequence size in basepairs

- **max_sequence_size**: Maximum accepted sequence size in basepairs

- **clonal_or_fragment**: Whether the product will be clonal (an insert in a plasmid) or a linear DNA fragment.

- **min_business_days**: Minimum number of business days that the manufacturer will need to complete an order. If there is no upper bound (max_business_days), it means that this number is indicative of the typical lead time.

- **max_business_days**: Upper bound on the number of business days that the manufacturer will need to complete an order.


- **min_dna_amount_ug**: Minimum amount of DNA that the manufacturer can guarantee.

- **fixed_cost_usd**: Any flat cost that the supplier applies, and which comes in addition to the basepair cost (min_bp_cost_usd).

- **min_bp_cost_usd**: Minimum cost-per-basepair, in US Dollars. This cost is said "minimal" as a minority of suppliers write "from 35c/bp" instead of "35c/bp". 

- **min_unit_price_usd**: Minimal price to pay for a sequence: the final price for the sequence will be either this number or the addition [basepair cost + fixed cost], whichever is higher.

- **min_units_in_order**: Minimal number of sequences that you must order for the supplier to consider your order.

- **min_bp_in_order**: Minimal number of basepairs that you must order (in possibly several sequences) for the supplier to consider your order.

- **tube_or_plate**: Whether the order is delivered in tubes or plates (or "both" if you have the choice)

- **source_url**: Link to the webpage from which the infos about the offer where obtained.
