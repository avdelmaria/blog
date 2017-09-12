+++
title = "Obelisk: The Skycoin Consensus Algorithm"
tags = [
    "Statement",
]
date = "2017-09-08"
categories = [
    "Statement",
]
+++

![Obelisk Ο Αλγόριθμος Συναίνεσης του Skycoin](/img/obelisk-the-skycoin-consensus-algorithm.png)

Το blockchain του Skycoin κάνει χρήση ενός νέου τύπου αλγόριθμου συναίνεσης
που ονομάζεται "Οβελίσκος" και αντικαθιστά τόσο την απόδειξη εργασίας ("PoW") 
όσο και την απόδειξη της συμμετοχής ("PoS").

Ο στόχος των προγραμματιστών του Skycoin ήταν να διορθώσουν τις σημαντικές αδυναμίες ασφαλείας
και τις "συγκεντρωτικές τάσεις" που συνδέονται με τα δίκτυα blockchain στα οποία
η συναίνεση βασίζεται σε αλγόριθμους PoW ή PoS και η δημιουργία κερμάτων συνδέεται με ένα
εξόρυξης. Έτσι, το Skycoin προσπαθεί να δημιουργήσει την κρυπτοσυχνότητα την οποία
ανταποκρίνεται καλύτερα στο αρχικό όραμα του Σάτοσι για ένα πλήρως αποκεντρωμένο ψηφιακό
νομισματικό σύστημα.

Με αυτόν τον τρόπο, η τεχνολογία του Skycoin δημιουργεί μία αλυσίδα (blockchain network) 
χωρίς να απαιτούνται εξορυκτικές δραστηριότητες, 
με σταθερές προμήθειες στα κρυπτονομίσματα, 
χρόνοι συναλλαγής 10 δευτερολέπτων και μεγαλύτερη ασφάλεια. 
Σε ένα σύστημα στο οποίο η σύνδεση μεταξύ της δημιουργίας νομισμάτων 
και του δικτυακού ελέγχου αποκόπτεται, τα κρυπτονομίσματα χάνουν την πολιτική τους 
υπόσταση και αρχίζουν να λειτουργούν περισσότερο σαν μια μορφή ψηφιακής 
ιδιοκτησίας στην πιο απλή του έννοια.

## Η απόδειξη εργασίας ("PoW") και το σύστημα του Bitcoin

Κατά τον πρώιμο προγραμματισμό του Bitcoin, ένας βασικός λανθασμένος υπολογισμός 
ήταν η διαδικασία εξόρυξης όπου θα παρήγαγε μια οικονομική δομή με κίνητρα που 
θα μπορούσε να γίνει προαγωγή και προώθηση της αποκέντρωσης. 
Στην πραγματικότητα όμως, η σχέση μεταξύ συναίνεσης και της ενέργειας του κατακερματισμού 
(hashing power) ενθαρρύνει συνεχώς την αγορά της συνεχώς αυξανόμενης υπολογιστικής ισχύς 
ώστε να βρίσκεται σε έλεγχο του δίκτυο.

The Bitcoin network, for instance, is de facto controlled by three for-profit
mining pools which have been able to concentrate a large part of the network’s
hashing power on its servers. These pools have begun to act as a cartel,
splitting hashing power among each other by agreement. The link between mining
and control of the network was already identified by Satoshi as the main
non-cryptographic threat to the stability of the network. It allows actors who
accumulate sufficient processing power and achieve a majority hash rate to
falsify or revert transactions on the network in a 51% attack. Some argue that
this vulnerability has become less pressing in an environment where hash power
is highly centralized with actors who have invested large sums in the Bitcoin
network and depend for their survival on the high value of the coin. Yet the
power to influence the network is still highly concentrated, defeating the
purpose of a distributed ledger-based cryptocurrency.

The Bitcoin network’s PoW algorithm thus introduces security and monopoly
problems by placing power over the network with the actor capable of
mobilizing enough economic resources to control the mining process.

This also implies that the operation of the network is both economically and
environmentally inefficient. The continuous input of processing power required
by the mining process uses up large amounts of electricity, incurring monthly
costs in the tens of millions. These costs can only be offset with an
exponentially growing influx of new capital along with new users. Only a very
small number of well-established coins, like Bitcoin and Ethereum, will be
able to attract enough users to achieve such a continual flow. In the case of
most other PoW/PoS-based coins, the cost
of PoW/PoS mining is paid for in a lower market valuation as money is bled
out of a coin by mining costs until the coin is abandoned.

