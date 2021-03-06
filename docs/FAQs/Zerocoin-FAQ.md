# Zerocoin FAQ


##### Q: What is the Zerocoin Protocol? 

A: The Zerocoin Protocol is a privacy protocol that can be applied to cryptocurrency, utilizing advanced cryptography to hide the transaction history of any coin that has been passed through the "Zerocoin system"

##### Q: How does it work?

A: The simplest explanation is that the Zerocoin Protocol allows users to burn their BWK and get zBWK in exchange. zBWK is an I.O.U on the network that can be spent as normal BWK.  
When you want to initiate a spend, your wallet sends a zero-knowledge proof to the blockchain that allows fresh BWK to be created by the network which replaces the burnt BWK, but with no transaction history, essentially "washing" the coins.  
You can even instruct the network to send the redeemed BWK to a 3rd party address, to completely hide who sent the BWK to the recipient!

##### Q: So how do I convert BWK to zBWK?

A: Its very easy. Simply go to the `privacy` tab in your wallet, enter an amount in the `mint zerocoin` text box, click `mint zerocoin` and your coins will be in the que, waiting for confirmations. When it is in this que, it is waiting for confirmations and maturity, 20 confirmations on the network, and at least one other mint in the same denomination or denominations.

##### Q: How do I spend zBWK?

A: The process is very similar to sending a normal transaction. In the privacy tab, you will find a familiar field in the bottom-left which lets you choose denominations to spend, enter an amount, and choose an address. Then you can click send to either receive zBWK as BWK yourself, or send BWK anonymously to someone else.

##### Q: Security Levels? What are these?

A: The security level is a balancing act between being able to spend zBWK quicker, and better hiding your denominations amongst others. A Security Level of 1, for example, would take all of the minted coins in the block chain before your mint was added to the block chain, and would then add any coins that were minted within the next 10 blocks as well. A Security Level of 3 would do the same thing, except add the next 30 blocks worth of mints. A Security Level of 100 will add the maximum amount of mints up to the current end of the block chain.

Therefore, you should adjust the security level accordingly with the level of anonymity requires. The default for our wallet is 42, and this provides a good balance that should be fast and secure.

##### Q: What are denominations, and why can I only mint zBWK in specific amounts?

A: Specific denominations are used to decrease the time it takes to approve your mint on the blockchain. Since every mint needs to have one more mint come after it before it is verified, allowing people to mint any amount they like would potential lock coins in a perpetual state of "confirming". Utilizing specified denominations nearly eliminates the risk that minted coins will never be confirmed. The denominations used by zBWK are: 1, 5, 10, 50, 100, 500, and 1000. We made the decision to remove the 5000 denomination that PIVX utilizes to increase liquidity at the expense of large zBWK transactions requiring more mints. We feel that the benefit to users with smaller balances outweighs the potential downside to extremely large users. 

##### Q: How is this better than Obfuscation or CoinJoin?

A: To quote our blog post on our release of Zerocoin; "Firstly, the effectiveness of PrivateSend is dictated by how many people are currently taking part in the obfuscation process, therefore it can take weeks to obfuscate large balances depending on the liquidity at the time. Zerocoin massively cuts down on this time by not requiring there to be multiple people taking part in the mixing process.

Another core problem is recent research results with regards to how safe CoinJoin-based systems (such as PrivateSend) actually are. Studies have revealed that merchant cookies and cluster intersection attacks when combined can actually reveal the identity of who purchased X item online, and can even result in unidentified people linking your person to your public key. One of the 1st points we make in our whitepaper is that we intend to adopt best-practices to ensure Bulwark is as good if not better than all other privacy offerings on the market, and implementing Zerocoin is in perfect alignment with this."

##### Q: Do you have a video guide for all this?

A: We do indeed!

<div class="video-wrapper">
<iframe width="560" height="315" src="https://www.youtube.com/embed/iU6jD22_kqM" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>