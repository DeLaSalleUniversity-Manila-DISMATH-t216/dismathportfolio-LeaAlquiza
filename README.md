# WEEK 1
- On our first meeting, our professor discussed a brief introduction on what Discrete Mathematics was about and how our learning in Algebra can help in analyzing Discrete Mathematics problems.
- Following the brief introduction, we had a recap on what Propositions are. And I learned that Propositions are declarative statements that can be answered by either true or false.
- We were also asked one question each about propositions. I was asked if **2+3=5** was a proposition, and my answer was **yes** because it's true that 2 plus 3 is equal to 5.

- On our next meeting, we had officially started our class. We had a review type of discussion since we had already taken the course LOGICIR.
- The review type discussion started with some exercises and if we encounter unfamiliar terms our professor discusses them first and then proceeds with the exercises again.
- Recalling all logical operations:

  |             Operator               |    Symbol   |          Expression         | 
|:------------------------------------:|:-----------:|:---------------------------:| 
|            Negation (NOT)            |    ¬        |          ¬p                |
|          Conjunction (AND)           |   ∧        |       p ∧ q             |
|           Disjunction (OR)           |    ∨       |         p ∨ q            | 
|      Exclusive Disjunction (XOR)     |    ⊕   |  p ⊕ q ≡ (¬p ∧ q)  ∨  (p ∧ ¬q) |
|      Conditional (IF-THEN, etc.)     |   →     |        p → q ≡ ¬p ∨ q        |
| Biconditional (IF AND ONLY IF, etc.) |    ↔   |    p ↔ q ≡ (p → q) ∧ (q → p) |  
- Additionally, we also learned about Inverse, Converse, and Contrapositive. Expressing these three in logical expression form, assuming p → q:

  Conditinal Operator |  Expression 
:-------------------:|:------------:
Inverse | ¬p → ¬q 
Converse | q → p 
Contrapositive | ¬q → ¬p

- I was also able to answer some quesions during class including:

  Number-Letter of Question |  Question | Answer
:------------------------:|---------|:-----:
8-b | p: I bought a lottery ticket this week.<br/> q: I won the million dollar jackpot.<br/> Express p v q as an English sentence. | I bought a lottery ticket this week or I won the million dollar jackpot.
11-a | p: It is below freezing.<br/> q: It is snowing.<br/> Write "It is below freezing and snowing" using p and q and logical connectives (including negations). | p ∧ q 
13-g | p: You drive over 65 miles per hour.<br/> q: You get a speeding ticket.<br/> Write "Whenever you get a speeding ticket, you are driving over 65 miles per hour." using p and q and logical connectives (including negations). | q → p 
15-e | p: Grizzly bears have been seen in the area.<br/> q: Hiking is safe on the trail.<br/> r: Berries are ripe along the trail.<br/> Write "For hiking on the trail to be safe, it is necessary but not sufficient that berries not be ripe along the trail and for grizzly bears not to have been seen in the area." using p, q, and r and logical connectives (including negations). | (q → (¬r ∧ ¬p)) ∧ ¬((¬r ∧ ¬p) → p) 
17-a | Determine whether "If 1+1=2, then 2+2=5." is true or false. | False 
19-b | Determine whether "A password must have at least three digits or be at least eight characters long." an inclusive or, exclusive or, is intended. | Inclusive OR (because you can have a long password with digits in it) 
25-a | Write "If it is hot outside you buy an ice cream cone, and if you buy an ice cream cone it is hot outside." in the form of "p if and only if q" in English | You buy an ice cream cone if and only if it is hot outside. 
27-c | State the converse, contrapositive, and inverse of "A positive integer is a prime only if it has no divisors other than 1 and itslef." | **Converse**: A positive integer is a prime if it has no divisors other than 1 and itself.<br/> **Contrapositive**: If a positive integer does not have no divisors other than 1 and itself, then it is not prime.<br/> **Inverse**: If a positive integer is not prime, then it has a divisor other than 1 and itself. 
29-d | How many rows appear in a truth table for "(p ∧ r ∧ t) ↔ (q ∧ t)" | 2^4 = 16 
<br/>
#### Assignment:
- 31.b. Construct a truth table for p ∨ ¬p
  
    p | ¬p | p ∨ ¬p
    :---:|:---:|:---:
    T | F | T
    F | T | T

