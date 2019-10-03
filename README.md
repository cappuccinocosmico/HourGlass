# hugoBasicExample

This is an example site for [Hugo](https://gohugo.io/).

It is intended to be a demo site for the various [Hugo themes](https://themes.gohugo.io/).

# Using

1. [Install Hugo](https://gohugo.io/overview/installing/)
2. Clone this repository
```bash
git clone https://github.com/gohugoio/hugoBasicExample.git
cd hugoBasicExample
```
3. Clone the repository you want to test. If you want to test all hugo themes, you can clone [the full list](https://github.com/gohugoio/hugoThemes)
```bash
git clone --recursive https://URL/OF/YOUR/THEME themes/YOURTHEME
```
or
```bash
git clone --recursive https://github.com/gohugoio/hugoThemes.git themes
```
4. Run Hugo and select the theme of your choosing
```bash
hugo server -t YOURTHEME
```

# HourGlass

HourGlass is a alpha test of a Payment System based on the stellar network, that's being floated for XR Denver for their financial needs.

https://pad.riseup.net/p/SjZB-1j27BJd6qnsNbW-

## What is it and how the hell does it work?

### What is a crypto currency?

A cryptocurrency is a decentralised cryptographicly secure distributed leger payment system. _For more explanation on how this works I highly recommend this vido by 3b1b:<https://youtu.be/bBC-nXj3Ng4?t=130>, however because stellar uses quorum slices, the the last part of the video after 11:38, doesn't really apply, still worth watching though._

However what makes stellar different from a lot of other currencies is its consensus protocol (Called Federated Byzantine Consensus (FBZ)), it differs from a lot from other consensus protocols in that.

1. The algorithm doesnt require burning mountains of fossil fuels to power its consensus protocol. (See essentially any other cryptocurrency.(Bitcoin/Ethereum/Bitcoin Cash))
2. It has the ability to process way more transactions per second then any other protocol 1-2k tps for Stellar and Ripple, compared to 7-14 for Bitcoin and Ethereum (other solutions like Bitcoin Cash can get up to 100, but its still way short of the amount achievable by FBZ)
3. Transaction fees are quite low (1$ right now covers about 2 million transactions.) _Math Nerd Zone: Its also really intresting because to FBZ is really fundamentaly different from the other 2 most popular consensus protocols (Proof of Work and Proof of Stake), its both more simple and more complicated because POS and POW are both really simple in the sense that they work by trust whatever ledger took more power or money to produce. While FBZ uses this really intresting math to throw gaurentee this stuff, If you happen to be intrested I highly reccommend you read the whitepaper (beware the first 4 pages are hype, actual math is page 4 onwards.):<https://www.stellar.org/papers/stellar-consensus-protocol.pdf>_

### Why are we using cryptocurrencies instead of something simpler?

  <https://www.smbc-comics.com/index.php?id=2088>

But in all seriousness, there are several advantages.

1. This prevents serious financial fraud. There are tons of horror stories on the internet about non-profits and other small organisations getting defrauded because someone on their financial team was a bad actor. Most of the security comes from the fact that the books are psudo-public, (<https://www.profwoodward.org/2016/01/blog-post_30.html>), its possible to tell from the outside if its committing fraud (at least hypothetically).

2. It makes it possible to make payments to anyone on keybase. This is useful because with any other system they would all have to sign up for new accounts with some payment service, such as paypal or something. Whereas everyone on keybase can receive value in this way.

3. It makes it so that we control our own means of distribution compared to having a bank control our assets, (might be important police confiscation of money and stuff)

## Cool I am a user, how do I get reimbursed.

##### 1. Technical Stuff
So the first thing to do is to open a terminal on a computer where you have keybase installed, and type this command.

`keybase wallet add-trustline -a XRDENVER_ACCOUNT_ID -c HourGlass`

 **NEVER EVER TYPE IN COMMANDS TO A TERMINAL THAT YOU FOUND OFF THE INTERNET UNLESS YOU KNOW WHAT THEY DO**

 This will add a trustline to your main keybase account, that will allow you to receive money from XR.

 _In order to execute this command you will need to have a little bit of money in your main keybase account (about 25 cents should be fine), if you dont have it someone in the group probably has some laying around._

##### 2. Actual Reimbursement
The next step is to send some kind of proof of purchase in a direct chat to the keybase user XRDENVER_KEYBASE_ID (or some kind of secure form (we arent 100% certain about this)), and then you are done. If its valid the tokens will be sent your way.

### So I am a user who got reimbursed with these tokens what do I do with them?

  Once you have these HourGlass Tokens, they can be reimbursed in a multitude of ways.
##### 1. Direct Exchange
Its possible to reimburse these HourGlass tokens for 1 dollar a token by meeting any of the xr denver infrastructure team.

##### 2. Stellar Integration
There should be a bot set up with [kelp](https://github.com/stellar/kelp), that should keep the price of a HourGlass priced at the equivalent of 1 dollar worth of lumens. This makes it possible to redeem HourGlass for any other asset on the stellar network.

##### 3. Online Payment Reimbursement (Not Implemented)
There might be a system set up in the future that would integrate with an online payment service (paypal or amazon or somthing else), to allow automatic reimbursement.
