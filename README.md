# townlist.api
Official API for the known townlist.tk, this module can be used for many stuff. Especially sending stats.


**NPM:** [npmjs.com/package/townlist.api](https://www.npmjs.com/package/townlist.api/)<br>



<a href="https://nodei.co/npm/townlist.api"><img src="https://nodei.co/npm/townlist.api.png?downloads=true&stars=true" alt="npm installnfo" /></a>


## Installation
*If you have trouble with the installation, please feel free to visit our [discord](https://townlist.tk/dc) address.*
- `npm i listing-dtl-api`

#### 1. Where can I get townlist.tk API?
  [JavaScript Package](https://www.npmjs.com/package/townlist.api)
            

#### 2. How do I install it?
 `npm i townlist.api or npm install townlist.api`
          

#### 3. Does it have any GitHub Repository?
 Yes

#### 4. What is it's uses?
  Ans: To get the daily vote count, server count and information about your bot.
Examples:  avatar, botID, discriminator, shortDescription, prefix, votes, serverCount, ownerID, owner, co-owners, tags, longDescription, certificate etc.

#### 5. How can I get my bot's server count?
  `JavaScript:`
```js
const dtl = require("townlist.api");
const dbl = new dtl("TOKEN-HERE", client);

client.on("ready", async () => {
  dbl.serverCount();
});
```

#### 6. How can I get my bot's vote count?
  `Ans:`
```js
let hasVote = await dbl.hasVoted("Your-bot-id");
  if(hasVote === true) {
    console.log("Voted")
  } else {
    console.log("Vote please.")
  }
  
  
  let search = await dbl.search("Your-bot-id")
  console.log(search)

```

#### 7. Full Example?
```js
const dtl = require("townlist.api");
const dbl = new dtl("TOKEN-HERE", client);

client.on("ready", async () => {
  dbl.serverCount();
  console.log("Server count posted")
  
  let hasVote = await dbl.hasVoted("your-bot-id");
  if(hasVote === true) {
    console.log("Voted")
  } else {
    console.log("Vote please.")
  }
  
  
  let search = await dbl.search("townlist.api")
  console.log(search)

  /* SearchResults
  {
    avatar: '',
    botID: '',
    username: '',
    discrim: '',
    shortDesc: '',
    prefix: '? [changable]',
    votes: 25,
    ownerID: '',
    owner: '',
    coowners: [ '' ],
    tags: [ 'Moderation', 'NSFW', 'Music' ],
    longDesc: longDesc,
    certificate: 'Certified'
  }
  */
});
```
### More Updates
# Updates will be here, also the docs
[Click the link](<https://api.townlist.tk>)
