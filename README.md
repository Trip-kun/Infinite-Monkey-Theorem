# Infinite-Monkey-Theorem
 https://en.wikipedia.org/wiki/Infinite_monkey_theorem
 The infinite monkey theorem states that a monkey hitting keys at random on a typewriter keyboard for an infinite amount of time will almost surely type any given text, such as the complete works of William Shakespeare. In fact, the monkey would almost surely type every possible finite text an infinite number of times. However, the probability that monkeys filling the entire observable universe would type a single complete work, such as Shakespeare's Hamlet, is so tiny that the chance of it occurring during a period of time hundreds of thousands of orders of magnitude longer than the age of the universe is extremely low (but technically not zero).

In this context, "almost surely" is a mathematical term with a precise meaning, and the "monkey" is not an actual monkey, but a metaphor for an abstract device that produces an endless random sequence of letters and symbols. One of the earliest instances of the use of the "monkey metaphor" is that of French mathematician Émile Borel in 1913,[1] but the first instance may have been even earlier.

Variants of the theorem include multiple and even infinitely many typists, and the target text varies between an entire library and a single sentence. Jorge Luis Borges traced the history of this idea from Aristotle's On Generation and Corruption and Cicero's De natura deorum (On the Nature of the Gods), through Blaise Pascal and Jonathan Swift, up to modern statements with their iconic simians and typewriters. In the early 20th century, Borel and Arthur Eddington used the theorem to illustrate the timescales implicit in the foundations of statistical mechanics.
Solution
Direct proof
There is a straightforward proof of this theorem. As an introduction, recall that if two events are statistically independent, then the probability of both happening equals the product of the probabilities of each one happening independently. For example, if the chance of rain in Moscow on a particular day in the future is 0.4 and the chance of an earthquake in San Francisco on any particular day is 0.00003, then the chance of both happening on the same day is 0.4 × 0.00003 = 0.000012, assuming that they are indeed independent.

Suppose the typewriter has 50 keys, and the word to be typed is banana. If the keys are pressed randomly and independently, it means that each key has an equal chance of being pressed. Then, the chance that the first letter typed is 'b' is 1/50, and the chance that the second letter typed is 'a' is also 1/50, and so on. Therefore, the chance of the first six letters spelling banana is

(1/50) × (1/50) × (1/50) × (1/50) × (1/50) × (1/50) = (1/50)6 = 1/15 625 000 000 ,
less than one in 15 billion, but not zero.

From the above, the chance of not typing banana in a given block of 6 letters is 1 − (1/50)6. Because each block is typed independently, the chance Xn of not typing banana in any of the first n blocks of 6 letters is

{\displaystyle X_{n}=\left(1-{\frac {1}{50^{6}}}\right)^{n}.}X_n=\left(1-\frac{1}{50^6}\right)^n.
As n grows, Xn gets smaller. For n = 1 million, Xn is roughly 0.9999, but for n = 10 billion Xn is roughly 0.53 and for n = 100 billion it is roughly 0.0017. As n approaches infinity, the probability Xn approaches zero; that is, by making n large enough, Xn can be made as small as is desired,[2][a] and the chance of typing banana approaches 100%.

The same argument shows why at least one of infinitely many monkeys will produce a text as quickly as it would be produced by a perfectly accurate human typist copying it from the original. In this case Xn = (1 − (1/50)6)n where Xn represents the probability that none of the first n monkeys types banana correctly on their first try. When we consider 100 billion monkeys, the probability falls to 0.17%, and as the number of monkeys n increases, the value of Xn – the probability of the monkeys failing to reproduce the given text – approaches zero arbitrarily closely. The limit, for n going to infinity, is zero. So the probability of the word banana appearing at some point in an infinite sequence of keystrokes is equal to one.

Infinite strings
This can be stated more generally and compactly in terms of strings, which are sequences of characters chosen from some finite alphabet:

Given an infinite string where each character is chosen uniformly at random, any given finite string almost surely occurs as a substring at some position.
Given an infinite sequence of infinite strings, where each character of each string is chosen uniformly at random, any given finite string almost surely occurs as a prefix of one of these strings.
Both follow easily from the second Borel–Cantelli lemma. For the second theorem, let Ek be the event that the kth string begins with the given text. Because this has some fixed nonzero probability p of occurring, the Ek are independent, and the below sum diverges,

