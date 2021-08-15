# Migration from 1.1.0

#### ???
```ts
import v, { Custom } from "vimewrap";
const vimewrap = new v();

new Custom().apiTest().then(console.log);

vimewrap.custom.apiTest().then(console.log);
/*
{
  'x-ratelimit-reset-after': '12',
  'x-ratelimit-remaining': '59',
  'x-ratelimit-limit': '60'
}
{
  'x-ratelimit-reset-after': '12',
  'x-ratelimit-remaining': '58',
  'x-ratelimit-limit': '60'
}
*/
```

## Custom methods
### apiTest
1.1.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.apiTest().then(console.log);
```

1.2.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.custom.apiTest().then(console.log);
```

### parseGRank
1.1.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.parseGRank("MEMBER").then(console.log);
```

1.2.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.custom.parseGRank("MEMBER").then(console.log);
```

### parseRank
1.1.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.parseRank("MODER").then(console.log);
```

1.2.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.custom.parseRank("MODER").then(console.log);
```

## Guild methods
### get
1.1.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.guildGet({
    option: "id",
    parameter: "1"
}).then(console.log);
```

1.2.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.guild.get({
    option: "id",
    parameter: "1"
}).then(console.log);
```

### search
1.1.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.guildSearch("f5").then(console.log);

```
1.2.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.guild.search("f5").then(console.log);
```

## Leaderboard methods
### list
1.1.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.leaderboardList().then(console.log);

```
1.2.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.leaderboard.list().then(console.log);
```

## Locale
### execute
1.1.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.locale().then(console.log);
```

1.2.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.locale.execute().then(console.log);
```

## Match methods
### id
1.1.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.matchId("56171257032343552").then(console.log);
```

1.2.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.match.id("56171257032343552").then(console.log);
```

### latest
1.1.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.matchLatest().then(console.log);
```

1.2.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.match.latest().then(console.log);
```

### list
1.1.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.matchList({
    before: "185630643252625408"
}).then(console.log);
```

1.2.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.match.list({
    before: "185630643252625408"
}).then(console.log);
```

## Misc methods
### achievements
1.1.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.miscAchievements().then(console.log);
```

1.2.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.misc.achievements().then(console.log);
```

### games
1.1.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.miscGames().then(console.log);
```

1.2.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.misc.games().then(console.log);
```

### maps
1.1.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.miscMaps().then(console.log);
```

1.2.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.misc.maps().then(console.log);
```

### token
1.1.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.miscToken("DE6bkFvo7RuKw2Nnpfv3jvGEkfTQDAd").then(console.log);
```

1.2.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.misc.token("DE6bkFvo7RuKw2Nnpfv3jvGEkfTQDAd").then(console.log);
```

## Online methods
### online
1.1.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.online().then(console.log);
```

1.2.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.online.execute().then(console.log);
```

### staff
1.1.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.staff().then(console.log);
```

1.2.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.online.staff().then(console.log);
```

### streams
1.1.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.streams().then(console.log);
```

1.2.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.online.streams().then(console.log);
```

## User methods
### achievements
1.1.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.userAchievements("1").then(console.log);
// ...
vimewrap.userAchievements(1).then(console.log);
```

1.2.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.user.achievements("00000103alex", "nickname").then(console.log);
// ...
vimewrap.user.achievements("1", "id").then(console.log);
// ...
vimewrap.user.achievements(1, "id").then(console.log);
```

### friends
1.1.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.userFriends("1").then(console.log);
// ...
vimewrap.userFriends(1).then(console.log);
```

1.2.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.user.friends("00000103alex", "nickname").then(console.log);
// ...
vimewrap.user.friends("1", "id").then(console.log);
// ...
vimewrap.user.friends(1, "id").then(console.log);
```

### leaderboards
1.1.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.userLeaderboards("1").then(console.log);
// ...
vimewrap.userLeaderboards(1).then(console.log);
```

1.2.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.user.leaderboards("00000103alex", "nickname").then(console.log);
// ...
vimewrap.user.leaderboards("1", "id").then(console.log);
// ...
vimewrap.user.leaderboards(1, "id").then(console.log);
```

### matches
1.1.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.userMatches({
    id: 4167839,
    after: "57486713756319744",
    count: 1
}).then(console.log);
```

1.2.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.user.matches({
    parameter: 4167839,
    option: "id",
    after: "57486713756319744",
    count: 1
}).then(console.log);
// ...
vimewrap.user.matches({
    parameter: "FLASH_Free_STAYk",
    option: "nickname",
    after: "57486713756319744",
    count: 1
}).then(console.log);
```

### session
1.1.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.userSession("1").then(console.log);
// ...
vimewrap.userSession(1).then(console.log);
```

1.2.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.user.session("00000103alex", "nickname").then(console.log);
// ...
vimewrap.user.session("1", "id").then(console.log);
// ...
vimewrap.user.session(1, "id").then(console.log);
```

### sessions
1.1.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.userSessions("1,2,3").then(console.log);
```

1.2.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.user.sessions("1,2,3").then(console.log);
```

### sessionsPost
1.1.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.userSessionsPost([ 1, 2, 3 ]).then(console.log);
```

1.2.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.user.sessionsPost([ "00000103alex", "000Skrillex000", "002_Reptile" ], "nickname").then(console.log);
// ...
vimewrap.user.sessionsPost([ 1, 2, 3 ], "id").then(console.log);
```

### stats
1.1.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.userStats("1").then(console.log);
// ...
vimewrap.userStats(1).then(console.log);

vimewrap.userStats("1", "bw").then(console.log);
// ...
```

1.2.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.user.stats("1", "id").then(console.log);
// ...
vimewrap.user.stats("00000103alex", "nickname").then(console.log);
// ...
vimewrap.user.stats(1, "id").then(console.log);

vimewrap.user.stats("1", "id", "bw").then(console.log);
// ...
```

### userName/userId
1.1.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.userName("00000103alex").then(console.log);
// ...
vimewrap.userId("1").then(console.log);
// ...
vimewrap.userId(1).then(console.log);
```

1.2.0
```ts
import v from "vimewrap";
const vimewrap = new v();

vimewrap.user.execute("00000103alex", "nickname").then(console.log);
// ...
vimewrap.user.execute("1", "id").then(console.log);
// ...
vimewrap.user.execute(1, "id").then(console.log);

vimewrap.user.execute("1,2,3", "id").then(console.log);
// ...
vimewrap.user.execute("00000103alex,000Skrillex000,002_Reptile", "nickname").then(console.log);
```