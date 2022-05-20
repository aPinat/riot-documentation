# List of Riot Games Endpoints

Leaving out lots of internal dev/staging/test endpoints.

## Riot Games

### Websites

| URL                                  | Description                            |
| ------------------------------------ | -------------------------------------- |
| https://www.riotgames.com            | Riot Games                             |
| https://login.riotgames.com          | Riot Login                             |
| https://xsso.riotgames.com           | XSSO Riot Games                        |
| https://account.riotgames.com        | Riot Account Management                |
| https://recovery.riotgames.com       | Riot Account Recovery                  |
| https://update-account.riotgames.com | Riot Account username disambiguation   |
| https://parents.riotgames.com        | Riot Account Parents                   |
| https://status.riotgames.com         | Riot Status                            |
| https://support.riotgames.com        | Riot Support                           |
| https://tilttypes.riotgames.com      | Tilt Types - Riot Games Player Support |
| https://merch.riotgames.com          | Riot Merch                             |
| https://developer.riotgames.com      | Riot Developer Portal                  |
| https://technology.riotgames.com     | Riot Games Technology Blog             |

#### Riot Esports

Doesn't appear to have anything yet, except for RMS and XSSO, perhaps in the future.

| Endpoint                     | Description       |
| ---------------------------- | ----------------- |
| https://riotesports.com      | Riot Esports      |
| https://xsso.riotesports.com | XSSO Riot Esports |

#### Riot KR

Lots of KR specific websites, left out for now.

#### Riot Internal

| URL                       | Description       |
| ------------------------- | ----------------- |
| https://sso.riotgames.com | Riot Internal SSO |

#### Legacy

https://engineering.riotgames.com redirects to https://technology.riotgames.com


### Public API

| Endpoint                           | Description |
| ---------------------------------- | ----------- |
| https://americas.api.riotgames.com | AMERICAS    |
| https://asia.api.riotgames.com     | ASIA        |
| https://esports.api.riotgames.com  | ESPORTS     |
| https://europe.api.riotgames.com   | EUROPE      |

#### Static Data

https://static.developer.riotgames.com


### Riot Sign On (RSO) / OAuth 2.0 authorization / OIDC authentication

Also see https://github.com/aPinat/RiotAuth.

| Endpoint                               | Description |
| -------------------------------------- | ----------- |
| https://auth.riotgames.com             | production  |
| https://garena.auth.riotgames.com      | garena      |
| https://auth.esports.rpg.riotgames.com | riottr      |

#### Legacy

| Endpoint                                  | Description |
| ----------------------------------------- | ----------- |
| https://authenticate.riotgames.com        | production  |
| https://garena.authenticate.riotgames.com | garena      |


### Riot Account

| Endpoint                          | Description                |
| --------------------------------- | -------------------------- |
| https://ap.account.riotgames.com  | Riot Account Management AP |
| https://eu.account.riotgames.com  | Riot Account Management EU |
| https://na.account.riotgames.com  | Riot Account Management NA |
| https://ap.recovery.riotgames.com | Riot Account Recovery AP   |
| https://eu.recovery.riotgames.com | Riot Account Recovery EU   |
| https://na.recovery.riotgames.com | Riot Account Recovery NA   |

#### Player Account API

| Endpoint                                      | Description    |
| --------------------------------------------- | -------------- |
| https://api.account.riotgames.com             | production     |
| https://ap.api.account.riotgames.com          | production AP  |
| https://eu.api.account.riotgames.com          | production EU  |
| https://sea.api.account.riotgames.com         | production SEA |
| https://us.api.account.riotgames.com          | production US  |
| https://use.api.account.riotgames.com         | production USE |
| https://usw.api.account.riotgames.com         | production USW |
| https://account-api.esports.rpg.riotgames.com | riottr         |

#### Legacy

https://email-verification.riotgames.com/api now handled by https://account.riotgames.com/email-verification


### Entitlements

Also see https://github.com/aPinat/RiotAuth.

`/api/token/v1`