- 33.c. Construct a truth table for (p ∨ q) ⊕ (p ∧ q)

    p | q | p ∨ q | p ∧ q | (p ∨ q) ⊕ (p ∧ q)
    :---:|:---:|:---:|:---:|:---:
    T | F | T | F | T
    F | T | T | F | T
    T | T | T | T | F
    F | F | F | F | F

- 35.d. Construct a truth table for  (p → q) ∧ (¬p → q)

    p | ¬p | q | p → q | ¬p → q | (p → q) ∧ (¬p → q)
    :---:|:---:|:---:|:---:|:---:|:---:
    T | F | F | F | T | F
    F | T | T | T | T | T
    T | F | T | T | T | T
    F | T | F | T | F | F

- 37.e. Construct a truth table for (p ↔ q) ∨ (¬q ↔ r)

    p | q | ¬q | r | p ↔ q | ¬q ↔ r | (p ↔ q) ∨ (¬q ↔ r)
    :---:|:---:|:---:|:---:|:---:|:---:|:---:
    T | F | T | T | F | F | T
    T | T | F | F | T | T | T
    T | F | T | F | F | F | F
    T | T | F | T | T | F | T
    F | T | F | F | F | T | T
    F | F | T | T | T | T | T
    F | T | F | T | F | F | F
    F | F | T | F | T | F | T
    
<br/>
# WEEK 2
- During our second week, we had a brief discussion on Propositional Equivalences.
- We differentiated Tautology, Contradiction, and Contingency.
  * **Tautology** - a compound proposition that's **_always true_** regardless of what the truth values of the propositions are.
  * **Contradiction** - a compound proposition that's **_always false_** regardless of what the truth values of the propositions are.
  * **Contingency** - it's **_neither a tautology nor a contradiction_**.
- Regarding contradiction, the logical operation **AND** is a natural partner for contradiction.
- Following the brief introduction, we proceeded to our main topic which was Logical Equivalences. Compound propositions that have the same truth value in all possible cases are **logically equivalent**.
- When proving logical statements using truth table seem too much of a hassle to do, an alternative to it is to use logical equivalences.
- Below is a table of Logical Equivalences:

  | Equivalence | Name |
  | :---------: | :--: |
  | p ∧ **T** ≡ p<br/> p ∨ **F** ≡ p | Identity Laws |
  | p ∨ **T** ≡ **T**<br/> p ∧ **F** ≡ **F** | Domination Laws |
  | p ∨ p ≡ p<br/> p ∧ p ≡ p | Idempotent Laws |
  | ¬(¬p) ≡ p | Double Negation Law |
  | p ∨ q ≡ q ∨ p<br/> p ∧ q ≡ q ∧ p | Commutative Laws |
  | (p ∨ q) ∨ r ≡ p ∨ (q ∨ r)<br/> (p ∧ q) ∧ r ≡ p ∧ (q ∧ r)| Associative Laws |
  | p ∨ (q ∧ r) ≡ (p ∨ q) ∧ (p ∨ r)<br/> p ∧ (q ∨ r) ≡ (p ∧ q) ∨ (p ∧ r)| Distributive Laws |
  | ¬(p ∧ q) ≡ ¬p ∨ ¬q<br/> ¬(p ∨ q) ≡ ¬p ∧ ¬q | De Morgan's Law |
  | p ∨ (p ∧ q) ≡ p<br/> p ∧ (p ∨ q) ≡ p | Absorption Laws |
  | p ∨ ¬p ≡ **T**<br/> p ∧ ¬p ≡ **F** | Negation Laws |
  | p → q ≡ ¬p ∨ q | Implication Equivalence |
  
