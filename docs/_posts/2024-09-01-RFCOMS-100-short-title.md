---
# First fill out the document information.

title: 'Test Post'            # Full title of your paper
author: 'Biblo Baggins'            # Your name or alias
category: Guide                    # Essay, Guide, Proposal, or Exploratory
rfcoms: 21
date: 2024-09-04
tags:
  - example
  - pink-flamingos

shortTitle: 'Document'            # An abbreviated version
shortAuthor: 'B. Baggins'         # Your name or alias abbreviated.

abstract: |-
  This is an abstract that I am writing, and I hope it goes well if I write it out like this.


# Next fill out personal information

org: 'Smart People University'     # Optional
working-group: none
address:                           # Optional
    - country: US 
    - address: 'South Bagshot Row'
    - address-code: 55555
public-key: <your-key>             # The fingerprint of your public key if you wish to remain 
                                   # anonymous but verify you wrote this if someone asks.
---

This is an example submissions of an RFCOMS document labled `RFCOMS-example`. Typically your submissions will be `RFCOMS-21` or whatever number happens to be the latest available. Unlike the official documentation for the internet, known as RFCs, these rules are not as strict. However, you do need to provide the following YAML header when submitting an RFCOMS. Use this as a template.[^1]

```yaml
---
# First fill out the document information.

title: 'Document Title'            # Full title of your paper
author: 'Biblo Baggins'            # Your name or alias
date: 2024-09-04
category: Guide                    # Essay, Guide, Proposal, or Exploratory
rfcoms: 21

short-title: 'Document'            # An abbreviated version
author-short: 'B. Baggins'         # Your name or alias abbreviated.

abstract: |-
  This is an abstract that I am writing, and I hope it goes well if I write it out like this.

keywords:
  - example
  - pink-flamingos

# Next fill out personal information

org: 'Smart People University'     # Optional
working-group: none
address:                           # Optional
    - country: US 
    - address: 'South Bagshot Row'
    - address-code: 55555
public-key: <your-key>             # The fingerprint of your public key if you wish to remain 
                                   # anonymous but verify you wrote this if someone asks.
---
```

[^1]: This is an example of a footnote.
