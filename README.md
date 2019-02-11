# WikiExtractor for WikiMentions

This is a modified version of the great [Wikiextractor](https://github.com/attardi/wikiextractor) with the additional option to extract the internal Wikipedia links from an article. 

If you run the following command with the enwiki-XXXXXXXX-pages-articles1.xml-XXXXXXXX.bz2 replaced by an actual dump file

    python WikiExtractor.py --json --filter_disambig_pages --processes 2 --collect_links enwiki-XXXXXXXX-pages-articles1.xml-XXXXXXXX.bz2 -o test

then each articles dictionary contains an additional field 'internal_links'. Please see [this notebook](https://github.com/samuelbroscheit/wikiextractor-wikimentions/blob/master/Load%20wikiextractor%20data.ipynb) for a HOWTO and code snippet for reading the data.

For the full README please consult https://github.com/attardi/wikiextractor. However, I have not tested my modifications with other options.