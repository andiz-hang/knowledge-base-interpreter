My knowledge base is a simple animal search database. By entering traits (atoms), the 
knowledge base can infer a specific animal/type of animal. For example, 

kb> tell mammal can_swim  no_legs  smart

will result in the knowledge base inferring the atom "dolphin".
Some traits can be inferred by other traits. For example:

kb> tell warm_blooded vertebrate

results in the trait "mammal" being added to the database.
I also have included specific species in the kb:

kb> tell whale massive

results in "blue_whale"

I am not a biologist, and my kb is by no means an exhaustive list of all animals. This is just
a sample list of possible animals. I found it hard to distinguish some animals using this system
(for example, I couldn't think of a trait that would separate "caribou" and "moose"), which is why
many animals are not present in the kb. Also, some traits can be debatable (I gave "bear" the trait
"big"). Furthermore, since I couldn't have negative atoms, the kb will search for all animals
that satisfy the traits that you input. You will get both "ant" and "bee" if you enter

kb> tell insect has_queen digs can_fly

