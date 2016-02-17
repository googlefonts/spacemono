Colophon Space Mono
===================

Space Mono is an original monospace display typeface family designed by Colophon for Google Design.

It supports a Latin Extended glyph set, enabling typesetting for English and other Western European languages. 

Developed explicitly for use in headline and display typography, the letterforms infuse a geometric slab core with novel over-rationalized forms. 

License
-------

Space Mono is available under the SIL Open Font License v1.1, for more details see [OFL.txt](OFL.txt)

Contributions
-------------

The project is led by Colophon, a type design foundry based in London and New York. 
To contribute ideas and feedback, see [github.com/googlefonts/spacemono/issues](https://github.com/googlefonts/spacemono/issues)

We may accept contributions via GitHub pull requests, but require all authors to sign the Google Contributor License. 
Please see [CONTRIBUTING.md](CONTRIBUTING.md) for more details.

Disclaimer
----------

This is not an official Google product (experimental or otherwise), it is just work that happens to be owned by Google.

Source Files
------------

```
└── sources
    ├── FontMenuNameDB # Contains font family names for each style naming
    └── Roman # Two folders containing all of the information needed to build the fonts
        ├── Bold
        │   ├── GlyphOrderAndAliasDB
        │   ├── SpaceMono-Bold-Beta-4.ttf
        │   ├── SpaceMono-Bold-Beta4-Source.ttf
        │   ├── current.fpr
        │   ├── features
        │   └── fontinfo
        └── Regular
            ├── GlyphOrderAndAliasDB
            ├── SpaceMono-Regular-Beta5-Source.ttf
            ├── SpaceMono-Regular-Beta5.ttf
            ├── current.fpr
            ├── features
            └── fontinfo
```

Build Instructions
------------------

Use the [Adobe AFDKO](https://github.com/adobe-type-tools/afdko) to build:

    cd sources/Roman/Regular;
    makeotf -r -f SpaceMono-Regular-Beta-X-Source.ttf -o SpaceMono-Regular-Beta-X-Build.ttf;
    cd ../Bold;
    makeotf -r -f SpaceMono-Bold-Beta-X-Source.ttf -o SpaceMono-Bold-Beta-X-Build.ttf;
