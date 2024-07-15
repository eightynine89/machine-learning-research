# Classification

- For classification models, the response variable is a qualitative variable: yes/no, e.g. eye color {brown|blue|green}
- Predicting a qualitative response for an observation can be referred to as classifying that observation, since it involves assigning the observation to a category, or class.
- X, Y, and C (set of variables): C(X) belongs to C
  - X is a vector (1-dimensional array) with different features
  - Pass these features to the function and it will return the output that belongs to the C set
- Other examples
  - A person arrives at the emergency room with a set of symptoms that could possibly be attributed to one of three medical conditions. Which of the three conditions does the individual have?
  - An online banking service must be able to determine whether or not a transaction being performed on the site is fraudulent, on the basis of the user’s IP address, past transaction history, and so forth.
  - On the basis of DNA sequence data for a number of patients with and without a given disease, a biologist would like to figure out which DNA mutations are deleterious (disease-causing) and which are not.
- Why Not Linear Regression?
  - there are at least two reasons not to perform classifica- tion using a regression method: (a) a regression method cannot accommodate a qualitative response with more than two classes; (b) a regression method will not provide meaningful estimates of `Pr(Y|X)`, even with just two classes. Thus, it is preferable to use a classification method that is truly suited for qualitative response values.

## Logistic Regression

- Considering a linear regression model: `p(X) = β₀ + β₁X`. The problem with this approach is that for balances close to zero we predict a negative probability of default — it can produce any real number
- In logistic regression, we use the logistic function (aka sigmoid function): `p(X) = (1 + e^(β₀+β₁X)) / e^(β₀+β₁X)`.
  - The logistic function maps any real-valued number into the range (0, 1). Negative responses and values greater than 1 are inherently removed because the logistic function constrains the output to a probability-like range (Probabilities, by definition, cannot be negative or exceed 1)
  - The logistic function will always produce an S-shaped curve of this form: For large positive inputs, the function approaches 1, and for large negative inputs, it approaches 0. This helps in creating a clear decision boundary between different classes.

## Questions

- [ ] TODO: logistic regression
- [ ] TODO: case-control sampling
- [ ] TODO: bayes theorem? foundation math behind? why is it used?
- [ ] TODO: gauss distribution
- [ ] TODO: poisson regression
- [ ] TODO: poisson regression vs gauss vs logistic regression
- [ ] TODO: the math behind poisson regression, gauss, logistic regression
- [ ] TODO: what's density? is it a statistics concept?
- [ ] TODO: what does mean a model being stable?