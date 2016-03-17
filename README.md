# ughjira

:hankey: Import GitHub issues into JIRA :hankey:

U GitHub->JIRA. `ughjira`. Get it?

## Usage

 1. Configure `dot.ughjira.conf` and put it in `$HOME/.ughjira.conf`.
 2. Run `carton install`.
 3. Run `carton exec ./ughjira`.
 4. Be happy you didn't have to wade through the half-finished, mostly broken
    GitHub API implementations in Perl and spend way too many hours figuring
    out that there is no good way to convert Markdown -> Confluence.
 5. Send a PR or file an issue if you have an error, and accept my apologies if
    that creates extra work for you.

## Features

`Ughjira` imports issues from GitHub into JIRA, and attempts to be friendly in the
following ways:

 1. It attempts to preserve (to the best of its ability) formatting in issue
    descriptions and comments.
 2. It attempts to preserve user information.
 3. Cross-references issues from GH -> JIRA -> GH.
 4. Closes issues in GH.

## TODOs

 1. Some formatting things do not carry over.
 2. Images do not carry over (as far as I'm aware).
 3. Blockquotes are not handled.
 4. Issues closed in GH are not handled.
 5. User assignment in JIRA is not handled.
 6. Does not import closed issues.

I'll happily accept patches that help your use case. This script is a quick
hack that I'm sure will be disappointing to someone when it doesn't do 
exactly what they want.