| Endpoint                                       | Description |
| ---------------------------------------------- | ----------- |
| https://entitlements.auth.riotgames.com        | production  |
| https://entitlements.garena.auth.riotgames.com | garena      |
| https://entitlements.esports.rpg.riotgames.com | riottr      |


### Player Affinity Service (PAS)

`/pas/v1`

| Endpoint                              | Description |
| ------------------------------------- | ----------- |
| https://riot-geo.pas.si.riotgames.com | production  |
| https://pas.esports.rpg.riotgames.com | riottr      |
| https://canary.pas.si.riotgames.com   | canary      |


### Player Preferences

`/playerPref/v3`

| Endpoint                                            | Description |
| --------------------------------------------------- | ----------- |
| https://playerpreferences.riotgames.com             | production  |
| https://playerpreferences.esports.rpg.riotgames.com | riottr      |


### Client Config

`/api/v1/config`

| Endpoint                                       | Description |
| ---------------------------------------------- | ----------- |
| https://clientconfig.rpg.riotgames.com         | production  |
| https://clientconfig.esports.rpg.riotgames.com | riottr      |


### Player Platform (pp)

Also see https://github.com/aPinat/RiotAuth.

Game-agnostic, e.g. login-queue used by LoL and VALORANT. \
`https://{ROUTE}.pp.riotgames.com` are edge endpoints and proxy to their respective `https://{ROUTE}-green.pp.sgp.pvp.net` for endpoints: \
`/login-queue/v2` \
`/match-history-query/v1` \
`/session-external/v1`

| Endpoint                           | Description        |
| ---------------------------------- | ------------------ |
| https://apne.pp.riotgames.com      | AP-NorthEast proxy |
| https://apne1-green.pp.sgp.pvp.net | AP-NorthEast       |
| https://apse.pp.riotgames.com      | AP-SouthEast proxy |
| https://apse1-green.pp.sgp.pvp.net | AP-SouthEast       |
| https://euc.pp.riotgames.com       | EU-Central proxy   |
| https://euc1-green.pp.sgp.pvp.net  | EU-Central         |
| https://usw.pp.riotgames.com       | US-West proxy      |
| https://usw2-green.pp.sgp.pvp.net  | US-West            |

#### SGP

`/mailbox/v1` / `player-reporting`

| Endpoint                          | Description             |
| --------------------------------- | ----------------------- |
| https://apne.pp.sgp.riotgames.com | AP-NorthEast production |
| https://apse.pp.sgp.riotgames.com | AP-SouthEast production |
| https://euc.pp.sgp.riotgames.com  | EU-Central production   |
| https://usw.pp.sgp.riotgames.com  | US-West production      |


### Text Chat (XMPP)

| Endpoint                        | Description   |
| ------------------------------- | ------------- |
| as2.chat.si.riotgames.com:5223  | AS2           |
| br.chat.si.riotgames.com:5223   | BR1/BR/US-BR1 |
| eu3.chat.si.riotgames.com:5223  | EU3           |
| eun1.chat.si.riotgames.com:5223 | EUN1          |
| euw1.chat.si.riotgames.com:5223 | EUW1          |
| jp1.chat.si.riotgames.com:5223  | ASIA/JP1      |
| kr1.chat.si.riotgames.com:5223  | KR1           |
| la1.chat.si.riotgames.com:5223  | LA1/US        |
| la2.chat.si.riotgames.com:5223  | LA2/US-LA2    |
| na2.chat.si.riotgames.com:5223  | NA2/NA1       |
| oc1.chat.si.riotgames.com:5223  | OC1           |
| pbe1.chat.si.riotgames.com:5223 | PBE1          |
| ru1.chat.si.riotgames.com:5223  | EU/RU1        |
| sa1.chat.si.riotgames.com:5223  | SA1/SEA1      |
| sa2.chat.si.riotgames.com:5223  | SA2/SEA2      |
| sa3.chat.si.riotgames.com:5223  | SA3/SEA3      |
| sa4.chat.si.riotgames.com:5223  | SA4/SEA4      |
| tr1.chat.si.riotgames.com:5223  | TR1           |
| us2.chat.si.riotgames.com:5223  | US2           |


### Voice Chat (Vivox)

`/vts/v2`