{\displaystyle \sum _{k=1}^{\infty }P(E_{k})=\sum _{k=1}^{\infty }p=\infty ,}\sum_{k=1}^\infty P(E_k) = \sum_{k=1}^\infty p = \infty,
the probability that infinitely many of the Ek occur is 1. The first theorem is shown similarly; one can divide the random string into nonoverlapping blocks matching the size of the desired text, and make Ek the event where the kth block equals the desired string.[b]

Probabilities
However, for physically meaningful numbers of monkeys typing for physically meaningful lengths of time the results are reversed. If there were as many monkeys as there are atoms in the observable universe typing extremely fast for trillions of times the life of the universe, the probability of the monkeys replicating even a single page of Shakespeare is unfathomably small.

Ignoring punctuation, spacing, and capitalization, a monkey typing letters uniformly at random has a chance of one in 26 of correctly typing the first letter of Hamlet. It has a chance of one in 676 (26 × 26) of typing the first two letters. Because the probability shrinks exponentially, at 20 letters it already has only a chance of one in 2620 = 19,928,148,895,209,409,152,340,197,376[c] (almost 2 × 1028). In the case of the entire text of Hamlet, the probabilities are so vanishingly small as to be inconceivable. The text of Hamlet contains approximately 130,000 letters.[d] Thus there is a probability of one in 3.4 × 10183,946 to get the text right at the first trial. The average number of letters that needs to be typed until the text appears is also 3.4 × 10183,946,[e] or including punctuation, 4.4 × 10360,783.[f]

Even if every proton in the observable universe were a monkey with a typewriter, typing from the Big Bang until the end of the universe (when protons might no longer exist), they would still need a far greater amount of time – more than three hundred and sixty thousand orders of magnitude longer – to have even a 1 in 10500 chance of success. To put it another way, for a one in a trillion chance of success, there would need to be 10360,641 observable universes made of protonic monkeys.[g] As Kittel and Kroemer put it in their textbook on thermodynamics, the field whose statistical foundations motivated the first known expositions of typing monkeys,[4] "The probability of Hamlet is therefore zero in any operational sense of an event ...", and the statement that the monkeys must eventually succeed "gives a misleading conclusion about very, very large numbers."

In fact there is less than a one in a trillion chance of success that such a universe made of monkeys could type any particular document a mere 79 characters long.[h]

Almost surely
Main article: Almost surely
The probability that an infinite randomly generated string of text will contain a particular finite substring is 1. However, this does not mean the substring's absence is "impossible", despite the absence having a prior probability of 0. For example, the immortal monkey could randomly type G as its first letter, G as its second, and G as every single letter thereafter, producing an infinite string of Gs; at no point must the monkey be "compelled" to type anything else. (To assume otherwise implies the gambler's fallacy.) However long a randomly generated finite string is, there is a small but nonzero chance that it will turn out to consist of the same character repeated throughout; this chance approaches zero as the string's length approaches infinity. There is nothing special about such a monotonous sequence except that it is easy to describe; the same fact applies to any nameable specific sequence, such as "RGRGRG" repeated forever, or "a-b-aa-bb-aaa-bbb-...", or "Three, Six, Nine, Twelve…".

If the hypothetical monkey has a typewriter with 90 equally likely keys that include numerals and punctuation, then the first typed keys might be "3.14" (the first three digits of pi) with a probability of (1/90)4, which is 1/65,610,000. Equally probable is any other string of four characters allowed by the typewriter, such as "GGGG", "mATh", or "q%8e". The probability that 100 randomly typed keys will consist of the first 99 digits of pi (including the separator key), or any other particular sequence of that length, is much lower: (1/90)100. If the monkey's allotted length of text is infinite, the chance of typing only the digits of pi is 0, which is just as possible (mathematically probable) as typing nothing but Gs (also probability 0).

The same applies to the event of typing a particular version of Hamlet followed by endless copies of itself; or Hamlet immediately followed by all the digits of pi; these specific strings are equally infinite in length, they are not prohibited by the terms of the thought problem, and they each have a prior probability of 0. In fact, any particular infinite sequence the immortal monkey types will have had a prior probability of 0, even though the monkey must type something.

