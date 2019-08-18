---
layout: post
title: "devICT Presents: Cypress (End to End Testing Tool)"
categories: [talks, devict]
tags: [cypress, testing, integration testing]
---

      ![devICT](http://devict.org/images/devICT-Logo.svg)
      # Cypress - End to End Testing Tool
      ### cypress.io
      Sandip Southekal

      ---

      # Agenda

      - Why another integration testing tool?
      - Features
      - Really interesting features
      - Examples

      ---

      # Why?
      - Importance of integration tests
        - unit tests can give you a false sense of security
        - ...and most were actually integration tests

      - What about selenium?
        - requires custom handlers: page load waits, clickable buttons etc
        - treated as a separate entity

      - TDD on steroids: debugger/network monitoring/stubs

      ---

      # Features
      - Single library install
        - no other dependencies eg: chromedriver, requests, BeautifulSoup
      - Philosophy difference: `Selenium` vs `Cypress`
        - **selenium** - externally controls the browser through remote commands
        - **cypress** - node.js server process allowing it to operate at the network layer and alter requests.
      - Syntax uses familiar javascript testing tools
        - understands mocha, chai
        - eg: `describe, it`
      - Out of the box dashboard
        - debugging
        - screenshots and videos
      - Runs against `chrome`, `canary`, `chromium`, `electron headless`

      ---

      # Interesting Features
      - hot reload
      - **fixtures**: keeps test repeatable with known and fixed values
      - can write in `.js`, `.jsx`, `.coffee`, `.cjsx` and `.ts`
      - can forcibly fire events such as `click`
      - blacklist hosts
      - stub responses
      - **clock**: control `setInterval` or `throttling`. can put you ahead by 'x' sec

      #### <u>Additional Notes:</u>
      - no ability to tag tests
      - no `firefox`, `IE` support
      - ordering of tests when running in parallel is not guaranteed

      ---

      # Examples
      - devict.org
      - visit homepage => click on banner => verify about page
      - visit homepage => verify slack url
      - beforeEach and afterEach
      - visit code of conduct => verify form action, form fill
      - verify videos are visible => tags are present
      - verify catching javascript errors

      #### <u>Not discussed:</u>
      - Parallelization
      - Continuous Integration