| Endpoint                              | Description                      |
| ------------------------------------- | -------------------------------- |
| https://riot-geo.vts.si.riotgames.com | Global production (Placeholder?) |
| https://eu.vts.si.riotgames.com       | EU-Central production            |
| https://us.vts.si.riotgames.com       | US-West production               |
| https://asia.vts.si.riotgames.com     | Asia production                  |
| https://garena.vts.si.riotgames.com   | Garena production                |
| https://stage.vts.si.riotgames.com    | staging                          |


### Loyalty

`/loyalty-event-relay-service/v1/`

| Endpoint                                        | Description      |
| ----------------------------------------------- | ---------------- |
| https://eu.lers.loyalty.riotgames.com           | EU production    |
| https://northamerica.lers.loyalty.riotgames.com | NA production    |
| https://latam.lers.loyalty.riotgames.com        | LATAM production |
| https://kr.lers.loyalty.riotgames.com           | KR production    |

#### PC Bang Service (PCBS)

https://pcbs.loyalty.riotgames.com/pcbcheck/v1/pcb-status


### Riot Messaging Service (RMS)

`/rms/v1`

#### riotgames.com

| Endpoint                               | Description |
| -------------------------------------- | ----------- |
| wss://eu.edge.rms.si.riotgames.com     | EU          |
| wss://us.edge.rms.si.riotgames.com     | US          |
| wss://asia.edge.rms.si.riotgames.com   | Asia        |
| wss://sea.edge.rms.si.riotgames.com    | SEA         |
| wss://stage1.edge.rms.si.riotgames.com | stage1      |
| wss://stage2.edge.rms.si.riotgames.com | stage2      |

#### lolesports.com

| Endpoint                                | Description |
| --------------------------------------- | ----------- |
| wss://eu.edge.rms.si.lolesports.com     | EU          |
| wss://us.edge.rms.si.lolesports.com     | US          |
| wss://asia.edge.rms.si.lolesports.com   | Asia        |
| wss://sea.edge.rms.si.lolesports.com    | SEA         |
| wss://stage1.edge.rms.si.lolesports.com | stage1      |
| wss://stage2.edge.rms.si.lolesports.com | stage2      |

#### riotesports.com

| Endpoint                                 | Description |
| ---------------------------------------- | ----------- |
| wss://asia.edge.rms.si.riotesports.com   | Asia        |
| wss://eu.edge.rms.si.riotesports.com     | EU          |
| wss://sea.edge.rms.si.riotesports.com    | SEA         |
| wss://us.edge.rms.si.riotesports.com     | US          |
| wss://stage1.edge.rms.si.riotesports.com | stage1      |
| wss://stage2.edge.rms.si.riotesports.com | stage2      |



## League of Legends (LoL)

### Websites

| URL                                           | Description                         |
| --------------------------------------------- | ----------------------------------- |
| https://www.leagueoflegends.com               | League of Legends                   |
| https://login.leagueoflegends.com             | League of Legends Login             |
| https://support-leagueoflegends.riotgames.com | League of Legends Support           |
| https://pbr.leagueoflegends.com               | League of Legends Player Bug Report |
| https://universe.leagueoflegends.com          | Universe of League of Legends       |
| https://map.leagueoflegends.com               | Map of Runeterra                    |

#### Teamfight Tactics (TFT)

| URL                                            | Description               |
| ---------------------------------------------- | ------------------------- |
| https://teamfighttactics.leagueoflegends.com   | Teamfight Tactics (TFT)   |
| https://support-teamfighttactics.riotgames.com | Teamfight Tactics Support |

#### League of Legends: Wild Rift

| URL                                                   | Description                  |
| ----------------------------------------------------- | ---------------------------- |
| https://wildrift.leagueoflegends.com                  | League of Legends: Wild Rift |
| https://support-wildrift.riotgames.com                | Wild Rift Beta Support       |
| https://findyourchampion.wildrift.leagueoflegends.com | Find your Champ - Wild Rift  |

#### LoL Esports

