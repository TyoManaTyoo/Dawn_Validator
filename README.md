# DAWN Validator Extension automatic claim

## What needed
- Node JS

## Features

- Automatically send keep-alive requests to claim points.
- Multi-account.
- Auto loop.
- Proxy support.


## Installing and setup

### Install
1. Clone the project and go to project directory
   ```
   git clone https://github.com/TyoManaTyoo/Dawn_Validator
   ```
   ```
   cd Dawn_Validator
   ```
2. Install required package
   ```
   npm install
   ```
   or
   ```
   npm i
   ```
### Setup and run

1. Login/register Dawn Validator account and login, get the token in "getpoint?appid=" -> "authorization:" at network tab in inspect element in browser. 
2. In `dawn-validator` directory, Edit and adjust this line in `account.js` and save it
	```
	// accounts.js
	module.exports = [
		{ email: "user1@example.com", token: "token1" },
		{ email: "user2@example.com", token: "token2" },
		// Add more accounts as needed
	];
	```
3. Edit and adjust the `config.js` for proxy and delay options.
	```
	// config.js
	module.exports = {
		useProxy: false, // Set to true if you want to run with proxies
		minDelay: 3,
		maxDelay: 10,
		restartDelay: 160,
	};
	```
4. Edit the `proxy.js` if you want to use proxy
5. Run the script to start, use :
    ```
    node index.js
    ```
	
	
	
Dawn Validator Extension : https://chromewebstore.google.com/detail/dawn-validator-chrome-ext/fpdkjdnhkakefebpekbdhillbhonfjjp?authuser=0&hl=en

My reff code if you want :) : 9lv10g33
