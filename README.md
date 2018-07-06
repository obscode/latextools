# latextools
Some python-based latex tools useful to authors of scientific journals

# Contents
- make_authors:  Given a file with author names and affiliations (with many-to-one association),
                 contruct a .tex file with the appropriate authors section (either in AASTeX 5 or
                 AASTeX 6 format). Keeps track of order of affiliations, multiple authors at the
                 same affiliation, etc.
- fix_authors:  Given a .bbl file generated from BibTeX, go throug the author list and for those
                entries where the number of authors is greater than a certain number (default 5),
                truncate the author list to authors one to three, followed by "et al."
- check_env_order: Scan a .tex file (and any files \input by the file) for labels defined in figure
                and table environments. Then check the order in which they are referenced in the 
                paper. If the order they are referenced does not match the order they were presented,
                let the user know what oder they should use.