| URL                                   | Description         |
| ------------------------------------- | ------------------- |
| https://lolesports.com                | LoL Esports         |
| https://login.lolesports.com          | LoL Esports Login   |
| https://pickem.lolesports.com         | LoL Esports Pick'em |
| https://championsqueue.lolesports.com | Champions Queue NA  |

#### Legacy

https://account.leagueoflegends.com redirects to https://account.riotgames.com.

`https://{REGION}.lolesports.com` / https://watch.lolesports.com / `https://watch.{REGION}.lolesports.com` / https://proview.lolesports.com all now redirect to https://lolesports.com.

`https://pickem.{REGION}.lolesports.com` all redirect to https://pickem.lolesports.com.

https://fantasy.lolesports.com / `https://fantasy.{REGION}.lolesports.com` was Fantasy Leagues.

https://vote.lolesports.com / `https://vote.{REGION}.lolesports.com` was All-Star Event (ASE) fan voting.

https://emp.lolesports.com shows up as `Esports Management Portal`.

https://event.lolesports.com / `https://event.{REGION}.lolesports.com` was the info page for 2017 Global Events (still functioning).


### Public API

| Endpoint                       | Description                    |
| ------------------------------ | ------------------------------ |
| https://br1.api.riotgames.com  | Brazil (BR1)                   |
| https://eun1.api.riotgames.com | EU Nordic & East (EUN1)        |
| https://euw1.api.riotgames.com | EU West (EUW1)                 |
| https://jp1.api.riotgames.com  | Japan (JP1)                    |
| https://kr.api.riotgames.com   | Korea (KR)                     |
| https://la1.api.riotgames.com  | Latin America North (LA1)      |
| https://la2.api.riotgames.com  | Latin America South (LA2)      |
| https://na1.api.riotgames.com  | North America (NA1)            |
| https://oc1.api.riotgames.com  | Oceania (OC1)                  |
| https://pbe1.api.riotgames.com | Public Beta Environment (PBE1) |
| https://ru.api.riotgames.com   | Russia (RU)                    |
| https://tr1.api.riotgames.com  | Turkey (TR1)                   |

#### Data Dragon

https://ddragon.leagueoflegends.com

#### Legacy

https://leagueconnect.api.riotgames.com was used by the old League+ app to fetch specific data from API directly, bypassing restrictions.

Public API still has `/leagueplus`-prefixed endpoints today, which the old app had used to query data without ID or PUUID encryption.


### LoLEsports API

Also see https://github.com/aPinat/RiotEsportsRewardsBot.

| Endpoint                                    | Description                     |
| ------------------------------------------- | ------------------------------- |
| https://esports-api.lolesports.com          | production                      |
| https://test-esports-api.lolesports.com     | testing                         |
| https://dev-esports-api.lolesports.com      | development                     |
| https://feed.lolesports.com                 | livestats feed                  |
| https://settings.lolesports.com             | settings                        |
| https://rex.rewards.lolesports.com          | rex rewards production          |
| https://raptor.rewards.lolesports.com       | raptor rewards production       |
| https://account.rewards.lolesports.com      | account rewards production      |
| https://entitlements.rewards.lolesports.com | entitlements rewards production |


### Player Platform (pp)

Used for `login-queue`, `match-history-query`, `session-external`.

See `Riot Games/Player Platform (pp)` above.


### New League Edge (ledge)

Also see https://github.com/aPinat/HextechAutomation.

