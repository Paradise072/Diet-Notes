# Diet Notes
I felt that most notes apps and data storage systems were insufficient for the way I organize information. I rarely need more than a few key words or pieces of information to be noted down.

This notes system uses a simple key-value pairing system to store and display provided text. It includes an easy search filter so that the user can look for previous data by its name or contents (i.e. "Zack's Birthday").

## Sorting Notes by Synonyms

This system, while functional, led to an interesting issue- what if I forgot exactly what the name of my note was? What if I named the data "passcode" instead of "password"?

To remedy this issue, I added a list of English synonyms to the search criteria. When creating a new note, the site will "tag" that note with synonyms for every word in its name and contents. (e.g. A note with "help" will have "assist, aid, support" as some of its tagged keywords.)

The dataset for the synonyms came from a JSON file at this GitHub repository, by writing a script to convert from JSON to a Javascript object for ease of access: [https://github.com/zaibacu/thesaurus/blob/master/en_thesaurus.jsonl]

All credit for the original data goes to Wordnet. Their license can be viewed here: [https://wordnet.princeton.edu/license-and-commercial-use]
