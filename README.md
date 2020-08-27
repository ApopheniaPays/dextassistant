VERSION ALPHA 2020.08.25
 
(This is the initial alpha release. More complete information will be added later. Follow [http://t.me/ApopheniaProjects](http://t.me/ApopheniaProjects) on Telegram for announcements.)

# BACKGROUND 

The nice people at [http://DEXTools.io](http://DEXTools.io) have built a great information explorer for Uniswap. However, I found that as I explored the information it gave me, I had to do far too much clicking around to other websites to do my own research on the coins listed. I wanted a quicker way to gather information and determine which coins might be worth investing in, and more importantly, which look like scams and should be avoided. So I took all the research I was doing by hand, and coded an add-on tool that set on top of DEXTools but gave quicker access to all that information, and in some cases, embedded it right in the page without having to leave DEXTools.

Installation tips are included below. Yes, you're going to have to _read_.

# DISCLAIMER 

## TO BE READ IN A STERN, GRUFF VOICE: 

Despite my efforts to give it an easy-to-understand GUI, this is an advanced tool for technically advanced traders.

If you are trading on Uniswap or other DEXs, you need to have a certain level of general knowledge in order to avoid the high risks, and I'm not going to enable anyone to jump in and lose money. If there's anything in this you don't understand, then you probably shouldn't be trading on Uniswap yet, so this tool is not for you.

What's more, as this is under active development, you may find bugs, though I try hard to avoid that.

## Support? Support is for _closers_.

As I'm sharing this for free, I won't give you any support or any guarantees, and if you choose to use it I don't owe you anything for any reason. It's presented as-is, use it only at your own risk. What you see is what you get. If you have questions you'll have to do your own research and figure out the answers yourself. I'm grouchy, don't bother me.

## The murky depths from whence this came

This is an independent project that bubbled up out of a single developer's needs. It's not affiliated with DEXTools.io or its development team in any way, please *never bother them with questions about it*.

## In not so many words:

Essentially, YOU'RE ON YOUR OWN with this. 

Do you think Indiana Jones needed someone holding his hand? No, never. When you're fighting for your life in a remote jungle or far-flung desert outpost, there's no support, no instruction manual, no second chances... just your own ingenuity, will to live, and the rich rewards that will come if you can figure out on your own how to succeed.

As of right now, _that is your life._

(Metaphorically speaking.)

Enjoy!

# INSTRUCTIONS 

## Installation

This script is for use with a browser plugin that allows you to install and manage user scripts, such as Greasemonkey, Tampermonkey, or Violentmonkey. I chose to go with a userscript instead of a browser plugin because it would allow the code to remain 100% open source and cross-platform. 

(Here's where you need to bring a little knowledge to the table. If you're unfamiliar with userscripts or Tampermonkey, Greasemonkey, Violentmonkey, etc, you should educate yourself from a page like [https://simply-how.com/enhance-and-fine-tune-any-web-page-the-complete-user-scripts-guide](https://simply-how.com/enhance-and-fine-tune-any-web-page-the-complete-user-scripts-guide) before you try to use this. BTW I use Tampermonkey [https://www.tampermonkey.net/](https://www.tampermonkey.net/) myself, on Firefox, Brave, and Chrome, so I know for sure this works with that, and that the browser copy properly auto-updates when I update the master in this repo to a new version. But you'll need to decide for yourself which userscript manager is right for you. Consult your doctor.)

*BONUS!* For users that already have a userscript manager extension installed in their browser, you can install DextAssistant simply by loading the raw javascript file by clicking this link: [https://github.com/ApopheniaPays/dextassistant/raw/master/dextAssistant.user.js](https://github.com/ApopheniaPays/dextassistant/raw/master/dextAssistant.user.js). This script is also hosted at [https://openuserjs.org/scripts/ApopheniaPays/DextAssistant](https://openuserjs.org/scripts/ApopheniaPays/DextAssistant) for one-click install if you prefer to get a minified version.

## Usage

This adds a few cosmetic changes to the DEXTools.io Pool Explorer, and soon will also add features to their Pair Explorer page. You will notice them right away:

1.) The most prominent addition is a new icon under the Pool Explorer's Actions column, which opens a "research assistant" popup that will allow you to view data from other websites pertaining to the token Name, Contract Address, and Uniswap.info Pair Address for the token on that row. Next to the Contract addresses you will see a little circled arrow that will show you Google search results for those contract addresses, embedded right in the popup, when you hover your mouse over it.

2.) For tokens with a particularly low DEXT score or which are auto-generated by a lazy website token-generator script, the distinguished monocle and handlebar mustache on the "research assistant" gear button are replaced with a "poop" emoji.

3.) Rows in the the Pool Explorer are color-coded to indicate liquidity adds, removes, and new pools. 100% removals are now labeled as "rugpull" instead of just "remote"

4.) Columns are sortable on both the Pool and Pair explorers buy clicking on the column headings.

5.) In the Pair Explorer page, wallet addresses that have more than one transaction in the list are now color-coded to make it easier to spot scammy trades, where one address buys and sells just to generate activity. Next to these addresses, there is also now a "ƒ" button to filter the list to show all the transactions for just that address, and a "Z" button that takes you to the Zerion overview for that wallet.

As this script makes cosmetic changes only, there's no harm you can do by poking around. Explore it.

# KNOWN ISSUES

1.) Right now the list filtering and sorting only acts on existing rows. As new transactions or pools appear, they come in at the top, exactly as if the list wasn't filtered or sorted. I'll get around to it. Hey, it's an open source script, you don't like it, fix it yourself.