This is an extension of the principle that a finite string of random text has a lower and lower probability of being a particular string the longer it is (though all specific strings are equally unlikely). This probability approaches 0 as the string approaches infinity. Thus, the probability of the monkey typing an endlessly long string, such as all of the digits of pi in order, on a 90-key keyboard is (1/90)∞ which equals (1/∞) which is essentially 0. At the same time, the probability that the sequence contains a particular subsequence (such as the word MONKEY, or the 12th through 999th digits of pi, or a version of the King James Bible) increases as the total string increases. This probability approaches 1 as the total string approaches infinity, and thus the original theorem is correct.

Correspondence between strings and numbers
In a simplification of the thought experiment, the monkey could have a typewriter with just two keys: 1 and 0. The infinitely long string thusly produced would correspond to the binary digits of a particular real number between 0 and 1. A countably infinite set of possible strings end in infinite repetitions, which means the corresponding real number is rational. Examples include the strings corresponding to one-third (010101...), five-sixths (11010101...) and five-eighths (1010000...). Only a subset of such real number strings (albeit a countably infinite subset) contains the entirety of Hamlet (assuming that the text is subjected to a numerical encoding, such as ASCII).

Meanwhile, there is an uncountably infinite set of strings which do not end in such repetition; these correspond to the irrational numbers. These can be sorted into two uncountably infinite subsets: those which contain Hamlet and those which do not. However, the "largest" subset of all the real numbers are those which not only contain Hamlet, but which contain every other possible string of any length, and with equal distribution of such strings. These irrational numbers are called normal. Because almost all numbers are normal, almost all possible strings contain all possible finite substrings. Hence, the probability of the monkey typing a normal number is 1. The same principles apply regardless of the number of keys from which the monkey can choose; a 90-key keyboard can be seen as a generator of numbers written in base 90.

History
Statistical mechanics
In one of the forms in which probabilists now know this theorem, with its "dactylographic" [i.e., typewriting] monkeys (French: singes dactylographes; the French word singe covers both the monkeys and the apes), appeared in Émile Borel's 1913 article "Mécanique Statistique et Irréversibilité" (Statistical mechanics and irreversibility),[1] and in his book "Le Hasard" in 1914.[5] His "monkeys" are not actual monkeys; rather, they are a metaphor for an imaginary way to produce a large, random sequence of letters. Borel said that if a million monkeys typed ten hours a day, it was extremely unlikely that their output would exactly equal all the books of the richest libraries of the world; and yet, in comparison, it was even more unlikely that the laws of statistical mechanics would ever be violated, even briefly.

The physicist Arthur Eddington drew on Borel's image further in The Nature of the Physical World (1928), writing:

If I let my fingers wander idly over the keys of a typewriter it might happen that my screed made an intelligible sentence. If an army of monkeys were strumming on typewriters they might write all the books in the British Museum. The chance of their doing so is decidedly more favourable than the chance of the molecules returning to one half of the vessel.[6][7]

These images invite the reader to consider the incredible improbability of a large but finite number of monkeys working for a large but finite amount of time producing a significant work, and compare this with the even greater improbability of certain physical events. Any physical process that is even less likely than such monkeys' success is effectively impossible, and it may safely be said that such a process will never happen.[4] It is clear from the context that Eddington is not suggesting that the probability of this happening is worthy of serious consideration. On the contrary, it was a rhetorical illustration of the fact that below certain levels of probability, the term improbable is functionally equivalent to impossible.

Origins and "The Total Library"
In a 1939 essay entitled "The Total Library", Argentine writer Jorge Luis Borges traced the infinite-monkey concept back to Aristotle's Metaphysics. Explaining the views of Leucippus, who held that the world arose through the random combination of atoms, Aristotle notes that the atoms themselves are homogeneous and their possible arrangements only differ in shape, position and ordering. In On Generation and Corruption, the Greek philosopher compares this to the way that a tragedy and a comedy consist of the same "atoms", i.e., alphabetic characters.[8] Three centuries later, Cicero's De natura deorum (On the Nature of the Gods) argued against the atomist worldview:

