# Waking up Tamagotchi Town —TamaTown

> Tamatown was an interactive website for the Tamagotchi Connection Version 3, and later for the Version 4 and Version 4.5. It was an extension to the virtual pets, and allowed players to connect to the site and earn prizes for their Tamagotchi device. 
>
> On February 6, 2013 the servers for Tamatown were shut down. Tamatown no longer supports the enhanced gameplay feature for any of the Tamagotchi Connection devices. Any codes that come with certain pets, such as the Music Star, are no longer usable with the TamaTown websites.
>
> —[Tamagotchi Wiki](http://tamagotchi.wikia.com/wiki/TamaTown)

This project's goal is to document the various TamaTowns that were once available online and how they functioned.

### Contents

* [TamaTown Main Site](#tamatown-main-site)
* [TamaTown V3](#tamatown-v3)
* [TamaTown V4/4.5](#tamatown-v445)
* [TamaTown V5](#tamatown-v5)
* [TamaTown post 2013](#tamatown-post-2013)
* [Japanese TamaTowns](#japanese-tamatowns)
* [External Links](#external-links)
* [Notes](#notes)

## TamaTown Main Site

TamaTown was originally available at [tamatown.com](http://tamatown.com). The site had buttons to open the actual TamaTown (a Flash file) in a browser pop-up. Between 2005 and 2013, four TamaTown versions were released worldwide in English: V3, V4/4.5, V5, Music Star in addition to three in Japanese: Tama Go (Entama), Uri Tama and Tama School.

The [last archived version of tamatown.com](https://web.archive.org/web/20120628032429/http://new.tamatown.com:80/) dates from Jun 28th, 2012. Since 2017, a [Tamagotchi Collectors group](https://www.facebook.com/groups/TamagotchiCollectors/) owns the domain name [tamatown.com](http://tamatown.com).

TamaTown was officially shutdown on Feb 6, 2013. As of 2018, Bandai keeps hosting a TamaTown site at [bandai.com/tamagotchi/new](http://www.bandai.com/tamagotchi/new/). See below [TamaTown post 2013](#tamatown-post-2013).

## TamaTown V3

TamaTown V3 was originally available at [v3.tamatown.com](http://v3.tamatown.com), no longer available.

[Last archived version](http://web.archive.org/web/20120210204403/http://v3.tamatown.com/#) available is from Feb 10th, 2012.

### Recovered files

* Main loader and intro scene: `tama_shell.swf`, `intro.swf`
* Places: `town.swf`, `grandparents.swf`, `king.swf`, `parents.swf`
* Characters: `32400.swf`
* Definitions: `items.xml`

See all files recovered by the Wayback Machine [here](http://web.archive.org/web/*/v3.tamatown.com/*).

### Missing files

The following files have not been archived by the [Wayback Machine](http://web.archive.org):

* Places: `arcade.swf`, , `clothing.swf`, `foodcourt.swf`, `mall.swf`, `school.swf`, `theatre.swf`, `townhall.swf`, `travel.swf`
* Games: `clawgame.swf`, `createasonggame.swf`, `japanracegame.swf`, `namethattuneGame.swf`, `racegame.swf`, `suitcasegame.swf`, `tamasaysgame.swf` 
* Audio: `grandparents.mp3`, `king.mp3`, `song1.mp3`

### Auth

We are asked an username at the beginning, e.g. 'abc'.

Then, the following HTTP request is sent to the server:

> GET http://v3.tamatown.com/cgi-bin/Tamatown.cgi?d=80&a=GI&p=0000000000&u=abc

Note we are not being asked a password quite yet, hence it is sent as '0000000000'. The request contains 2 more parameters, `d=80` and `a='GI'`.

To access the Parents, Grandparents or King area, TamaTown asks for our Tamagotchi's password:

SWF Decompilation indicates hardcoded passwords to access these 3 areas:

* Parents: type `pass paren`
* Grandparents: type `pass grand`
* King: type `pass king`

If none of this is used, provided the input are 10 digits (e.g. `1234567890`), the following HTTP request is sent:

> GET http://v3.tamatown.com/cgi-bin/Tamatown.cgi?a=AP&p=1234567890&u=abc

## TamaTown V4/4.5

TamaTown V4/4.5 was originally available at [v4.tamatown.com](http://v4.tamatown.com) and [tamagotchieurope.com/EN/JinSeiEN/tamaok.html](http://www.tamagotchieurope.com/EN/JinSeiEN/tamaok.html), today down. Thanks to the Wayback Machine, some SWF files were recovered.

This [TamaTown Commercial](https://www.youtube.com/watch?v=lT0aCfIb-qQ) shows how it looked like.

### Recovered files

These were found in [archived tamagotchieurope.com (May 9, 2013)](http://web.archive.org/web/20130509173044/http://www.tamagotchieurope.com:80/EN/JinSeiEN/tamaok.html) and this [MEGA repository](https://mega.nz/#F!1vwBiDyS!SyjPOhuZlurpd_wY7zWmRg).

* Main loader and intro scene: `tama_shell.swf`, `intro.swf`
* Places: `town.swf`, `grandparents.swf`, `king.swf`, `mall.swf`, `music.swf`, `music1.swf`, `music2.swf`, `parents.swf`, `tama_island.swf`, `toys.swf`
* Assets: `charaALL.swf`, `vote_off.swf`
* Definitions: `tama_games.xml`, `tama_help_welcome.xml`, `tama_info.xml`, `tama_items_characters.xml`, `tama_shell_text.xml`

See all files recovered by the Wayback Machine [here](http://web.archive.org/web/*/v4.tamatown.com/*).

### Missing files

The following files have not been archived by the [Wayback Machine](http://web.archive.org):

* Places: `arcade.swf`, `bank.swf`, `clothing.swf`, `foodcourt.swf`, `hospital.swf`, `office.swf`, `postoffice.swf`, `preschool.swf`, `racegame.swf`, `school.swf`, `station.swf`, `theatre.swf`, `townhall.swf`, `travel.swf`
* Audio: `king.mp3`

## TamaTown V5

TamaTown V5, also known as _The Tama & Earth Expo_, was originally available at [famitama.com/pc/index_en.html](http://famitama.com:80/pc/index_en.html), today down.

### Recovered files

SWF files for games were first recovered by [SA311 in this TamaTalk thread](http://www.tamatalk.com/IB/topic/190374-tama-earth-expos-games-v5famitama/) using the [web archive (Jan 30, 2010)](http://web.archive.org/web/20100130042932/http://famitama.com/pc/index_en.html) and continued by this project.

See all files recovered by the Wayback Machine [here](http://web.archive.org/web/*/famitama.com/pc/*).

### Auth

Upon start, an HTTP request is sent to:

> GET http://famitama.com/pc/cgi/Famiif.php?r=845107&a=0&e=00&f=ww&d=00000&u=00000&c=3

where:

* r is a pseudo-random number generated by: `getTime() / 1800000`
* c is `1` for login/logout, `3` for wagon, `4` for farm, `5` for poll 
* a is poll data, otherwise `0`
* e is poll key, otherwise `00`
* f is `ww` for wagon
* u is a 5 digits upper password, default `00000`
* d is a 5 digits lower password, default `00000`

The expected response is a `text/plain` string with the following parameters:
 
* `ResultCode`: must be `OK` to consider the response valid.
* Rest of parameters: `LoginMode`, `VER`, `CharacterCode`, `FamilyCode`, `TiesCode`, `JPFarm`, `JPWagon`, `AOFarm`, `AOWagon`, `NAWagon`, `EUFarm`, `EUWagon`, `JPAnswer`, `AOAnswer`, `NAAnswer`, `EUAnswer`, `DateTime`, `ResultDetail`

Whenever users choose a game to play, they are asked to login. This sends the following request:

> GET http://famitama.com/pc/cgi/Famitama.cgi?p=game%5Ffishing%2Eswf&i=0&g=0&m=0&d=11111&u=11111&c=1

where 

* p is the current game filename, e.g. `game_fishing.swf`
* c is the request code, `1` for login
* i is the items upon logout, `0` for login
* g are the gotchi points upon logout, `0` for login
* m is the logout code, `0` for login
* u is a 5 digits upper password, default `00000`
* d is a 5 digits lower password, default `00000`

The expected response is a `text/plain` string with the following parameters:

* `ResultCode` must be `OK` to consider the response valid.
* Rest of parameters: `LoginMode`, `VER`, `CharacterCode`, `FamilyCode`, `TiesCode`, `PasswordUp`, `PasswordDown`, `DateTime`

After finishing a game, players can logout. This issues the following request:

> GET http://famitama.com/pc/cgi/Famitama.cgi?p=game%5Fmochitsuki%2Eswf&i=0&g=0&m=2&d=11111&u=11111&c=1

* p is the current game filename, e.g. `game_mochitsuki.swf`
* i is the number of items upon logout, default `0`
* g are the gotchi points upon logout, default `0`
* m is the logout code, `1` for nothing, `2` for gotchi points, `3` for getting item, `4` for buying item
* d is a 5 digits lower password, default `00000`
* u is a 5 digits upper password, default `00000`
* c is the request code, `1` for logout

## TamaTown Music Star

TamaTown Music Star was originally available at [new.tamatown.com](http://new.tamatown.com/), no longer available. This [TamaTown Exploration video](https://www.youtube.com/watch?v=8LImCTDiMb4&t=2s) shows how it looked like.

### Recovered files

See all files recovered by the Wayback Machine [here](http://web.archive.org/web/*/new.tamatown.com/*).

### Auth

## TamaTown post 2013

Bandai keeps hosting an extremely lighter version of TamaTown Music Star at [bandai.com/tamagotchi/new](http://www.bandai.com/tamagotchi/new/). Upon language selection, English and Spanish redirect to the ['Thank you'](http://www.bandai.com/tamagotchi/thankyou/) and ['Gracias'](http://www.bandai.com/tamagotchi/gracias/) shutdown pages respectively. The site in Portuguese, however, lets user access the forest area and play a rafting game.

## Japanese TamaTowns

**e-TamaGo** was Japan's TamaTown website, originally available at [e-tamago.com/pc/index.html](http://e-tamago.com/pc/index.html), [last archived in 2010](http://web.archive.org/web/20100928030034oe_/http://e-tamago.com/pc/index.html). Today e-tamago.com redirects to [tamagotch.channel.or.jp](http://tamagotch.channel.or.jp). e-TamaGo let players enter 3 TamaTowns: Tama Go, Ura Tama and Tama School.

### Tama Go

Tama Go was originally available at [e-tamago.com/pc/flash/tamago.html](http://e-tamago.com/pc/flash/tamago.html), see [(this archive from 2010)](http://web.archive.org/web/20100928030034oe_/http://e-tamago.com/pc/flash/tamago.html).

#### Recovered files

See all files recovered by the Wayback Machine [here](http://web.archive.org/web/*/e-tamago.com/pc/flash/*).

### Ura Tama

Ura Tama was originally available at [e-tamago.com/urapc/flash/uratama.html](http://e-tamago.com/urapc/flash/uratama.html), see [(this archive from 2010)](http://web.archive.org/web/20100928030034/http://e-tamago.com/urapc/flash/uratama.html)

#### Recovered files

See all files recovered by the Wayback Machine [here](http://web.archive.org/web/*/e-tamago.com/urapc/flash/*).

### Tama School

Tama School was originally available at [school.e-tamago.com/pc/flash/tamasc.html](http://school.e-tamago.com/pc/flash/tamasc.html), see [this archive from 2010](http://web.archive.org/web/20100201125243/http://school.e-tamago.com/pc/flash/tamasc.html)

#### Recovered files

See all files recovered by the Wayback Machine [here](http://web.archive.org/web/*/school.e-tamago.com/pc/flash/*).

## External Links

### On TamaTown

* [Wikipedia, "Tamagotchi Town"](https://en.wikipedia.org/wiki/Tamagotchi_Town)
* [Archived tamagotchieurope.com (May 9, 2013)](http://web.archive.org/web/20130509173044/http://www.tamagotchieurope.com:80/EN/JinSeiEN/tamaok.html) 
* [MEGA repository, unknown owner](https://mega.nz/#F!1vwBiDyS!SyjPOhuZlurpd_wY7zWmRg)
* [lostmediawiki.com, "Tamagotchi TamaTown (partially found flash game; 2006-2013)"](https://lostmediawiki.com/Tamagotchi_TamaTown_(partially_found_flash_game;_2006-2013))
* [change.org 'Get TamaTown back!'. Petition closed in 2015](https://www.change.org/p/bandai-co-ltd-get-tamatown-back)

### On Flash

* [Adobe. SWF File Format Specification. Version 19](https://wwwimages2.adobe.com/content/dam/acom/en/devnet/pdf/swf-file-format-spec.pdf)

### TamaTalk threads

* [Playing e-Tamago's games](http://www.tamatalk.com/IB/topic/190345-playing-e-tamagos-games/)
* [Playing Ura-TamaTown's games](http://www.tamatalk.com/IB/topic/190354-playing-ura-tamatowns-games/)
* [Tamagotchi School (TamaSuku) page's games](http://www.tamatalk.com/IB/topic/190368-tamagotchi-school-tamasuku-pages-games/)
* [Tama & Earth EXPO's games. (V5/Famitama)](http://www.tamatalk.com/IB/topic/190374-tama-earth-expos-games-v5famitama/)
* [Games from the old Japanese TamaTown](http://www.tamatalk.com/IB/topic/194300-games-from-the-old-japanese-tamatown)

## Notes

I decompiled the SWF files that the Wayback Machine preserved with [JPEXS Free Flash Decompiler](https://github.com/jindrapetrik/jpexs-decompiler). It's a powerful open-source tool, way superior to other commercial options in my opinion.

##### Disclaimer

TamaTown and Tamagotchi are trademarks of Bandai Namco Inc. This website is not affiliated or endorsed by Bandai Namco Inc. in any way.