- Me and my other classmate were able to answer what is the logical equivalent of p → q using AND, OR, or NOT and we answered ¬p ∨ q because it has the same truth table as the given.
- Afterwhich, we moved on to the next discussion which was about Quantifiers. There are two types of Quantifiers:

  | Quantifier | Symbol | Statement | Definition | Negation |
  | :---: | :--: | :---: | :---: | :---: |
  | Universal | ∀ | ∀xP(x) | P(x) for all values of x in the domain | ¬(∀xP(x)) ≡ ∃x¬P(x) |
  | Existential | ∃ | ∃xP(x) | There exist an element x in the domain such that P(x) | ¬(∃xP(x)) ≡ ∀x¬P(x) |

- In the Universal quantifier, **_∀xP(x) is true_** if *P(x) is true for all values of x*, and **_false_** if *there exist a value of x which will make P(x) false*.
- In the Existential quantifier, **_∃xP(x) is true_** if *there exist a value of x which will make P(x) true*, and **_false_** if *P(x) is false for all values of x*.
- We also took a glimpse of Nested Quantifiers. Below is a comparison table for each of the combinations (universal and existential):

  | Statement | TRUE when | FALSE when |
  | :---: | :---: | :---: |
  | ∀x∀yP(x,y) | P(x,y) is true for every pair x, y | There is a pair x, y for which P(x, y) is false |
  | ∀y∀xP(x,y) | P(x,y) is true for every pair x, y | There is a pair x, y for which P(x, y) is false |
  | ∀x∃yP(x,y) | For every x there is a y for which P(x,y) is true | There is an x such that P(x,y) is false for every y |
  | ∃x∀yP(x,y) | There is an x for which P(x,y) is true for every y | For every x there is a y for which P(x,y) is false |
  | ∃x∃yP(x,y) | There is pair x, y for which P(x,y) is true | P(x,y) is false for every pair x, y |

- Afterwhich, we moved on to Rules of Inference, which is like the Logical Equivalence Laws. Rules of Inference are used to prove an argument. Below is a table of Rules of Inference:

 | Rule of Inference | Tautology  |  Name  |
 | :-------: | :--------------: | :---------: |
 | p<br/>p→q<br/>∴q |  (p ∧ (p → q)) → q  | Modus Ponens  |
 | ¬q<br/>p → q<br/>∴ ¬p  |  (¬q ∧ (p → q)) → ¬p |  Modus Tollens  |
 | p → q<br/>q → r<br/>∴ p → r  | ((p → q) ∧ (q → r)) → (p → r) |  Hypothetical Syllogism  |
 | p ∨ q<br/>¬p<br/>∴ q  | ((p ∨ q) ∧ ¬p) → q   |  Disjunctive Syllogism |
 | p<br/>∴ p ∨ q  |  p → p ∨ q  |  Addition  |
 | p ∧ q<br/>∴ p  |  (p ∧ q) → p  | Simplification  |
 |  p<br/>q<br/>∴ p ∧ q |  ((p) ∧ (q)) → (p ∧ q)  |  Conjunction  |
 | p ∨ q<br/>¬p ∨ r<br/>∴ q ∨ r  |  ((p ∨ q) ∧ (¬p ∨ r)) → q ∨ r | Resolution  |

- I was also able to answer some quesions during class including:

  Number-Letter of Question |  Question | Answer
:------------------------:|---------|:-----:
7-b | Use De Morgan's laws to find the negation of "Carlos will bicycle or run tomorrow". | Carlos will not bicycle tomorrow and will not run tomorrow.
15 | Determine whether (¬q ∧ (p → q)) → ¬p is a tautology. | *Answer in Table 1 below*
17 | Show that ¬(p ↔ q) and p ↔ ¬q are logically equivalent. | *Answer in Table 2 below*

  Number-Letter of Question |  Question | Answer
:------------------------:|---------|:-----:
3-c | Let Q(x,y) denote the statement "x is the capital of y." Is Q(Massachusetts, Boston) true?. | False
3-d | Let Q(x,y) denote the statement "x is the capital of y." Is Q(New York, New York) true?. | False
7-b | Translate ∀x(C(x) ∧ F(x)) into English, where C(x) is "x is a comedian" and F(x) is "x is funny" and the domain consists of all people. | Every person is a funny comedian.
11-a | Let P(x) be the statement "x = x^2." If the domain consists of integers, is P(0) true? | True 
13-b | Determine the truth value of ∃n(2n = 3n) if the domain consists of all integers. | True 
17-a | Suppose that the domain of the propositional function P(x) consists of the integers 0, 1, 2, 3, and 4. Write out ∃xP(x) using disjunctions, conjunctions, and negations. | Disjunction

  Number-Letter of Question |  Question | Answer