| Endpoint                              | Description                          |
| ------------------------------------- | ------------------------------------ |
| https://br-blue.lol.sgp.pvp.net       | Brazil (BR1)                         |
| https://eune-blue.lol.sgp.pvp.net     | EU Nordic & East (EUN1)              |
| https://euw-blue.lol.sgp.pvp.net      | EU West (EUW1)                       |
| https://jp-blue.lol.sgp.pvp.net       | Japan (JP1)                          |
| https://kr-blue.lol.sgp.pvp.net       | Korea (KR)                           |
| https://lan-blue.lol.sgp.pvp.net      | Latin America North (LA1)            |
| https://las-blue.lol.sgp.pvp.net      | Latin America South (LA2)            |
| https://na-blue.lol.sgp.pvp.net       | North America (NA1)                  |
| https://oce-blue.lol.sgp.pvp.net      | Oceania (OC1)                        |
| https://pbe-red.lol.sgp.pvp.net       | Public Beta Environment (PBE1)       |
| https://ru-blue.lol.sgp.pvp.net       | Russia (RU)                          |
| https://tr-blue.lol.sgp.pvp.net       | Turkey (TR1)                         |
| https://esportstmnt01.lol.sgp.pvp.net | Esports Tournament 1 (ESPORTSTMNT01) |
| https://esportstmnt02.lol.sgp.pvp.net | Esports Tournament 2 (ESPORTSTMNT02) |
| https://esportstmnt03.lol.sgp.pvp.net | Esports Tournament 3 (ESPORTSTMNT03) |
| https://esportstmnt04.lol.sgp.pvp.net | Esports Tournament 4 (ESPORTSTMNT04) |
| https://esportstmnt05.lol.sgp.pvp.net | Esports Tournament 5 (ESPORTSTMNT05) |
| https://esportstmnt06.lol.sgp.pvp.net | Esports Tournament 6 (ESPORTSTMNT06) |


### LifeCycle Data Services (LCDS)

Adobe LiveCycle Data Services over RTMPS

| Endpoint                                          | Description                          |
| ------------------------------------------------- | ------------------------------------ |
| rtmps://prod.br.lol.riotgames.com:2099            | Brazil (BR1)                         |
| rtmps://prod.eun1.lol.riotgames.com:2099          | EU Nordic & East (EUN1)              |
| rtmps://prod.euw1.lol.riotgames.com:2099          | EU West (EUW1)                       |
| rtmps://prod.jp1.lol.riotgames.com:2099           | Japan (JP1)                          |
| rtmps://prod.kr.lol.riotgames.com:2099            | Korea (KR)                           |
| rtmps://prod.la1.lol.riotgames.com:2099           | Latin America North (LA1)            |
| rtmps://prod.la2.lol.riotgames.com:2099           | Latin America South (LA2)            |
| rtmps://prod.na2.lol.riotgames.com:2099           | North America (NA1)                  |
| rtmps://prod.oc1.lol.riotgames.com:2099           | Oceania (OC1)                        |
| rtmps://feapp.pbe1.lol.pvp.net:2099               | Public Beta Environment (PBE1)       |
| rtmps://prod.ru.lol.riotgames.com:2099            | Russia (RU)                          |
| rtmps://prod.tr.lol.riotgames.com:2099            | Turkey (TR1)                         |
| rtmps://prod.esportstmnt01.lol.riotgames.com:2099 | Esports Tournament 1 (ESPORTSTMNT01) |
| rtmps://prod.esportstmnt02.lol.riotgames.com:2099 | Esports Tournament 2 (ESPORTSTMNT02) |
| rtmps://prod.esportstmnt03.lol.riotgames.com:2099 | Esports Tournament 3 (ESPORTSTMNT03) |
| rtmps://prod.esportstmnt04.lol.riotgames.com:2099 | Esports Tournament 4 (ESPORTSTMNT04) |
| rtmps://prod.esportstmnt05.lol.riotgames.com:2099 | Esports Tournament 5 (ESPORTSTMNT05) |
| rtmps://prod.esportstmnt06.lol.riotgames.com:2099 | Esports Tournament 6 (ESPORTSTMNT06) |

### Legacy

#### Inventory Service (CAP)

`https://{REGION}.cap.riotgames.com`

Now part of New League Edge (ledge) `/lolinventoryservice-ledge/v1` and `/services/cap`.

#### Old League Edge (ledge)

`https://{REGION}.ledge.leagueoflegends.com`

See New League Edge (ledge) above.

#### Access Control System (ACS)

https://acs.leagueoflegends.com

Shutdown, previously used for match-history, which was moved to ledge, then finally now in Player Platform (pp).

#### Login Queue (LQ)

`https://lq.{REGION}.lol.riotgames.com/login-queue/rest/queues/lol/ticker` \
`https://lq.{REGION}.lol.riotgames.com/login-queue/rest/queues/lol/authenticate/RSO`

Now part of Player Platform (pp).

#### Clubs

