### Bitcoin

Auszüge vom [The Satoshi Nakamoto Institute](https://nakamotoinstitute.org/).

> From: Satoshi Nakamoto
> Subject: Bitcoin P2P e-cash paper
> Date: October 31, 2008 at 18:10:00 UTC

I've been working on a new electronic cash system that's fully
peer-to-peer, with no trusted third party.

The paper is available at:
http://www.bitcoin.org/bitcoin.pdf

The main properties:
Double-spending is prevented with a peer-to-peer network.
No mint or other trusted parties.
Participants can be anonymous.
New coins are made from Hashcash style proof-of-work.
The proof-of-work for new coin generation also powers the
network to prevent double-spending.

Bitcoin: A Peer-to-Peer Electronic Cash System

Abstract. A purely peer-to-peer version of electronic cash would
allow online payments to be sent directly from one party to another
without the burdens of going through a financial institution.
Digital signatures provide part of the solution, but the main
benefits are lost if a trusted party is still required to prevent
double-spending. We propose a solution to the double-spending
problem using a peer-to-peer network. The network timestamps
transactions by hashing them into an ongoing chain of hash-based
proof-of-work, forming a record that cannot be changed without
redoing the proof-of-work. The longest chain not only serves as
proof of the sequence of events witnessed, but proof that it came
from the largest pool of CPU power. As long as honest nodes control
the most CPU power on the network, they can generate the longest
chain and outpace any attackers. The network itself requires
minimal structure. Messages are broadcasted on a best effort basis,
and nodes can leave and rejoin the network at will, accepting the
longest proof-of-work chain as proof of what happened while they
were gone.

Full paper at:
http://www.bitcoin.org/bitcoin.pdf

Satoshi Nakamoto

> From: Hal Finney
> Subject: Bitcoin P2P e-cash paper
> Date: November 7, 2008 at 23:40:12 UTC

Bitcoin seems to be a very promising idea. I like the idea of basing
security on the assumption that the CPU power of honest participants
outweighs that of the attacker. It is a very modern notion that exploits
the power of the long tail. When Wikipedia started I never thought it
would work, but it has proven to be a great success for some of the
same reasons.

I also do think that there is potential value in a form of unforgeable
token whose production rate is predictable and can't be influenced
by corrupt parties. This would be more analogous to gold than to fiat
currencies. Nick Szabo wrote many years ago about what he called "bit
gold"[1] and this could be an implementation of that concept. There have
also been proposals for building light-weight anonymous payment schemes on
top of heavy-weight non-anonymous systems, so Bitcoin could be leveraged
to allow for anonymity even beyond the mechanisms discussed in the paper.

[...]

Sorry about all the questions, but as I said this does seem to be a
very promising and original idea, and I am looking forward to seeing
how the concept is further developed. It would be helpful to see a more
process oriented description of the idea, with concrete details of the
data structures for the various objects (coins, blocks, transactions),
the data which is included in messages, and algorithmic descriptions
of the procedures for handling the various events which would occur in
this system. You mentioned that you are working on an implementation,
but I think a more formal, text description of the system would be a
helpful next step.

Hal Finney

[1] http://unenumerated.blogspot.com/2005/12/bit-gold.html