:------------------------:|---------|:-----:
1-a | Translate ∀x∃y(x < y) into English, where the domain for each variable consists of all real numbers. | For all x there exists a y such that x is less than y.
3-e | Let Q(x, y) be the statement “x has sent an e-mail message to y,” where the domain for both x and y consists of all students in your class. Express ∀y∃xQ(x, y) in English. | All students in your class has been sent an e-mail message from some students in your class.

  * I was also asked to give an example of Modus Ponens and answered: Punu is cute, and if Punu is cute then Punu is cuddly; therefore Punu is cuddly.
<br/>
<br/>
**Table 1 for answered question:**

   p | ¬p | q | ¬q | p → q | ¬q ∧ (p → q) | (¬q ∧ (p → q)) → ¬p
 :---:|:---:|:---:|:---:|:---:|:---:|:---:
  T | F | F | T | F | F | **T**
  F | T | T | F | T | F | **T**
  T | F | T | F | T | F | **T**
  F | T | F | T | T | T | **T**
<br/>
  **Table 2 for answered question:**

   p | q | ¬q | p ↔ q | ¬(p ↔ q) | p ↔ ¬q |
 :---:|:---:|:---:|:---:|:---:|:---:
  T | T | F | T | **F** | **F** 
  F | F | T | T | **F** | **F** 
  T | F | T | F | **T** | **T** 
  F | T | F | F | **T** | **T** 

<br/>
#### Assignment:
- 5.b. Let W(x, y) mean that student x has visited website y, where the domain for x consists of all students in your school and the domain for y consists of all websites. Express ∃xW(x, www.imdb.org) by a simple English sentence.
  * **There exist a student in your school who has visited www.imdb.org.**

- 7.c. Let T (x, y) mean that student x likes cuisine y, where the domain for x consists of all students at your school and the domain for y consists of all cuisines. Express ∃y(T (Monique Arsenault, y) ∨ T (Jay Johnson, y)) by a simple English sentence.
  * **There exist a cuisine that either Monique Arsenault or Jay Johnson likes.**

- 9.d. Let L(x, y) be the statement “x loves y,” where the domain for both x and y consists of all people in the world. Use quantifiers to express "Nobody loves everybody".
  * **¬∃x∀yL(x, y)**

- (1.6)35. Determine whether this argument, taken from Kalish and Montague [KaMo64], is valid.
<br/>If Superman were able and willing to prevent evil, he would do so. If Superman were unable to prevent evil, he would be impotent; if he were unwilling to prevent evil, he would be malevolent. Superman does not prevent evil. If Superman exists, he is neither impotent nor malevolent. Therefore, Superman does not exist.
  * Let A be “Superman is able to prevent evil”, W be “Superman is willing to prevent evil”, P be “Superman prevents evil”, I be “Superman is impotent”, M be “Superman is malevolent”, and E be “Superman exists”.
  <br/>
  <br/>
**Premises are**:
  * 1. (A ∧ W) → P
  * 2. ¬A → I
  * 3. ¬W → M
  * 4. ¬P
  * 5. E → (¬I ∧ ¬M)
  <br/>
  <br/>
**Solution**:
  * 6. Modus Tollens on #1 and #4: ¬(A ∧ W)
  * 7. De Morgan's law on #6: ¬A ∨ ¬W
  * 8. Resolution on #2 and 7: I ∨ ¬W
  * 9. Resolution on #3 and 8: M ∨ I
  * 10. De Mordan's law on #9: ¬M ∧ ¬I
  * 11. Modus Tollens on #5 and #10: ¬E
  <br/>
  <br/>
Therefore, the argument is **VALID**.

