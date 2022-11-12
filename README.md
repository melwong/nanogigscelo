Nano Gigs
-----------------------------

A gig economy platform that empowers people to request and respond to help by doing little tasks called "nano gigs." Responders are rewarded with crypto tokens as a token of appreciation. This token can be withdrawn (cash out), if allowed.

It is highly customisable with many awesome features:

- Asking and answering help.
- Voting, comments, best help selection, follow-on and closed requests.
- Complete user management including token-based management.
- Create experts, editors, moderators and admins.
- Fast integrated search engine.
- Categories (up to 4 levels deep) and/or tagging.
- Easy styling with CSS themes.
- Supports translation into any language.
- Custom sidebar, widgets, pages and links.
- SEO features such as neat URLs, microformats and XML Sitemaps.
- User avatars (or Gravatar) and custom fields.
- Private messaging.
- Custom single sign-on support for other sites.
- PHP/MySQL scalable to millions of users and posts.
- Safe from XSS, CSRF and SQL injection attacks.
- Beat spam with captchas, rate-limiting, moderation and/or flagging.
- Block users, IP addresses, and censor words

## How to install

- Clone this repo.
- Create a MySQL database, and a MySQL user with full permissions for that database. If you're interested, the privileges actually needed are: CREATE, ALTER, DELETE, INSERT, SELECT, UPDATE, LOCK TABLES. Note down the MySQL details: username, password, database name and server host name. If MySQL is running on the same server as your website, the server host name is likely to be 127.0.0.1 or localhost.
- Open qa-config.php in your text editor, insert the MySQL details at the top, and save the file. Do not use a word processor such as Microsoft Word for this, but rather Notepad or another appropriate text editing program.
- Go to installers folder and run the sql_to_run.sql file in your MySQL IDE or Phpmyadmin.
- Go to browser and run the site. That's it.

## How to deploy the smart contract on Celo

- To set up your Metamask with Celo testnet, just go to https://chainlist.org and search for "Celo Alfajores Testnet" and click on the "Connect Metamask" button. 
- Go get some test CELO tokens for Celo Testnet. Go to -> https://celo.org/developers/faucet
- Go to installers folder at the installation and open NanoGigs.sol with text editor. Copy the entire code.
- Visit https://remix.ethereum.org and create a new contract file. Call it NanoGigs.sol
- Paste the code you copied on the file.
- Compile the code.
- Deploy the code on Aurora and copy the contract address.
- At the installation folder, go to qa-theme/lion/js/web3-connector.js and at line 18 to 20, enter your wallet address and contract details.

## How to use
Watch this video -> https://youtu.be/L4dynaSivxQ

----------

This code is based on [Question2Answer][Q2A] and it is also GPL licensed. Instead of reinventing the wheel from scratch, we reused existing robust and production-ready [Question2Answer][Q2A] code and build on top of it to ensure minimum bugs and vulnerabilities.


[Q2A]: http://www.question2answer.org/
