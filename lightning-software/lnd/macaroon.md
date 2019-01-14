---
latest-revision: '1999-01-29T00:00:00.000Z'
original-author: >-
  Isaac Newton (@appleman) < List of Original Authors' Real Name and Github;
  email address optional >
created: 1999-01-01 < ISO 8601 (yyyy-mm-dd) format >
status: >-
  < Draft | Under Review | Deferred | Proofing | Rejected | Withdrawn | Accepted
  | Superseded>
title: Macaroon
contributors: >-
  Leonardo Da Vinci (@leodavinci); Galileo Galilei (@ggal) < List of
  contributors -- Real Name + Github; email optional >
type: null
description: Description guidelines
discussions-to: (GitHub PR)
category: null
---

# Macaroon

## Overview

from [https://github.com/lightningnetwork/lnd/blob/master/docs/macaroons.md](https://github.com/lightningnetwork/lnd/blob/master/docs/macaroons.md)

You can think of a **macaroon** as a cookie, in a way. Cookies are small bits of data that your browser stores and sends to a particular website when it makes a request to that website. If you're logged into a website, that cookie can store a session ID, which the site can look up in its own database to check who you are and give you the appropriate content.

A macaroon is similar: it's a small bit of data that a client \(like `lncli`\) can send to a service \(like `lnd`\) to assert that it's allowed to perform an action. The service looks up the macaroon ID and verifies that the macaroon was initially signed with the service's root key. However, unlike a cookie, you can _delegate_ a macaroon, or create a version of it that has more limited capabilities, and then send it to someone else to use.

Just like a cookie, a macaroon should be sent over a secure channel \(such as a TLS-encrypted connection\), which is why we've also begun enforcing TLS for RPC requests in this release. Before SSL was enforced on websites such as Facebook and Google, listening to HTTP sessions on wireless networks was one way to hijack the session and log in as that user, gaining access to the user's account. Macaroons are similar in that intercepting a macaroon in transit allows the interceptor to use the macaroon to gain all the privileges of the legitimate user. 

## Details

### Section 1

### Section 2

### Section 3

## Resources

### Key People

* [Person 1](macaroon.md)
* [Person 2](macaroon.md)

### See also

## References
