Bitwrk - A Bitcoin-friendly, anonymous marketplace for computing power
======================================================================

This is going to be a proof-of-concept implementation of a marketplace
for computing services, an idea I had in 2011 when I saw the enormous
amounts of computing capacity dedicated to mining Bitcoin.

Since then, the work needed to mine a single bitcoin has increased by
at least a factor of 50! (See http://blockchain.info/charts/hash-rate)

If generating this enormous amount of work for nothing more than a
simple cryptographic lottery can be lucrative, there must be demand
for tasks more useful. Let's find out!

Status
------
This project has been under heavy development for the last couple of
weeks and currently consists of:
- A rudimentary server written in Go (http://golang.org/), running on
  Google App Engine. It exports an API for entering bids and updating
  transactions. The lifecycle of every transaction can be traced,
  and all communication is secured with Elliptic-Curve cryptographic
  signatures of the same kind than those that can be generated using
  the originaö Bitcoin client.
- An even more rudimentary client, also written in Go, that currently
  doesn't do anything more useful than create a random bid under a
  random address. I used it to test the workload the server can handle.
  Some day, the client will act as an intermediary, taking tasks from
  local programs and dispatching them to the internet.

There is no pretty UI and no actual money can be made or lost.


Have fun!
2013-08-01, Jonas Eschenburg