<br/>
# WEEK 3
- The first thing we did was to answer our superman assignment. I found out that it would be more orderly and understandable when every step (logical equivalences, rules of inference) is stated.
- I was able to express my opinion on what I think is the correct law/rule to be used in order to further prove the statement in the superman question. (Modus Tollens on #1 and #4: **_¬(A ∧ W)_** ).
- We proceeded to a really brief discussion on Fallacies. **_Fallacies resemble rules of inference, but are based on contingencies rather than tautologies. In short, it is a common form of incorrect reasoning which leads to  invalid arguments._**
- We also learned about the concept of instantation. Instantation is a method of getting a specific sample in the given domain. There are 2 types of instantation: Universal Instantation and Existential Instantation. These two only differ in the "Universal" or "Existential" part.
<br/>
- On our second meeting of the week, we only answered our given items from the assignment (Chapter 1.7).
- I was also able to answer some quesions during class including:

  Number-Letter of Question |  Question | Answer
:------------------------:|---------|:-----:
(1.6) Example 7 | After establishing the premise r → s, what must be the next step (what rule/law must be applied) to come up with the conclusion ¬q → s? | Hypothetical Syllogism on the argument obtained in step 4 (¬q → r) and the premise established in step 5 (r → s): **¬q → s**
(1.6) 1 | Find the argument form for the following argument and determine whether it is valid. Can we conclude that the conclusion is true if the premises are true? <br/> If Socrates is human, then Socrates is mortal. <br/> Socrates is human. <br/> ∴ Socrates is mortal. | Modus Ponens - Valid

<br/>
#### Assignment:
- (1.7) 3. Show that the square of an even number is an even number using a direct proof.
  * If n is even, then n^2 is even.
  * **p** = n is even || **q** = n^2 is even
  * If p is *true*: n = 2k
  * n^2 = (2k)^2 = 4k^2 = 2(2k^2)
  * Let m = 2k^2
  * Therefore, **2m**

- (1.7) 17. Show that if n is an integer and n^3 + 5 is odd, then n is even using (a) a proof by contraposition.
  * p → q = ¬q → ¬p
  * If n is an integer and n^3 + 5 is odd, then n is even.
  * **¬q** = n is odd || **¬p** = n^3 + 5 is even
  * Odd integers: n = 2k + 1
  * Substituting n in n^3 + 5: (2k+1)^3 + 5 = 8k^3 + 12k^2 + 6k + 6 = 2(4k^3 + 6k^2 + 3k + 3)
  * Let m = 4k^3 + 6k^2 + 3k + 3
  * Therefore, **2m** (Even)

<br/>
# WEEK 4
- This week we continued with our topic on proving or proofs. There are 5 methods of proving: Direct Proof, Proof by Contraposition, Proof by Contradiction, Vacuous Proof, and Proof of Equivalence. But we mainly discussed the first three methods.
  * Direct Proof - given **p → q**, we **assume p is true** then **prove that q must also be true**
  * Proof by Contraposition - given **p → q**, we **let p → q ≡ ¬q → ¬p** then apply **direct proof on ¬q → ¬p**
  * Proof by Contradiction - given **p → q**, we assume **p is true** and **¬q is true**, then substitute ¬q in p which will lead to a contradiction
- I was also able to answer some quesions during class including:

  Number-Letter of Question |  Question | Answer
:------------------------:|---------|:-----:
(1.7) 33 | Show that these statements about the real number x are equivalent: (i) x is irrational, (ii) 3x + 2 is irrational, (iii) x/2 is irrational. | Use Proof by Contraposition on (i) → (ii), (ii) → (i), (i) → (iii), and then on (iii) → (i). These will result to: (i) → (ii) will show that x is rational, (ii) → (i) will show that 3x + 2 is rational, (i) → (iii) will show that x is rational, and lastly, (iii) → (i) will show that x/2 is rational.
(1.8) 1 | Prove that n^2 + 1 ≥ 2^n when n is a positive integer with 1 ≤ n ≤ 4 | Using Proof by Cases: <br> @n=1: 1^2 + 1 = 2 ≥ 2 = 2^1 <br> @n=2: 2^2 + 1 = 5 ≥ 4 = 2^2 <br> @n=3: 3^2 + 1 = 10 ≥ 8 = 2^3 <br> @n=4: 4^2 + 1 = 17 ≥ 16 = 2^4 <br> @n=5: 5^2 + 1 = 26 ≤ 32 = 2^5 <br> Therefore, the statement is TRUE.
(1.8) 5 | Prove using the notion of without loss of generality that min(x, y) = (x + y − lx − yl)/2 and max(x, y) = (x + y + lx − yl)/2 whenever x and y are real numbers. | Since lx - yl = ly - xl, x and y are interchangeable. Applying "without loss of generality", we assume x ≥ y: <br> [x + y - (x - y)]/2 = [x + y - x + y]/2 = 2y/2 = y = min(x,y) <br> [x + y + (x - y)]/2 = [x + y + x - y]/2 = 2x/2 = x = max(x,y).

- We then proceeded to the discussion of sets. A **set** is an unordered collection of objects called elements.
- The statement a is an element of the set A is denoted by **a ∈ A**.
- Below is a list of different sets denoted  by specific letters:
  * **N** = {0, 1, 2, 3, . . .}, the set of **natural numbers**
  * **Z** = {. . . ,−2,−1, 0, 1, 2, . . .}, the set of **integers**
  * **Z+** = {1, 2, 3, . . .}, the set of **positive integers**
  * **Q** = {p/q | p ∈ Z, q ∈ Z, and q ≠ 0}, the set of **rational numbers**
  * **R**, the set of **real numbers**
  * **R+**, the set of **positive real numbers**
  * **C**, the set of **complex numbers**
- We also discussed the different terms used under the topic of sets.
  * Empty or Null Set (∅) - set that has no elements
  * Subset (⊆) - given 2 sets, A and B, set A is a subset of B if and only if every element of A is also an element of B
  * Cardinality (| |) - number of unique elements of a set
  * Power Set (P( )) - set of all subsets of the set
-  I was also able to answer some quesions during class including:

  Number-Letter of Question |  Question | Answer
:------------------------:|---------|:-----:
(2.1) 1-b | List the members of the set {x l x is a positive integer less than 12} | {1,2,3,4,5,6,7,8,9,10,11}
(2.1) 4-a | For the pair: the set of people who speak English, the set of people who speak English with an Australian accent, determine whether the first is a subset of the second, the second is a subset of the first, or neither is a subset of the other. | the second is a subset of A.
(2.1) 5-b | Determine whether this {{1}}, {1, {1}} pair of sets is equal. | No. The first set has only 1 element, while the other set has 2 elements.
(2.1) 8-b,c | b) For the set {x ∈ R | x is the square of an integer} in Exercise 7, determine whether {2} is an element of that set. <br> c) For the set {2,{2}} in Exercise 7, determine whether {2} is an element of that set. | b) No. <br> c) Yes.
(2.1) 9-c,d | c) Determine whether {0} ⊂ ∅ is true or false. <br> d) Determine whether ∅ ⊂ {0} is true or false. | c) False <br> d) True.
(2.1) 10-c | Determine whether the statement {∅} ∈ {∅} is true or false. | True.
(2.1) 11-c | Determine whether the statement {x} ∈ {x} is true or false. | False.
(2.1) 19-d | What is the cardinality of {a, {a}, {a, {a}}} | 3
(2.1) 23-c | How many elements does the set P(P(∅)) have where a and b are distinct elements? | 2^1 = 2 elements

