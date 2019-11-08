# CascadiaJS - Day 1
Thursday November 7th, 2019

# Codemods
* jscodeshift (facebook) -> check out 
* Recast -> Parse and manipulate code -> AST to AST 
* AST explorer
* `react-javascript-to-typescript-transformers`

-------

# Perf budgets
* Milestone
* Quantity
* Rules

* Building Sandspiel - an Interactive WebAssembly experience
	* [Building Sandspiel - an Interactive WebAssembly experience, Max Bittker - YouTube](https://www.youtube.com/watch?v=sh6lIuX4Hzc)

* Ubiquitous
* Mobile Only
* Localize

* WebAssembly 
	* Offers predictable perf
	* Is extremely portable

* Wasm by example

* When should you be using web workers
	* [When should you be using Web Workers? — DasSur.ma](https://dassur.ma/things/when-workers/)

* Workbox
	* https://developers.google.com/web/tools/workbox
* Preact
	* [Preact](https://preactjs.com/)
* https://webassembly.sh/

--------

# Kafka
* Offline persistance

* Kafka = Post Office
* Producer = Sender
* Consumer = Receiver
* Topic = PO Box Wall
	* Partitions = PO boxes
	* Messages = Mail

* Netflix > 6 Petabytes / day

* `kafka-node`
	* https://github.com/SOHU-Co/kafka-node

* Kafka + Docker
	* `kafka-docker`

* Kafka Pub Sub
	* Pub Sub wrapper around `kafka-node`
	* https://github.com/NeuCleans/kafka-pub-sub

* Takeway Resources
	* https://podplayer.net/?id=82304318
	* https://kafka-tutorials.confluent.io
	* https://www.youtube.com/watch?v=udnX21__SuU
	* https://www.youtube.com/watch?v=UEg40Te8pnE
	* https://kafka.apache.org

---

# Programming the Cloud with JavaScript
* Issue with Droplets
	* Cant see whats inside
	* Can't duplicate it
	* Cant scale it out easily
	* Can't recover from disaster

* Types of Tools
	* Configuration management
		* Chef 
		* Puppet
		* Ansible
		* SaltStack
	* Provisioning
		* Terraform
		* AWS CloudFormation
		* Azure Resource Manager

* They're declarative: we express the *what* an the tools determine the *how*

* Reliable
* Repeatable
* Replicable
* Testable
* Self documentational

* App-friendly resources
	* Function
	* Table
	* Event Record
	* Route

* AWS Cloud Development Kit
	* Javascript
* Pulumi



## Questions
* Does it "auto-generate" resources for you in the cloud?
	* If it does, How do you deal with costs?
	* If it doesnt, do you have to "define" all the resources by hand upfront?
	* Or are there budgets or limits?


# Portable, Distributed Web Content with Web Packaging
* https://blog.cloudflare.com/the-road-to-quic/
* Benefits HTTP/2
	* Multiplexing and concurrency
	* Stream dependencies
	* Header compression
	* Server push
* Why HTTP/3
	* TCP head-of-line blocking
		* http3-explained.haxx.se/en/why-tcphol.html
* HTTP/3 over QUIC
	* QUIC is built on UDP
	* Protocols don't update that fast -> routes don't get replaced quickly
* HTTP/3 IETF draft
* https://github.com/nodejs/quic

---

# Several ways to construct an object
* bit.ly/several-ways

----

# Binary encoding in JavaScript
* github.com/cztomsik/graffiti
* github.com/servo/bincode
* WASM understands only number and binary data (at least today)
* Avoid encoding strings into utf-8. It is slow
* Look up SharedArrayBuffer

---

# App Not Ejected Properly
https://github.com/giladgray/ejected-react-app

----

#  How User Centered Build Time Integration Tests Benefit You and Your Users
* Immediate feedback
	- build time
* Isolated to code
	* Network isolation
* User interactions
	* test all units of application together

* Puppeteer Request Interception
* Nock library

* Axe-puppeteer

* User centered build time integration tests
	* Gives devs fast, actionable feedback
	* Test if users can achieve the goal

---

# Fair Trade Open Source















