# How to deal with admin extensions

instructions (taken from https://ltmeat.bypassi.com/#exploit )

The method linked above involves less spamming. It doesn't work for all extensions, but it should work for your filter. However, it's also easier to block. The original instructions are shown below.

STEP ONE: Find a page belonging to the extension you want to disable. You'll need your extension's 32-character ID to continue. If you're trying to bypass stuff, try finding it in a filter extension ID list. For further help, check the help section.

Once you have the ID, you'll be guaranteed to get to a working chrome-extension:// page by visiting the manifest file: (with your extension's ID substituted in, of course)
chrome-extension://extension_id_here_please/manifest.json

Some extensions' pages are much easier to access directly (like their options or block pages). All that's important is that you open a page belonging to the extension you want to disable.

STEP TWO: Bookmark the extension page (bookmark A) if you wish. Then, bookmark chrome://kill (B) and chrome://hang (C).

STEP THREE: While on the extension page (A), click the chrome://kill bookmark (B). The page should crash. You should already have the next step prepared.

STEP FOUR: Instantly start spamming chrome://hang (bookmark C) and quickly reload the page while spamming using the refresh key on your keyboard (or less ideally, ctrl+R). You should have reloaded within one or two seconds of killing the page.

## List of Chrome Extension IDs

Lightspeed/Relay has different IDs for every district, sorry. Read the help section.

GoGuardian: haldlgldplgnggkjaafhelgiaglafanh
Securly (old): iheobagjkfklnlikgihanlhcddjoihkg
Securly (new): joflmkccibkooplaeoinecjbmdebglab
Blocksi: ghlpmldmjjhmdgmneoaibbegkjjbonbk
iBoss: kmffehbidlalibfeklaefnckpidbodff
Fortiguard: igbgpehnbmhgdgjbhkkpedommgmfbeao
Cisco Umbrella: jcdhmojfecjfmbdpchihbeilohgnbdci
NetRef: khfdeghnhlpdfeenmdofgcbilkngngcp
ContentKeeper: jdogphakondfdmcanpapfahkdomaicfa
Hapara: kbohafcopfpigkjdimdcdgenlhkmhbnc
Smoothwall: jbldkhfglmgeihlcaeliadhipokhocnm
Linewize: ddfbkhpmcdbciejenfcolaaiebnjcbfc
LANSchool: baleiojnjpgeojohhhfbichcodgljmnj 



Credit to Caffe#3880
Contact Bypassi if you want any IDs added

## Retrieving one yourself

Okay, fair. Extension IDs are leaked in a couple of places. Generally, the best way to get them is to go to extension settings and copy the URL query value as shown in the (https://thezone-sat0rn.vercel.app/other/vid.webm "Video")

If you're actually competent in dealing with JSON, you can easily find IDs in chrome://extensions-internals too, as well as another similar URL.

##### It says blocked by client?

That's the message you get when you try to visit an a page belonging to an extension that doesn't exist. The error message (ERR_BLOCKED_BY_CLIENT) is extremely misleading. Nobody blocked it--you just need to find the right extension ID (see above).

If you got this because you tried to visit the extension_id_here_please example URL, you should be extremely ashamed of yourself. Please change and grow as a person. 
