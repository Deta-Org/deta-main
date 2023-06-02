<p align="center"><img src="https://s3.amazonaws.com/deta-assets/logo_large_white.png" width="256" /></p>

<div align="center">
  <a href="https://circleci.com/gh/detaprotocol/workflows/perpetual/tree/master" style="text-decoration:none;">
    <img src="https://img.shields.io/circleci/project/github/detaprotocol/perpetual.svg" alt='CI Status' />
  </a>
  <a href='https://www.npmjs.com/package/@detaprotocol/perpetual' style="text-decoration:none;">
    <img src='https://img.shields.io/npm/v/@detaprotocol/perpetual.svg' alt='NPM' />
  </a>
  <a href='https://coveralls.io/github/detaprotocol/perpetual' style="text-decoration:none;">
    <img src='https://coveralls.io/repos/github/detaprotocol/perpetual/badge.svg?t=cPGDk7' alt='Coverage Status' />
  </a>
  <a href='https://github.com/detaprotocol/perpetual/blob/master/LICENSE' style="text-decoration:none;">
    <img src='https://img.shields.io/github/license/detaprotocol/protocol.svg?longCache=true' alt='License' />
  </a>
  <a href='https://t.me/joinchat/GBnMlBb9mQblQck2pThTgw' style="text-decoration:none;">
    <img src='https://img.shields.io/badge/chat-on%20telegram-9cf.svg?longCache=true' alt='Telegram' />
  </a>
</div>

> Ethereum Smart Contracts and TypeScript client library for the deta Perpetual Contracts Protocol. Currently used by [trade.deta.exchange](https://trade.deta.exchange).

**Full Documentation at [docs.deta.exchange](https://docs.deta.exchange).**

## Table of Contents

 - [Documentation](#documentation)
 - [Install](#install)
 - [Contracts](#contracts)
 - [Security](#security)
 - [Development](#development)
 - [Maintainers](#maintainers)
 - [License](#license)

## Documentation

Check out our full documentation at [docs.deta.exchange](https://docs.deta.exchange):
* [Protocol Overview](https://docs.deta.exchange/#/perpetual-protocol)
* [Perpetual Guide and Contract Specification](https://docs.deta.exchange/#/perpetual-guide)

## Install

`npm i -s @detaprotocol/perpetual`

## Contracts

The current contract addresses can be found in the [`migrations/deployed.json`](https://github.com/detaprotocol/perpetual/blob/master/migrations/deployed.json) file.

## Security

### Independent Audits

The smart contracts were audited independently by
[Zeppelin Solutions](https://zeppelin.solutions/) at commit [`c5e2b0e`](https://github.com/detaprotocol/perpetual/tree/c5e2b0e58aaf532d2c8b1f658d1df2f6a3385318/contracts), excluding [`P1Orders.sol`](contracts/protocol/v1/P1Orders.sol).

**[Zeppelin Solutions Audit Report](https://blog.openzeppelin.com/deta-perpetual-audit/)**

### Code Coverage

All production smart contracts are tested and have 100% line and branch coverage.

### Vulnerability Disclosure Policy

The disclosure of security vulnerabilities helps us ensure the security of our users.

**How to report a security vulnerability?**

If you believe you’ve found a security vulnerability in one of our contracts or platforms,
send it to us by emailing [security@deta.exchange](mailto:security@deta.exchange).
Please include the following details with your report:

* A description of the location and potential impact of the vulnerability.

* A detailed description of the steps required to reproduce the vulnerability.

**Scope**

Any vulnerability not previously disclosed by us or our independent auditors in their reports.

**Guidelines**

We require that all reporters:

* Make every effort to avoid privacy violations, degradation of user experience,
disruption to production systems, and destruction of data during security testing.

* Use the identified communication channels to report vulnerability information to us.

* Keep information about any vulnerabilities you’ve discovered confidential between yourself and
deta until we’ve had 30 days to resolve the issue.

If you follow these guidelines when reporting an issue to us, we commit to:

* Not pursue or support any legal action related to your findings.

* Work with you to understand and resolve the issue quickly
(including an initial confirmation of your report within 72 hours of submission).

* Grant a monetary reward based on the [OWASP risk assessment methodology](https://medium.com/detaderivatives/announcing-bug-bounties-for-the-deta-margin-trading-protocol-d0c817d1cda4).


## Development

### Compile Contracts

Requires a running [docker](https://docker.com) engine.

`npm run build`

### Compile TypeScript

`npm run build:js`

### Test

Requires a running [docker](https://docker.com) engine.

**Start test node:**

`docker-compose up`

**Deploy contracts to test node & run tests:**

`npm test`

**Just run tests (contracts must already be deployed to test node):**

`npm run test_only`

**Just deploy contracts to test node:**

`npm run deploy_test`

## Maintainers

 - **Brendan Chou**
 [@brendanchou](https://github.com/BrendanChou)
 [`brendan@deta.exchange`](mailto:brendan@deta.exchange)

 - **Ken Schiller**
 [@kenadia](https://github.com/Kenadia)
 [`ken@deta.exchange`](mailto:ken@deta.exchange)

## License

[Apache-2.0](./blob/master/LICENSE)