<br/>
# WEEK 5
- During the fifth week, we discussed about another method of proving which is the Mathematical Induction. **Mathematical Induction** consists of 2 steps: Bases and Inductive.
  * **Basis** - In this step, the output of the given formula or equation is checked.
  * **Inductive** - In this step, direct proving is applied: Assume P(k) is true, and then substitute P(k) in P(k+1).
- Induction - from specific to general (theory)
- Deduction - from general (theory) to specific
- I was also able to answer some quesions during class including:

  Number-Letter of Question |  Question | Answer
:------------------------:|---------|:-----:
(5.1) 1 | There are infinitely many stations on a train route. Suppose that the train stops at the first station and suppose that if the train stops at a station, then it stops at the next station. Show that the train stops at all stations. | Let P(n) = the train stops at station n. <br> Basis: P(1) is true. <br> Inductive: P(k) → P(k+1) for each k≥1.
(5.1) 5 | Prove that 1^2 + 3^2 + 5^2 + ··· +(2n + 1)^2 = (n + 1)(2n + 1)(2n + 3)/3 whenever n is a nonnegative integer. | Let P(n) = 1^2 + 3^2 + 5^2 + ... + (2n + 1)^2 = (n + 1)(2n + 1)(2n + 3)/3 <br> Basis: P(0) => 1^2 = 1 = (0 + 1)[2(0) + 1][2(0) + 3]/3 <br> Inductive: Assume P(k) is true, then: 1^2 + 3^2 + ··· + (2k + 1)^2 + [2(k+1)+ 1]^2 = (k + 1)(2k + 1)(2k + 3)/3 + (2k + 3)^2 = (2k + 3)[(k + 1)(2k + 1)/3 + (2k + 3)] = (2k + 3)(2k^2 + 9k + 10)/3 = (2k + 3)(2k + 5)(k + 2)/3 = [(k + 1) + 1][2(k + 1) + 1][2(k + 1) + 3]/3