He who believes this may as well believe that if a great quantity of the one-and-twenty letters, composed either of gold or any other matter, were thrown upon the ground, they would fall into such order as legibly to form the Annals of Ennius. I doubt whether fortune could make a single verse of them.[9]

Borges follows the history of this argument through Blaise Pascal and Jonathan Swift,[10] then observes that in his own time, the vocabulary had changed. By 1939, the idiom was "that a half-dozen monkeys provided with typewriters would, in a few eternities, produce all the books in the British Museum." (To which Borges adds, "Strictly speaking, one immortal monkey would suffice.") Borges then imagines the contents of the Total Library which this enterprise would produce if carried to its fullest extreme:

Everything would be in its blind volumes. Everything: the detailed history of the future, Aeschylus' The Egyptians, the exact number of times that the waters of the Ganges have reflected the flight of a falcon, the secret and true nature of Rome, the encyclopedia Novalis would have constructed, my dreams and half-dreams at dawn on August 14, 1934, the proof of Pierre Fermat's theorem, the unwritten chapters of Edwin Drood, those same chapters translated into the language spoken by the Garamantes, the paradoxes Berkeley invented concerning Time but didn't publish, Urizen's books of iron, the premature epiphanies of Stephen Dedalus, which would be meaningless before a cycle of a thousand years, the Gnostic Gospel of Basilides, the song the sirens sang, the complete catalog of the Library, the proof of the inaccuracy of that catalog. Everything: but for every sensible line or accurate fact there would be millions of meaningless cacophonies, verbal farragoes, and babblings. Everything: but all the generations of mankind could pass before the dizzying shelves – shelves that obliterate the day and on which chaos lies – ever reward them with a tolerable page.[11]

Borges' total library concept was the main theme of his widely read 1941 short story "The Library of Babel", which describes an unimaginably vast library consisting of interlocking hexagonal chambers, together containing every possible volume that could be composed from the letters of the alphabet and some punctuation characters.

Actual monkeys
In 2002[12], lecturers and students from the University of Plymouth MediaLab Arts course used a £2,000 grant from the Arts Council to study the literary output of real monkeys. They left a computer keyboard in the enclosure of six Celebes crested macaques in Paignton Zoo in Devon, England for a month, with a radio link to broadcast the results on a website.[13]

Not only did the monkeys produce nothing but five total pages largely consisting of the letter 'S',[12] the lead male began striking the keyboard with a stone, and other monkeys followed by soiling it. Mike Phillips, director of the university's Institute of Digital Arts and Technology (i-DAT), said that the artist-funded project was primarily performance art, and they had learned "an awful lot" from it. He concluded that monkeys "are not random generators. They're more complex than that. ... They were quite interested in the screen, and they saw that when they typed a letter, something happened. There was a level of intention there."[13][14]

The full text created by the monkeys is available to read "here" (PDF).[12]
Applications and criticisms
Evolution
In his 1931 book The Mysterious Universe, Eddington's rival James Jeans attributed the monkey parable to a "Huxley", presumably meaning Thomas Henry Huxley. This attribution is incorrect.[15] Today, it is sometimes further reported that Huxley applied the example in a now-legendary debate over Charles Darwin's On the Origin of Species with the Anglican Bishop of Oxford, Samuel Wilberforce, held at a meeting of the British Association for the Advancement of Science at Oxford on 30 June 1860. This story suffers not only from a lack of evidence, but the fact that in 1860 the typewriter itself had yet to emerge.[16]

Despite the original mix-up, monkey-and-typewriter arguments are now common in arguments over evolution. As an example of Christian apologetics Doug Powell argued that even if a monkey accidentally types the letters of Hamlet, it has failed to produce Hamlet because it lacked the intention to communicate. His parallel implication is that natural laws could not produce the information content in DNA.[17] A more common argument is represented by Reverend John F. MacArthur, who claimed that the genetic mutations necessary to produce a tapeworm from an amoeba are as unlikely as a monkey typing Hamlet's soliloquy, and hence the odds against the evolution of all life are impossible to overcome.[18]

