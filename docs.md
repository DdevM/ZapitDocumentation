## Documentation


## CodeFiles and Uses

This hold the codefiles of all folders and their usage.

### Components

#### Buttons

* CustomIconButton and CustomButtons (Used in almost everywhere on screen, Rounded big buttons and Icon Buttons during transaction)
* CachedImageNetwork and AnimatedProgressIndicator (Used in nft Screen and splConfirmTransaction) 
* MyextFormField (Used in transaction sending and Address Coverter text boxes)
* MyTextFormFieldMulti (Not Used)
* MyTextFormFieldPrefixSuffix (Used in screen profile {The screen when tapped on username on homeScreen})
* ImageIdentification (Used in rendering images like assets, nfts etc.)
* Virtual Keyboard (Not Used yet, Complete Virtual keyboard that can override the default keyboard)

#### Switches
* Animated CustomSwitch (Not Used)

* BaseAppBar (Customisation of appbar based on the color values, Used almost everywhere)
* SwipeButton (Custom Animated SwipeButton both with the outer container as well as the inner circle drag behaviour)

### Core

#### App Colors
Contains all the colors of different opacities used inside of app

#### App Dimes
Contains margins (0-1200) and textSizes (8-72)

#### App Fonts
Fonts used in apps as well as some of the popular text Theme colors

#### App Images
Contains base urls i.e. assetUrls and all other required images

#### App Strings 
Contains all the static texts used inside of the application

#### Core Imports
Contains the core imports or exports

#### Extension
Extension classes developed on Strings in order to validate password, number and email.

## Screens

#### Assets
Contains the code for the assets screen on the homeScreen
It fetches the initial token data from the Hive DB and sets all the state properties accordingly per each token.
It has a slptokencard function that returns the widget holding the token data

#### Bch
* It is holding the transaction screen the view add contact is the bottom sheet that appears on clicking on add new contact
* Bch utils holds the explorers and links of various blockchain domaisn
* Cash account holds the cash account page in which it fetches the data from HiveDB in order to check for existing address and stores the data in the state.
  - Create new cash account takes in a username and creates the cash account.
  - Contains functions like show success modals etc.
* Confirm Transaction is the page that is hown up before transaction is done
  - At start it fetches the reciever and sender address along with BCH fees from bitbox and discounts from Hive DB
  - Doubt (wif)
  - Send Discounted transactions
* Discount screen consists of the discounts page where it fetches the discount available in different tokens from the DB and then verifies the discounts and adds it up.
* Edit Contact Screen takes in all the required parameters as arguments and allows editing option and pushes the contact back to DB
* Enter amount is a textfield that takes the fiat currency input and then gets the corresponding BCH price and then checks for sufficient balance in sender's account and functions accordingly, to go to Navigation page / Show error
* Recieve page is the page we see when we click on the username on the home page. The BCH address / Cash Account details of the user is fetched from the DB along with forming the QR accordingly if SLP or BCH.
* Scan consists of the QR code controller, decoding the qr, and checking if the address belongs to an user, checking if the id has a cash account or is a SLP id and accordingly execute the function and send data.
* Send consists of the send page along with the contact details. It fetches the user bch / SLP address and then it also checks and ahndles the transaction part. i.e. if the transaction is done by manually entering the address or if it is from a QR code and if it is from a QR code then decode the address to a valid BCH address and execute the transaction.
* 
