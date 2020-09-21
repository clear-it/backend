## Backend Documentation
This document will lay out the specifications of the Backend and the data to be sent/received.

## Data Shape
Proposed (may have to be modified based on research):

    { State: "NJ",
    ProhibCrimes: ["Sex", "Drugs"],
    Duration: "10",
    Source: "https://law.justia.com/codes/new-jersey/2009/title-2c/2c-52/",
    Updated: "9/21/2020"
    Qualifiers: "Expungement possible in certain cases after 5 years",
    ExtraReqs: ["Sentence", "Fine"]
    }

Describes a State which allows expungement of crimes after 10 years, providing that sentencing has been completed and fines paid and they are not sex or drug crimes.  It provides the source for the information, a last updated notice, and notes that in some cases, expungement may be granted after 5 years.

By default the api should return the lengthier term and note the possibility of a shorter term, which user can research on the source page.