Evolutionary biologist Richard Dawkins employs the typing monkey concept in his book The Blind Watchmaker to demonstrate the ability of natural selection to produce biological complexity out of random mutations. In a simulation experiment Dawkins has his weasel program produce the Hamlet phrase METHINKS IT IS LIKE A WEASEL, starting from a randomly typed parent, by "breeding" subsequent generations and always choosing the closest match from progeny that are copies of the parent, with random mutations. The chance of the target phrase appearing in a single step is extremely small, yet Dawkins showed that it could be produced rapidly (in about 40 generations) using cumulative selection of phrases. The random choices furnish raw material, while cumulative selection imparts information. As Dawkins acknowledges, however, the weasel program is an imperfect analogy for evolution, as "offspring" phrases were selected "according to the criterion of resemblance to a distant ideal target." In contrast, Dawkins affirms, evolution has no long-term plans and does not progress toward some distant goal (such as humans). The weasel program is instead meant to illustrate the difference between non-random cumulative selection, and random single-step selection.[19] In terms of the typing monkey analogy, this means that Romeo and Juliet could be produced relatively quickly if placed under the constraints of a nonrandom, Darwinian-type selection because the fitness function will tend to preserve in place any letters that happen to match the target text, improving each successive generation of typing monkeys.

A different avenue for exploring the analogy between evolution and an unconstrained monkey lies in the problem that the monkey types only one letter at a time, independently of the other letters. Hugh Petrie argues that a more sophisticated setup is required, in his case not for biological evolution but the evolution of ideas:

In order to get the proper analogy, we would have to equip the monkey with a more complex typewriter. It would have to include whole Elizabethan sentences and thoughts. It would have to include Elizabethan beliefs about human action patterns and the causes, Elizabethan morality and science, and linguistic patterns for expressing these. It would probably even have to include an account of the sorts of experiences which shaped Shakespeare's belief structure as a particular example of an Elizabethan. Then, perhaps, we might allow the monkey to play with such a typewriter and produce variants, but the impossibility of obtaining a Shakespearean play is no longer obvious. What is varied really does encapsulate a great deal of already-achieved knowledge.[20]

James W. Valentine, while admitting that the classic monkey's task is impossible, finds that there is a worthwhile analogy between written English and the metazoan genome in this other sense: both have "combinatorial, hierarchical structures" that greatly constrain the immense number of combinations at the alphabet level.[21]

Literary theory
R. G. Collingwood argued in 1938 that art cannot be produced by accident, and wrote as a sarcastic aside to his critics,

... some ... have denied this proposition, pointing out that if a monkey played with a typewriter ... he would produce ... the complete text of Shakespeare. Any reader who has nothing to do can amuse himself by calculating how long it would take for the probability to be worth betting on. But the interest of the suggestion lies in the revelation of the mental state of a person who can identify the 'works' of Shakespeare with the series of letters printed on the pages of a book ...[22]

Nelson Goodman took the contrary position, illustrating his point along with Catherine Elgin by the example of Borges' "Pierre Menard, Author of the Quixote",

What Menard wrote is simply another inscription of the text. Any of us can do the same, as can printing presses and photocopiers. Indeed, we are told, if infinitely many monkeys ... one would eventually produce a replica of the text. That replica, we maintain, would be as much an instance of the work, Don Quixote, as Cervantes' manuscript, Menard's manuscript, and each copy of the book that ever has been or will be printed.[23]

In another writing, Goodman elaborates, "That the monkey may be supposed to have produced his copy randomly makes no difference. It is the same text, and it is open to all the same interpretations. ..." Gérard Genette dismisses Goodman's argument as begging the question.[24]

For Jorge J. E. Gracia, the question of the identity of texts leads to a different question, that of author. If a monkey is capable of typing Hamlet, despite having no intention of meaning and therefore disqualifying itself as an author, then it appears that texts do not require authors. Possible solutions include saying that whoever finds the text and identifies it as Hamlet is the author; or that Shakespeare is the author, the monkey his agent, and the finder merely a user of the text. These solutions have their own difficulties, in that the text appears to have a meaning separate from the other agents: What if the monkey operates before Shakespeare is born, or if Shakespeare is never born, or if no one ever finds the monkey's typescript?[25]

Random document generation
The theorem concerns a thought experiment which cannot be fully carried out in practice, since it is predicted to require prohibitive amounts of time and resources. Nonetheless, it has inspired efforts in finite random text generation.

