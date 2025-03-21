# stacks-marketplace-bitcoin
This repository hosts the source code for a decentralized marketplace powered by the Bitcoin Stacks blockchain, allowing users to securely buy, sell, and trade digital assets in a decentralized environment.

## Project Structure

### Contracts
contracts.clar file
```
;; title: gor
;; version:
;; summary:
;; description:

;; traits
;;

;; token definitions
;; 

;; constants
;;
(define-constant price1 u2)
(define-constant price2 u1)
(define-constant price3 u3)
(define-constant price4 u5)

;; data vars
;;
(define-map listings
    uint
    {
        name: (string-ascii 20),
        pno: uint,
        quantity: uint,
        amount: uint,
        purchase-time: uint,
    }
)

(define-data-var listing-nonce uint u0)
;; data maps
;;

;; public functions
;;
(define-public (hello-world) 
 (ok (print "Hello World!")))
;; read only functions
;;

;; private functions
;;
```

### Settings
Devnet.toml
```
[network]
name = "devnet"
deployment_fee_rate = 10

[accounts.deployer]
mnemonic = "twice kind fence tip hidden tilt action fragile skin nothing glory cousin green tomorrow spring wrist shed math olympic multiply hip blue scout claw"
balance = 100_000_000_000_000
# secret_key: xxx
# stx_address: xxx
# btc_address: xxx

[accounts.wallet_1]
mnemonic = "sell invite acquire kitten bamboo drastic jelly vivid peace spawn twice guilt pave pen trash pretty park cube fragile unaware remain midnight betray rebuild"
balance = 100_000_000_000_000
# secret_key: xxx
# stx_address: xxx
# btc_address: xxx

[accounts.wallet_2]
mnemonic = "hold excess usual excess ring elephant install account glad dry fragile donkey gaze humble truck breeze nation gasp vacuum limb head keep delay hospital"
balance = 100_000_000_000_000

[accounts.wallet_3]
mnemonic = "cycle puppy glare enroll cost improve round trend wrist mushroom scorpion tower claim oppose clever elephant dinosaur eight problem before frozen dune wagon high"
balance = 100_000_000_000_000

[accounts.wallet_4]
mnemonic = "board list obtain sugar hour worth raven scout denial thunder horse logic fury scorpion fold genuine phrase wealth news aim below celery when cabin"
balance = 100_000_000_000_000

[accounts.wallet_5]
mnemonic = "hurry aunt blame peanut heavy update captain human rice crime juice adult scale device promote vast project quiz unit note reform update climb purchase"
balance = 100_000_000_000_000

[accounts.wallet_6]
mnemonic = "area desk dutch sign gold cricket dawn toward giggle vibrant indoor bench warfare wagon number tiny universe sand talk dilemma pottery bone trap buddy"
balance = 100_000_000_000_000

[accounts.wallet_7]
mnemonic = "prevent gallery kind limb income control noise together echo rival record wedding sense uncover school version force bleak nuclear include danger skirt enact arrow"
balance = 100_000_000_000_000

[accounts.wallet_8]
mnemonic = "female adjust gallery certain visit token during great side clown fitness like hurt clip knife warm bench start reunion globe detail dream depend fortune"
balance = 100_000_000_000_000

[accounts.faucet]
mnemonic = "shadow private easily thought say logic fault paddle word top book during ignore notable orange flight clock image wealth health outside kitten belt reform"
balance = 100_000_000_000_000

[devnet]
disable_stacks_explorer = false
disable_stacks_api = false

# Send some stacking orders
[[devnet.pox_stacking_orders]]
start_at_cycle = 3
duration = 12
wallet = "wallet_1"
slots = 2
btc_address = "mr1iPkD9N3RJZZxXRk7xF9d36gffa6exNC"

[[devnet.pox_stacking_orders]]
start_at_cycle = 3
duration = 12
wallet = "wallet_2"
slots = 1
btc_address = "muYdXKmX9bByAueDe6KFfHd5Ff1gdN9ErG"

[[devnet.pox_stacking_orders]]
start_at_cycle = 3
duration = 12
wallet = "wallet_3"
slots = 1
btc_address = "mvZtbibDAAA3WLpY7zXXFqRa3T4XSknBX7"
```

### Clarinet.toml
```
[project]
name = 'contract'
description = ''
authors = []
telemetry = false
cache_dir = './.cache'
requirements = []
[contracts.contract]
path = 'contracts/contract.clar'
clarity_version = 1
epoch = 2.0
[repl.analysis]
passes = ['check_checker']

[repl.analysis.check_checker]
strict = false
trusted_sender = false
trusted_caller = false
callee_filter = false
```

## Contact Me
LinkedIn: [@Ljubomir Igic](https://www.linkedin.com/in/ljubomir-igic-6a9615340)

Telegram: [@Ljubomir Igic](https://t.me/@ljubomir_igic)
