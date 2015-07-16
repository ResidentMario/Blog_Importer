# Blog_Importer
A script that handles tedius setup tasks for the Blog section of the Wikipedia Signpost.

<h2>About</h2>

The "Blog" is a report published as a part of the weekly "Wikipedia Signpost", a community-organized and -written internal newspaper on the English Wikipedia that covers the Wikipedia movement at large. This report republishes content from posts to the Wikimedia Blog, another popular, albiet less neautral, movement platform.

Credit to the WMF's RESTBase API for its wonderful HTML-to-Wikicode conversion facilities.

<h2>Inputs</h2>

This script requires a "-p" or "--page" parameter that is within the domain of the Wikimedia Blog. Otherwise it doesn't know where to look! At a minimum you want to run something that looks like this:

    run Blog_Importer.py -p 'https://blog.wikimedia.org/2015/07/16/third-transparency-report-released'

The script will automatically find and target the next to-be-published Signpost issue, but it also provides a capacity to specify your target manually. Valid inputs are in the domain of the Signpost or my on-wiki userspace (a subpage of "User:Resident Mario").

    run Blog_Importer.py -p 'https://blog.wikimedia.org/2015/07/16/third-transparency-report-released' -t 'Wikipedia:Wikipedia Signpost/Newsroom/Special desk/Draft of stuff'

Or, for testing:

    run Blog_Importer.py -p 'https://blog.wikimedia.org/2015/07/16/third-transparency-report-released' -t 'User:Resident Mario/sandbox'

<h2>History</h2>

| Date  | Comment |
| ------------- | ------------- |
| 7/16/2015  | First version posted here. |
