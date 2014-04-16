## My understanding of formal methods in general and model checking in particular. ##

    lufei(13126112)

###What is Formal Methods###
Both formal specification techniques and formal verification techniques are referred to as formal methods collectively in literature.
Formal specification is concerned with producing an unambiguous set of product specifications so that customer requirements, as well as environmental constraints and design intentions, are correctly reflected, thus reducing the chances of accidental fault injections.
The basic idea of formal verification is to verify the correctness, or absence of faults, of some given program code or design against its formal specifications. Therefore, the existence of formal specifications is a prerequisite for formal verifications. 
When formal methods are used for software development, formal specifications are used upstream for requirement analysis and product specifications, and formal verifications or analyses are used downstream to verify the design and code before additional verification and validation (V&V) activities are carried out. Therefore, the use of formal methods can be summarized in the following two-step process:
Constructing formal specifications: The expected behavior and other properties of the software artifacts are represented in formal models.
Performing formal verifications: Formal analysis techniques are applied on the product components, typically product code or formal designs, to verify their correctness with respect to their formal specifications, or to check for certain properties.
Formal methods in general remain a costly alternative for ensuring software quality. This and other factors affect the applicability and effectiveness of formal verification analysis techniques in the quality engineering process.

###What is Model Checking###
Model checking is such an approach that automatically or algorithmically checks certain properties for some software systems. A good introduction to this topic can be found in Ghezzi et al. (2003), and the following briefly summarize the key ideas:
1. A software system is modeled as a finite-state machine (FSM), with some property of interest expressed as a suitable formula, or a proposition, defined with respect to the FSM. Ideally, this FSM and the propositions are both developed during the software specification process, much like the use of formal specifications in various formal methods.
2. The model checker is a software that runs an algorithm to check the validity of the proposition. If it is checked to be true, a proof is said to be produced. Otherwise, a counterexample is given, much like a failed test case that can be analyzed further for defect fixing.
