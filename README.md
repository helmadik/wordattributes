Normal case of encoding: ``<w id="1811590" lemma="τράπεζα" pos="n--s---fa-">τράπεζαν</w>``

Nasty edge case: hyphenated words in poetry that need to stay on separate lines: 

Choral odes (and some other forms of poetry) have words that are hyphenated and must remain hyphenated on the 'page' for reasons of meter. 
Say the word in the text is ἀξιόθρη HYPHEN NEWLINE νος

Their parsing (should) look as follows in our data: ``<w id="1817771" lemma="segment" pos="----------">ἀξιόθρη</w>-</l> <l n="905"><w id="1817772" lemma="ἀξιόθρηνος" pos="a--s---mn-">νος</w>.``  In an ideal world, this would count as ONE word for word counts etc.  In Philo4, we show the full parse in the final segment of a broken-up word. The previous segment(s) will have ``lemma="segment" pos="----------".`` 
I'm saying "segment(s)" because Aristophanes does some outrageous stuff with words stretching over multiple lines.