`https://clubs.{REGION}.lol.riotgames.com`

Shutdown, feature removed.



## VALORANT [aka Ares]

### Websites

| URL                            | Description    |
| ------------------------------ | -------------- |
| https://playvalorant.com       | VALORANT       |
| https://login.playvalorant.com | VALORANT Login |
| https://xsso.playvalorant.com  | XSSO VALORANT  |

#### VALORANT Arabia

| URL                                       | Description            |
| ----------------------------------------- | ---------------------- |
| https://saitara.playvalorant.com          | VALORANT AR RETAKE     |
| https://darbetak.playvalorant.com         | VALORANT AR Rewards    |
| https://ugcbackoffice.ar.playvalorant.com | VALORANT AR Backoffice |

#### VALORANT Turkey

| URL                                       | Description            |
| ----------------------------------------- | ---------------------- |
| https://ugcbackoffice.tr.playvalorant.com | VALORANT TR Backoffice |

#### VALORANT Esports

| URL                                | Description             |
| ---------------------------------- | ----------------------- |
| https://valorantesports.com        | VALORANT Esports        |
| https://assets.valorantesports.com | VALORANT Esports Assets |
| https://xsso.valorantesports.com   | XSSO VALORANT Esports   |

#### Legacy

| URL                             | Description          |
| ------------------------------- | -------------------- |
| https://redeem.playvalorant.com | VALORANT Beta redeem |


### Public API

| Endpoint                          | Description                    |
| --------------------------------- | ------------------------------ |
| https://ap.api.riotgames.com      | Asia Pacific (AP)              |
| https://br.api.riotgames.com      | Brazil (BR)                    |
| https://esports.api.riotgames.com | Esports (ESPORTS)              |
| https://eu.api.riotgames.com      | Europe (EU)                    |
| https://kr.api.riotgames.com      | Korea (KR)                     |
| https://latam.api.riotgames.com   | Latin America (LATAM)          |
| https://na.api.riotgames.com      | North America (NA)             |
| https://pbe1.api.riotgames.com    | Public Beta Environment (PBE1) |

### Player Platform (pp)

Used for login-queue.

See `Riot Games/Player Platform (pp)`.

### Shared

`config` / `content-service` / `latency`

| Endpoint                      | Description                                               |
| ----------------------------- | --------------------------------------------------------- |
| https://shared.ap.a.pvp.net   | Asia Pacific (AP)                                         |
| https://shared.eu.a.pvp.net   | Europe (EU)                                               |
| https://shared.kr.a.pvp.net   | Korea (KR)                                                |
| https://shared.na.a.pvp.net   | North America (NA), Brazil (BR), Latin America (LATAM)    |
| https://shared.pbe.a.pvp.net  | Public Beta Environment (PBE)                             |
| https://shared.ext1.a.pvp.net | EXT1, no affinity, needs entitlement to be used, Esports? |

### Player Data (PD)

`account-xp` / `aggstats` / `contracts` / `contract-definitions` / `daily-ticket` / `favorites` / `mass-rewards` / `match-details` / `match-history` / `mmr` / `name-service` / `personalization` / `progression` / `purchase-merchant` / `restrictions` / `store`

| Endpoint                  | Description                                               |
| ------------------------- | --------------------------------------------------------- |
| https://pd.ap.a.pvp.net   | Asia Pacific (AP)                                         |
| https://pd.eu.a.pvp.net   | Europe (EU)                                               |
| https://pd.kr.a.pvp.net   | Korea (KR)                                                |
| https://pd.na.a.pvp.net   | North America (NA), Brazil (BR), Latin America (LATAM)    |
| https://pd.pbe.a.pvp.net  | Public Beta Environment (PBE)                             |
| https://pd.ext1.a.pvp.net | EXT1, no affinity, needs entitlement to be used, Esports? |

### Globalization? (GLZ)

`core-game` / `matchmaking` / `parties` / `pregame` / `session`

