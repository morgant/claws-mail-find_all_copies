# claws-mail-find_all_copies
by Morgan Aldridge <morgant@makkintosshu.com>

## OVERVIEW

The "Find All Copies" script is an 'Action' script for [Claws Mail](https://claws-mail.org/) which, when run on a specific message, will find all messages in the same IMAP account with the same `Message-ID` header. This can be helpful if using a Gmail account via IMAP, as Gmail implements 'Labels' (i.e. tags) as standard IMAP folders with copies of an individual message in each. It can also help if you've migrated a Gmail account to another IMAP account and want to use IMAP folders in a similar manner. It's also useful in helping you identify where you might have copied a particular message within your IMAP account.

**IMPORTANT:** _This project is very much a work-in-progress and developed specifically for my needs. Use at your own risk!_

### Prerequisites

* An IMAP account synchronized for offline use
* An 'Action' configured to execute the `find_all_copies` script
* Preferably fast storage to improve search time

### Limitations

* It can only search for copies of a single message
* It only supports IMAP accounts (though could be modified to support POP & local MH accounts)
* It cannot find messages that have not yet been downloaded from the IMAP server and stored locally
* It cannot search across multiple accounts
* It's slow as it has to process _all_ messages in the IMAP account (this is despite optimizations to ensure that only the message headers are parsed)

## USAGE

_TBD_

## REFERENCE

* [Claws Mail FAQ: Actions](https://claws-mail.org/faq/index.php/Actions)
* [Claws Mail FAQ: Using Claws Mail with other programs](https://claws-mail.org/faq/index.php/Using_Claws_Mail_with_other_programs)
* [Wikipedia: MH Message Handling System](https://en.wikipedia.org/wiki/MH_Message_Handling_System)

## LICENSE

Released under the [MIT License](LICENSE).