One computer program run by Dan Oliver of Scottsdale, Arizona, according to an article in The New Yorker, came up with a result on 4 August 2004: After the group had worked for 42,162,500,000 billion billion monkey-years, one of the "monkeys" typed, "VALENTINE. Cease toIdor:eFLP0FRjWK78aXzVOwm)-‘;8.t" The first 19 letters of this sequence can be found in "The Two Gentlemen of Verona". Other teams have reproduced 18 characters from "Timon of Athens", 17 from "Troilus and Cressida", and 16 from "Richard II".[26]

A website entitled The Monkey Shakespeare Simulator, launched on 1 July 2003, contained a Java applet that simulated a large population of monkeys typing randomly, with the stated intention of seeing how long it takes the virtual monkeys to produce a complete Shakespearean play from beginning to end. For example, it produced this partial line from Henry IV, Part 2, reporting that it took "2,737,850 million billion billion billion monkey-years" to reach 24 matching characters:

RUMOUR. Open your ears; 9r"5j5&?OWTY Z0d
Due to processing power limitations, the program used a probabilistic model (by using a random number generator or RNG) instead of actually generating random text and comparing it to Shakespeare. When the simulator "detected a match" (that is, the RNG generated a certain value or a value within a certain range), the simulator simulated the match by generating matched text.[27]

More sophisticated methods are used in practice for natural language generation. If instead of simply generating random characters one restricts the generator to a meaningful vocabulary and conservatively following grammar rules, like using a context-free grammar, then a random document generated this way can even fool some humans (at least on a cursory reading) as shown in the experiments with SCIgen, snarXiv, and the Postmodernism Generator.

In February 2019, the OpenAI group published the Generative Pre-trained Transformer 2 (GPT-2) artificial intelligence to GitHub, which is able to produce a fully plausible news article given a two sentence input from a human hand. The AI was so effective that instead of publishing the full code, the group chose to publish a scaled-back version and released a statement regarding "concerns about large language models being used to generate deceptive, biased, or abusive language at scale."[28]

Testing of random-number generators
Main article: Diehard tests
Questions about the statistics describing how often an ideal monkey is expected to type certain strings translate into practical tests for random-number generators; these range from the simple to the "quite sophisticated". Computer-science professors George Marsaglia and Arif Zaman report that they used to call one such category of tests "overlapping m-tuple tests" in lectures, since they concern overlapping m-tuples of successive elements in a random sequence. But they found that calling them "monkey tests" helped to motivate the idea with students. They published a report on the class of tests and their results for various RNGs in 1993.[29]

In popular culture
Main article: Infinite monkey theorem in popular culture
The infinite monkey theorem and its associated imagery is considered a popular and proverbial illustration of the mathematics of probability, widely known to the general public because of its transmission through popular culture rather than through formal education.[i] This is helped by the innate humor stemming from the image of literal monkeys rattling away on a set of typewriters, and is a popular visual gag.

A quotation attributed[30] to a 1996 speech by Robert Wilensky stated, "We've heard that a million monkeys at a million keyboards could produce the complete works of Shakespeare; now, thanks to the Internet, we know that is not true."

The enduring, widespread popularity of the theorem was noted in the introduction to a 2001 paper, "Monkeys, Typewriters and Networks: The Internet in the Light of the Theory of Accidental Excellence".[31] In 2002, an article in The Washington Post said, "Plenty of people have had fun with the famous notion that an infinite number of monkeys with an infinite number of typewriters and an infinite amount of time could eventually write the works of Shakespeare".[32] In 2003, the previously mentioned Arts Council funded experiment involving real monkeys and a computer keyboard received widespread press coverage.[12] In 2007, the theorem was listed by Wired magazine in a list of eight classic thought experiments.[33]

See also
Normal number
Hilbert's paradox of the Grand Hotel, another thought experiment involving infinity
Law of truly large numbers
Murphy's Law
Texas sharpshooter fallacy
The Hidden Reality: Parallel Universes and the Deep Laws of the Cosmos, explains the multiverse in which every possible event will occur infinitely many times
The Library of Babel
The Engine
Boltzmann brain
The Infinite Monkey Cage




---From Wikipedia
