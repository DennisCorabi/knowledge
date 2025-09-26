# Linear programming

**Linear programming** is a branch of operational research (OR) whose purpose is to find the **optimal** outcome of a real-life problem that can be mathematically modelled as a system of linear relationships.

> Linear programming is sometimes called linear optimisation.

LP has proven useful in modelling math-backed suggestions regarding problems in transportation, telecommunications and manufacturing.
## Terminology

- **Objective function**: linear function of which we have to find the optimal solution (i.e. global maximum or minimum)
- **(In)equality constraint**: linear function that defines a constraint that the solution of the objective function must satisfy. There are usually more that one constrains in a normal LP problem.
- **Feasible region**: a convex polytope whose surface is defined as the intersection between (in)equality constrains.

## Some little history

- `1930`: Leonid Kantorovich and Wassily Leontief independently delved into the pratical applications of linear programming (how solving linear systems could impact the world)
- `1946:-47`: George B. Dantzig developed a linear programming algorithm to tackle this kind of problems in a reasonable amount of time. This algorithm is called **simplex method**.
- `1947`: John Von Neumann conjured the **theory of duality** while talking to Dantzig.
- `1979`: The simplex problem was shown to be solvable in polynomial time.

## Representation

### Standard form

The standard form is the most intuitive form of describing an LP problem.

![[lp-standard-form.png]]

Every other form to describe a linear programming problem can be rewritten in the standard form. There is one problem, though. If we want to apply the simplex algorithm, another form is required: the **augmented form**.
### Augmented form

In order to apply the simplex algorithm, a linear programming problem must be converted to an augmented form.

![[lp-augmented-form.png]]

The augmented form wants us to convert the inequalities in equalities. We can do that by introducing **slack variables**, mock variables that represents "what's missing" (i.e. to add) for the left-side of the inequality to be equal to the known term on the right side.

## Solutions

The goal of a linear programming algorithm is to find the point within the feasible region where the objective function is at its highest (or lowest, depending on the type of problem).

>[!important]
>Sometimes an optimal solution cannot be determined. 

For a maximum problem, this happens when at least two constrains have no solution in common or the shape of the feasible region is unbounded or bounded yet concave.