-We also had our first quiz this week which was about all the topics that has been discussed up until last meeting, but mainly about proving.

<br/>
# WEEK 6
- We didn't have a meeting on the 19th because it was called off for our preparation of our thesis.
- On thursday, we proceeded to the next topic which was about Functions. A **function** mainly consist of two parts: a **domain** and a **codomain**.
  * Domain  - the set of all possible inputs of a function which allow the function to work
  * Codomain - the set of all possible outputs of a function
  * Range - a subset of Codomain
- There are also three types of functions discussed:
  * One-to-One (**Injunction**) - given any **b** in set B, there is only one **a** in set A that can be paired with the given **b**
  * Onto (**Surjection**) - if every element **b** in set B has a corresponding element **a** in set A such that f(a) = b
  * One-to-One and Onto (**Bijection**) - each element of set A is paired with exactly one element of set B, and each element of the set B is paired with exactly one element of set A (no unpaired elements)
- I was also able to answer some quesions during class including:

  Number-Letter of Question |  Question | Answer
:------------------------:|---------|:-----:
(2.3) 3-b | Determine whether f is a function from the set of all bit strings to the set of integers if f (S) is the number of 1 bits in S. | It is a function.
(2.3) 4-d | Find the domain and range of the function that assigns to a bit string the number of bits in the string. Note that in each case, to find the domain, determine the set of elements assigned values by the function. | Domain: a bit string <br> Range: all positive integers

<br/>
#### Assignment:
- (2.3) 15. Determine whether the function f : Z × Z → Z is onto if <br> a) f (m, n) = m + n <br> b) f (m, n) = m^2 + n^2 <br> c) f (m, n) = m <br> d) f (m, n) = |n| <br> e) f (m, n) = m − n.
  * a) Given any integer n, f(0,n) = n. Therefore, ONTO.
  * b) Range has no negative **Z**. Therefore, Not ONTO.
  * c) Given any integer m, f(m,1) = m. Therefore, ONTO.
  * d) Range has no negative **Z**. Therefore, Not ONTO.
  * e) Given any integer m, f(m,0) = m. Therefore, ONTO.

<br/>
# WEEK 7
- During this week, we continued answering exercises under the topic Functions.
- I was also able to answer some quesions during class including:

  Number-Letter of Question |  Question | Answer
:------------------------:|---------|:-----:
(2.3) 20-a | Give an example of a function from N to N that is one-to-one but not onto. | n + 1
(2.3) 20-b | Give an example of a function from N to N that is onto but not one-to-one. | \lfloor n + 0.5 \rfloor
(2.3) 22-b | Determine whether the function f (x) = −3x^2 + 7 is a bijection from R to R. | Not a Bijection.

<br/>
# WEEK 8
...
