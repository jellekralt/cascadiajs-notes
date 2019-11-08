# CascadiaJS - Day 2
Friday November 8th, 2019

# Hardware Hacking for Web Developers

* Particle 
  * https://www.particle.io/
* mqtt
* serialport.io
* johnny-five
* #porgjs
  * arduino
  * optocoupler (4N35)
  * resistor
  * green led
  * cables
* JerryScript
  * Ultra-lightweight JS engine for the IoT
* Espruino
* Neonious 
  * Built in ethernet & Wifi
* Tessel 2
  * tessel.io
* Hacking Coffee Machine: htcpcp-delonghi
  * https://github.com/dkundel/htcpcp-delonghi
* Useful to have
  * Digital Multimeter
  * Breadboard
  * Pletny of jumper wires
  * Set of resisstors
  * few leds
  * few solid state relays
* d-k.im/cascadia

---

# Controlling drones with JavaScript

* RyzeTech Tello
  * $100
  * 95 gram
  * UDP interface
  * No GPS
  * Downwards facing camera
    * Visual recognition of patterns on the ground
    * Keep the drone in place
    * Track distance moved
* UDP
  * Best effort, no immediate feedback
* Mission Pads
  * Recognised by downwards facing camera
  
---

# Portable, Distributable Web Content with Web Packaging

* How to improve loading problems?
  * Improve browser engine
    * move things off-main-thread
    * optimize **ipc & process** allocation
    * optimize **memory allocation**
    * **speculatively ** start something
    * Any micro optimazations, streaming, batching, avoiding copies
  * Empower devs
    * Improve **tools** & provide incentives
    * Define **metrics** & make them available
    * Provide **apis to measure** RUM
    * Work with **frameworks**!
  * Propose & Ship Web Platform APIs
    * Change how web works today
      * Examples:
        * Prefetch
        * Preload
        * Service Worksers
        * Fetch+Streams
        * Lazyload
    * Could be most powerful but could be most difficult

- bit.ly/webpackagging

* Important Concepts
  * Web Bundles
  * Signature

- It's a format, built into browsers, specifically designed for bundling HTTP resources
  - A CBOR format with a .bn extension
  - No reliance on JavaScript to parseresources
  - Unlike MHTML: JS execution is possible
  - Uses HTTP variant for content negotiation
  - Once buundle is locally available, loading it is nearly instant

* Once you have your .wbn, they can be loaded nearly instantly\

- Use Case: Save and Share
  * Broser can provide "Save as Bundle"
  * Sites can also craft their own .wbn and provide <link rel=alternat> for better UX
  * Users then get the bundle and browse it later and/or share it with others, **no connectivity needed**

* A closer look: Signature
  * Packaging offers a way to digitally sign
* Signed HTTP exchanges = SXG
  * is a single HTTP resourece that is signed by the origin
    * Chrome support since v73
    * Can come from a cache / AMP
  
- Use case: installable & shareable PWA
  - With TWA now you can have PWA in play store,
  - however, if youre offline on the first load you get offline error
  - Even with SW, first time UX cannot be fixed and its critical

* How to create
  * recipes for devs
    * Prepare the sites source code
    * build the site
    * run the bunling tool

- Go module
  * ```go get -u github.com/WICG/webpackage/go/bundle/clmd...```

* Node.js Module
  * `wbn`
  * https://npmjs.com/package/wbn

-  gen-bundle

* wpack@ietf.org
* webpackage-dev@chromium.org
* www.chromium.org/developers
* proxx.app
* bit.ly/proxx-wbn (reqs canary 80+)