| Endpoint                         | Description                                               |
| -------------------------------- | --------------------------------------------------------- |
| https://glz-ap-1.ap.a.pvp.net    | Asia Pacific (AP)                                         |
| https://glz-br-1.na.a.pvp.net    | Brazil (BR)                                               |
| https://glz-eu-1.eu.a.pvp.net    | Europe (EU)                                               |
| https://glz-kr-1.kr.a.pvp.net    | Korea (KR)                                                |
| https://glz-latam-1.na.a.pvp.net | Latin America (LATAM)                                     |
| https://glz-na-1.na.a.pvp.net    | North America (NA)                                        |
| https://glz-na-1.pbe.a.pvp.net   | Public Beta Environment (PBE)                             |
| https://glz-na-1.ext1.a.pvp.net  | EXT1, no affinity, needs entitlement to be used, Esports? |

## Legends of Runeterra (LoR) [aka Bacon]

### Websites

| URL                                              | Description                  |
| ------------------------------------------------ | ---------------------------- |
| https://playruneterra.com                        | Legends of Runeterra         |
| https://support-legendsofruneterra.riotgames.com | Legends of Runeterra Support |


### Public API

| Endpoint                           | Description         |
| ---------------------------------- | ------------------- |
| https://americas.api.riotgames.com | Americas            |
| https://europe.api.riotgames.com   | Europe              |
| https://sea.api.riotgames.com      | Asia-Pacific (APAC) |

#### Legacy

| Endpoint                       | Description                          |
| ------------------------------ | ------------------------------------ |
| https://apac.api.riotgames.com | APAC (deprecated, now served by SEA) |
| https://asia.api.riotgames.com | ASIA (deprecated, now served by SEA) |

#### Data Dragon

https://dd.b.pvp.net


### Login

| Endpoint                           | Description                                 |
| ---------------------------------- | ------------------------------------------- |
| https://l-americas-green.b.pvp.net | Americas                                    |
| https://l-apac-green.b.pvp.net     | Asia-Pacific (APAC) / South East Asia (SEA) |
| https://l-europe-green.b.pvp.net   | Europe                                      |


### Services

| Endpoint                            | Description                                 |
| ----------------------------------- | ------------------------------------------- |
| https://fe-americas-green.b.pvp.net | Americas                                    |
| https://fe-apac-green.b.pvp.net     | Asia-Pacific (APAC) / South East Asia (SEA) |
| https://fe-europe-green.b.pvp.net   | Europe                                      |


### Spectate

| Endpoint                           | Description                                 |
| ---------------------------------- | ------------------------------------------- |
| https://s-americas-green.b.pvp.net | Americas                                    |
| https://s-apac-green.b.pvp.net     | Asia-Pacific (APAC) / South East Asia (SEA) |
| https://s-europe-green.b.pvp.net   | Europe                                      |



## Arcane


### Websites

| URL                     | Description |
| ----------------------- | ----------- |
| https://arcane.com      | Arcane      |
| https://xsso.arcane.com | XSSO Arcane |

#### Legacy

| URL                               | Description                             |
| --------------------------------- | --------------------------------------- |
| https://riotxarcane.riotgames.com | RiotXArcane, shutdown after event ended |


### Legacy

#### Premiere Live API (PLAPI)

`/plapi/v1/player`

| Endpoint                      | Description                                     |
| ----------------------------- | ----------------------------------------------- |
| https://plapi.prod.arcane.com | production, shutdown after premiere event ended |
| https://plapi.dev.arcane.com  | dev, shutdown after premiere event ended        |

#### RiotXArcane Missions API

https://xp1missions.riotgames.com

For how it worked, see https://github.com/aPinat/RiotArcaneMissionsBot.



## Riot Forge


### Websites

| Endpoint                                | Description                                |
| --------------------------------------- | ------------------------------------------ |
| https://riotforgegames.com              | Riot Forge Games                           |
| https://support-riotforge.riotgames.com | Riot Forge Support                         |
| https://hextechmayhem.com               | Hextech Mayhem - A League of Legends Story |
| https://ruinedking.com                  | Ruined King: A League of Legends Story™    |
| https://convrgencegame.com              | CONV/RGENCE: A LEAGUE OF LEGENDS STORY     |
| https://songofnunu.com                  | Song of Nunu: A League of Legends Story    |
