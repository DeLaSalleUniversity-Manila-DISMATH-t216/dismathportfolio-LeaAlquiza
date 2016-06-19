# WEEK 1
- On our first meeting, our professor discussed a brief introduction on what Discrete Mathematics was about and how our learning in Algebra can help in analyzing Discrete Mathematics problems.
- Following the brief introduction, we had a recap on what Propositions are. And I learned that **Propositions are declarative statements that can be answered by either true or false.
- We were also asked one question each about propositions. I was asked if **2+3=5** was a proposition, and my answer was **yes** because it's true that 2 plus 3 is equal to 5.

- On our next meeting, we had officially started our class. We had a review type of discussion since we had already taken the course LOGICIR.
- The review type discussion started with some exercises and if we encounter unfamiliar terms our professor discusses them first and then proceeds with the exercises again.
- Recalling all logical operations:<br/>
		Operator                 Symbol             Expression          
  ------------------------------------   ------   ------------------------------- 
             Negation (NOT)                 ¬                   ¬p              
            Conjunction (AND)               ∧                 p ∧ q             
            Disjunction (OR)                ∨                 p ∨ q             
       Exclusive Disjunction (XOR)          ⊕     p ⊕ q ≡ (¬p ∧ q)  ∨  (p ∧ ¬q) |
       Conditional (IF-THEN, etc.)          →             p → q ≡ ¬p ∨ q        
  Biconditional (IF AND ONLY IF, etc.)      ↔       p ↔ q ≡ (p → q) ∧ (q → p) |  
- Additionally, we also learned about Inverse, Converse, and Contrapositive. Expressing these three in logical expression form, assuming p → q:
Conditinal Operator |  Expression 
--------------------|------------
Inverse | ¬p → ¬q 
Converse | q → p 
Contrapositive | ¬q → ¬p

- I was also able to answer some quesions during class including:
Number-Letter of Question |  Question | Answer
--------------------------|-----------|-------
8-b | p: I bought a lottery ticket this week.<br/> q: I won the million dollar jackpot.<br/> Express p v q as an English sentence. | I bought a lottery ticket this week or I won the million dollar jackpot.
11-a | p: It is below freezing.<br/> q: It is snowing.<br/> Write "It is below freezing and snowing" using p and q and logical connectives (including negations). | p ∧ q 
13-g | p: You drive over 65 miles per hour.<br/> q: You get a speeding ticket.<br/> Write "Whenever you get a speeding ticket, you are driving over 65 miles per hour." using p and q and logical connectives (including negations). | q → p 
15-e | p: Grizzly bears have been seen in the area.<br/> q: Hiking is safe on the trail.<br/> r: Berries are ripe along the trail.<br/> Write "For hiking on the trail to be safe, it is necessary but not sufficient that berries not be ripe along the trail and for grizzly bears not to have been seen in the area." using p, q, and r and logical connectives (including negations). | (q → (¬r ∧ ¬p)) ∧ ¬((¬r ∧ ¬p) → p) 
17-a | Determine whether "If 1+1=2, then 2+2=5." is true or false. | False 
19-b | Determine whether "A password must have at least three digits or be at least eight characters long." an inclusive or, exclusive or, is intended. | Inclusive OR (because you can have a long password with digits in it) 
25-a | Write "If it is hot outside you buy an ice cream cone, and if you buy an ice cream cone it is hot outside." in the form of "p if and only if q" in English | You buy an ice cream cone if and only if it is hot outside. 
27-c | State the converse, contrapositive, and inverse of "A positive integer is a prime only if it has no divisors other than 1 and itslef." | Converse: A positive integer is a prime if it has no divisors other than 1 and itself.<br/> Contrapositive: If a positive integer does not have no divisors other than 1 and itself, then it is not prime.<br/> Inverse: If a positive integer is not prime, then it has a divisor other than 1 and itself. 
29-d | How many rows appear in a truth table for "(p ∧ r ∧ t) ↔ (q ∧ t)" | 2^4 = 16 
