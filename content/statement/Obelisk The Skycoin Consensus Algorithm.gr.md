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

Ο στόχος των προγραμματιστών του Skycoin ήταν να διορθώσουν τις σημαντικές 
αδυναμίες thw ασφαλείας και τις "συγκεντρωτικές τάσεις" που συνδέονται με τα δίκτυα 
blockchain στα οποίαη συναίνεση βασίζεται σε αλγόριθμους PoW ή PoS και η 
δημιουργία κερμάτων συνδέεται με έναεξόρυξης. Έτσι, το Skycoin προσπαθεί 
να δημιουργήσει την κρυπτοσυχνότητα την οποία ανταποκρίνεται καλύτερα στο 
αρχικό όραμα του Σάτοσι για ένα πλήρως αποκεντρωμένο ψηφιακό νομισματικό σύστημα.

Με αυτόν τον τρόπο, η τεχνολογία του Skycoin δημιουργεί μία αλυσίδα (blockchain network) 
χωρίς να απαιτούνται εξορυκτικές δραστηριότητες, 
με σταθερές προμήθειες στα κρυπτονομίσματα, 
χρόνοι συναλλαγής των 10 δευτερολέπτων και μεγαλύτερη ασφάλεια. 
Σε ένα σύστημα στο οποίο η σύνδεση μεταξύ της δημιουργίας νομισμάτων 
και του δικτυακού ελέγχου αποκόπτεται, τα κρυπτονομίσματα χάνουν την πολιτική τους 
υπόσταση και αρχίζουν να λειτουργούν περισσότερο σαν μια μορφή ψηφιακής 
ιδιοκτησίας στην πιο ευρύτερη της έννοια.

## Η απόδειξη εργασίας ("PoW") και το σύστημα του Bitcoin

Κατά τον πρώιμο προγραμματισμό του Bitcoin, ένας βασικός υπολογισμός ο οποίος ήταν 
λανθασμένος, ήταν η διαδικασία εξόρυξης (mining), όπου θα παρήγαγε μια οικονομική δομή 
με κίνητρα για την προαγωγή και προώθηση της αποκέντρωσης. 
Στην πραγματικότητα όμως, η σχέση μεταξύ της ομοφονίας-συναίνεσης και της ενέργειας 
για την κρυπτογραφική συνάρτηση κατατεμαχισμού (hashing power) ενθαρρύνει συνεχώς 
την αγορά της αυξανόμενης υπολογιστικής ισχύς ώστε να βρίσκεται σε έλεγχο το δίκτυο.

Για παράδειγμα, το δίκτυο του Bitcoin ελέγχεται απόλυτα από τρεις δεξαμενές εξόρυξης 
(pools) που κατόρθωσαν να συγκεντρώσουν ένα μεγάλο μέρος της ισχύος που απαιτείται 
για τις κρυπτογραφικές συναρτήσεις κατατεμαχισμού (hashing power) 
στους διακομιστές (σερβερ) της. Αυτές οι ομάδες άρχισαν να λειτουργούν ως καρτέλ,
χωρίζοντας με συμφωνία, την δύναμη των συναρτήσεων, μεταξύ τους. Η σχέση μεταξύ της 
εξόρυξης και του ελέγχου του δικτύου αναγνωρίστηκε ήδη από τον Σάτοσι ως την κύρια
μη κρυπτογραφική απειλή για τη σταθερότητα του δικτύου. Επιτρέπει σε αυτούς, που
συσσωρεύουν την επαρκή ισχύ επεξεργασίας και επιτυγχάνουν το μέγιστο ποσοστό της 
υπολογιστικής πλειοψηφίας να πλαστογραφήσουν ή να επαναφέρει τις συναλλαγές 
στο δίκτυο σε μια επίθεση της τάξεως του 51%. Κάποιοι υποστηρίζουν πως αυτή 
η ευπάθεια έχει γίνει λιγότερο πιεστική σε ένα περιβάλλον όπου η δύναμη κατακερματισμού
είναι εξαιρετικά συγκεντρωμένη με φορείς που έχουν επενδύσει μεγάλα ποσά στο Bitcoin
και εξαρτώνται για την επιβίωσή τους από την υψηλή αξία του νομίσματος. Ωστόσο, η
δύναμη ώστε να επηρεάστει το δίκτυο εξακολουθεί να είναι πολύ συγκεντρωμένη, 
νικώντας έτσι τον σκοπό της κατανεμημένης ιδέας των κρυπτονομισμάτων.

Ο αλγόριθμος PoW του δικτύου Bitcoin εισάγει μονοπωλιακά και προβλήματα ασφάλειας 
τοποθετώντας την εξουσία του δίκτυου με αυτόν τον οποίο έχει την ικανότητα να
κινητοποιήσει επαρκείς οικονομικούς πόρους ώστε να αποκτήσει τον έλεγχο 
της εξόρυξης (mining).

Αυτό σημαίνει επίσης ότι η λειτουργία του δικτύου είναι τόσο οικονομικά όσο και
περιβαλλοντικά αναποτελεσματική. Η συνεχής εισαγωγή της απαιτούμενης επεξεργαστικής ισχύος
για την διαδικασία εξόρυξης καταναλώνει μεγάλες ποσότητες ηλεκτρικής ενέργειας
που ισοδυναμούν σε μηνιαία κόστη δεκάδων εκατομμύριων. 
Αυτά τα έξοδα μπορούν να αντισταθμιστούν μόνο με μία εκθετικά αυξανόμενη εισροή 
νέων κεφαλαίων παράλληλα με την εισαγωγή νέων χρήστων. Μόνο ένας πολύ μικρός
αριθμός νομισμάτων, όπως το Bitcoin και το Ethereum είναι ικανός για την
προσελκύση αρκετών νέων χρήστών ώστε να επιτύχια μια τέτοια συνεχής ροή. 
Στην περίπτωση των περισσότερων άλλων νομίσματων PoW / PoS, το κόστος
της εξόρυξης PoW / PoS πληρώνεται σε χαμηλότερη αποτίμηση της αγοράς 
καθώς αφαιρείται το χρήμα από ένα κέρμα από το κόστος εξόρυξης
έως ότου εγκαταλείψει το νόμισμα.

Αυτή τη στιγμή η οικονομία του Bitcoin αποτελείται από τους νέους χρήστες που 
τοποθετούν κάπου τα χρήματά τους και στη συνέχεια τα χρήματα αυτά ρίχνονται σε ένα λάκκο 
και καίγονται σε μια τελετουργία θυσία προς το κόστος εξόρυξης ηλεκτρικής ενέργειας. 
Αν ο μέσος χρήστης έπρεπε να πληρώσει τους miners, το κόστος της ηλεκτρικής ενέργειας,
άμεσα ως αμοιβή συναλλαγών, αντί να ληστεύεται μέσω του πληθωρισμού 
με τη δημιουργία νέων κερμάτων, στη συνέχεια κάθε συναλλαγή Bitcoin θα κόστιζε 
περισσότερο από $50. Θα ήταν ακριβότερη από ένα διεθνή τραπεζική μεταφορά.

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
του κάθε κόμβου, επιτρέπει στο δίκτυο να αντιδρά στις επιθέσεις, αποσυνδέοντας 
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
μειωμένους χρόνους συναλλαγών και μεγαλύτερη ασφάλεια.

*Διαβάστε ακόμη:*

* *[Skycoin Consensus Algorithm Whitepapers](https://www.skycoin.net/whitepapers)*
* *[Obelisk The Skycoin Consensus Algorithm | Information Pages](/overview/obelisk-skycoin-consensus-algorithm-information-pages/)*