>Right now the Bitcoin economy consists of new users putting their money in
and then the money being thrown in a pit and burned in a sacrifice ritual to
the mining electricity costs. If the average user had to pay the miners’
electricity cost directly as transaction fees, instead of it being robbed from
them through inflation by the creation of new coins, then each Bitcoin
transaction would cost more than $50. It would be more expensive than an
international bank transfer.

## The centralizing tendency of Proof of Stake

Although Proof of Stake algorithms tackle the security issue of 51% attacks,
they are arguably even more vulnerable to centralization than PoW networks. In
PoS, the size of network participants’ holdings of the cryptocurrency in the
network determines their authority and voting power to implement technical
changes in the network. Participants are able to mine an equivalent portion of
their stake regardless of processing power.

This principle significantly increases the economic barriers to launching a
51% attack because the financial cost of acquiring the majority of tokens on
the network in the open market is very likely to exceed the potential gain. If
an attacker ends up as the majority stakeholder in the network, he will suffer
most from the impact of the attack on the stability of the network or the
external value of the cryptocurrency.

Yet, although raising the barriers to human-led attacks on the network, PoS
creates a centralizing impulse which is as strong as, if not stronger than, in
the case of PoW. As Joseph Young summarizes in his comparison of the two
systems at [coinfox.info](http://www.coinfox.info/), “A system where the major
stakeholder enjoys extensive control and authority over both technical and
economic aspects of the network creates a major monopoly problem.” While in PoW
voting on the implementation of technical changes to the network “is divided
among miners, developers and other crucial members of the community,” in a PoS
system “major stakeholders have a technical ability to make any changes they
like without considering the will of the community, businesses, miners and
developers. This centralisation of voting power and, essentially, control of
the network defeats the purpose of a distributed ledger-based cryptocurrency
since it contradicts its entire principle of distributing all elements within
the network to avoid the presence of a central authority.”

## Obelisk: Skycoin's distributed consensus algorithm

To tackle this centralization problem, Skycoin moves beyond PoW/PoS.
It uses a distributed consensus algorithm, called Obelisk, which
distributes influence over the network according to a “web of trust”. In
essence, every node has a list of other nodes that it subscribes to, and the
density of a node’s network of subscribers determines its influence on the
network. Each node is assigned a personal blockchain which acts as a “public
broadcasting channel” on which all of a node’s actions are visible and
publicly recorded. As all consensus decisions and communication occur through
the personal blockchains of each node, the community can very easily audit
nodes for cheating or collusion. How decisions on the network are made and
which nodes influence those decisions is completely transparent.

Το δημόσιο αρχείο που παραμένει από το προσωπικό μπλοκ αλυσίδας (blockchain) 
του κάθε κόμβου, επιτρέπει στο δίκτυο να αντιδρά σε επιθέσεις αποσυνδέοντας 
τις συνδέσεις που είναι λιγότερο αξιόπιστες ή έχουν θεωρηθεί κακόβουλες, 
αναθέτοντας έτσι το δίκτυο σε έναν μικρότερο και πυκνότερο πυρήνα από
αξιόπιστους κόμβους. Ως εκ τούτου, εάν η κοινότητα δεν διαθέτει εμπιστοσύνη 
στους κόμβους που τις αντιπροσωπεύει ή αισθάνεται ότι η ισχύς στο δίκτυο 
είναι πολύ συγκεντρωμένη (ή όχι αρκετά συγκεντρωμένη), η κοινότητα 
είναι σε θέση να μετατοπίσει συλλογικά την ισορροπία της εξουσίας στο δίκτυο 
αλλάζοντας συλλογικά την εμπιστοσύνη τους στα μέλη του δικτύου. 
Η λογοδοσία των κόμβων στην κοινότητα, οι έλεγχοι από τρίτες μεριές 
καθώς και η διαφάνεια της συναίνεσης ενισχύονται για την συλλογική λήψη αποφάσεων 
και εισάγουν έτσι ένα ιδιαίτερα δημοκρατικό και αποκεντρωτικό στοιχείο μέσα στο δίκτυο.

Το σύστημα αυτό προβλέπει ένα σύστημα ψηφιακού νομίσματος με σημαντικά 
μειωμένους χρόνους συναλλαγής και μεγαλύτερη ασφάλεια.

*Διαβάστε ακόμη:*

* *[Skycoin Consensus Algorithm Whitepapers](https://www.skycoin.net/whitepapers)*
* *[Obelisk The Skycoin Consensus Algorithm | Information Pages](/overview/obelisk-skycoin-consensus-algorithm-information-pages/)*
