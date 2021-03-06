..  PyCantonese documentation master file, created by
    sphinx-quickstart on Sat Dec 27 15:23:24 2014.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.

..  _index:

PyCantonese: Cantonese Linguistics and NLP in Python
====================================================

PyCantonese is a Python library for Cantonese linguistics and natural
language processing (NLP).
The goal of PyCantonese is to provide general-purpose tools and other
functionality to work with Cantonese data. They include corpus search
functions as well as various analytic and annotation tools;
these and other possibilities
are gradually added
as the library grows and evolves.


#social-media#


.. sidebar:: Quick examples -- What can PyCantonese do?

    With PyCantonese in Python:

    .. code-block:: python

        >>> import pycantonese as pc

    1) Parsing Jyutping for (onset, nucleus, coda, tone)

    .. code-block:: python

        >>> pc.parse_jyutping('gwong2dung1waa2')  # 廣東話
        [('gw', 'o', 'ng', '2'), ('d', 'u', 'ng', '1'), ('w', 'aa', '', '2')]


    2) Finding all verbs in the HKCanCor corpus

       We search for the regular expression ``'^V'`` for all words whose
       part-of-speech tag begins with "V":

    .. code-block:: python

        >>> corpus = pc.hkcancor() # get HKCanCor
        >>> all_verbs = corpus.search(pos='^V')
        >>> len(all_verbs)  # number of all verbs
        29012
        >>> from pprint import pprint
        >>> pprint(all_verbs[:10])  # print 10 results
        [('去', 'V', 'heoi3', ''),
         ('去', 'V', 'heoi3', ''),
         ('旅行', 'VN', 'leoi5hang4', ''),
         ('有冇', 'V1', 'jau5mou5', ''),
         ('要', 'VU', 'jiu3', ''),
         ('有得', 'VU', 'jau5dak1', ''),
         ('冇得', 'VU', 'mou5dak1', ''),
         ('去', 'V', 'heoi3', ''),
         ('係', 'V', 'hai6', ''),
         ('係', 'V', 'hai6', '')]


Table of contents
-----------------

..  toctree::
    :maxdepth: 2

    download
    data
    reader
    jyutping
    searches
    papers


How to cite
-----------

PyCantonese is maintained by
`Jackson Lee <http://jacksonllee.com>`_.

A talk introducing PyCantonese:

Jackson L. Lee. 2015. PyCantonese: Cantonese linguistic research in the age of big data. Talk at the Childhood Bilingualism Research Centre, Chinese University of Hong Kong. September 15. 2015. `[Notes+slides] <http://pycantonese.org/papers/Lee-pycantonese-2015.html>`_

See :ref:`papers` for a running list of our work.

Technical support, library development, etc.
--------------------------------------------

Questions, bug reports and suggested features are more than welcome.
Please create issues on the
`GitHub page <https://github.com/pycantonese/pycantonese>`_.
Alternatively, you may contact `Jackson Lee <http://jacksonllee.com>`_.

`Changelog <https://github.com/pycantonese/pycantonese/blob/master/changelog.md>`_ on GitHub

