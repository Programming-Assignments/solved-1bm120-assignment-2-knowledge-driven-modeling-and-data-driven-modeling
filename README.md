Download Link: https://assignmentchef.com/product/solved-1bm120-assignment-2-knowledge-driven-modeling-and-data-driven-modeling
<br>
Assignment 2 is composed of two tasks: knowledge-driven modeling and data-driven modeling. That is, in the former case you must create two fuzzy inference systems (FIS) using domain knowledge, while in the latter case the model will be generated automatically using a machine learning approach.

<h1>Fuzzy models for clinical decision support</h1>

When a patient enters the Emergency Department of a hospital, his vitals and blood levels are immediately checked by a nurse. The following measurements are deemed important and are recorded by the nurse:

<ul>

 <li>Heart beats (per minute)</li>

 <li>Systolic blood pressure (in mmHg)</li>

 <li>Glucose level (mmol/L in the blood)</li>

 <li>Leukocyte count (per nL in the blood)</li>

</ul>

These combined measurements give insights in the health status of the patient and indicate how severe his condition is. Therefore, the head nurse decides based on these measurements in which order the patients should be examined by the doctors. However, there is only one head nurse available in the hospital, which leads to problems when multiple patients enter the Emergency Department at the same time. This also means that this nurse can not leave her working spot for breaks.

The management of the Emergency department has asked you to come up with an automated system to order the patients based on the severity of their condition and to build a prototype of this system to show the viability. Unfortunately, there is no data available, so you will have to go the ‘knowledge-driven’ way.

You have decided to develop a fuzzy model that gives each patient a health status score based on their bloodwork. What this score looks like (for example the range) is up to you. You can use any source to determine the parameters of the fuzzy sets. For example, for the blood level variables you could use:

<a href="https://www.catharinaziekenhuis.nl/files/Verwijzer/Specialismen_en_afdelingen/Laboratorium_algemeen_klinisch/Referentiewaarden/20210406_appreferentiewaardenlijst_V37.pdf">https://www.catharinaziekenhuis.nl/files/Verwijzer/Specialismen_en_afdelingen/Laboratorium_alge </a><a href="https://www.catharinaziekenhuis.nl/files/Verwijzer/Specialismen_en_afdelingen/Laboratorium_algemeen_klinisch/Referentiewaarden/20210406_appreferentiewaardenlijst_V37.pdf">meen_klinisch/Referentiewaarden/20210406_appreferentiewaardenlijst_V37.pdf</a>. Since ‘healthy’ values can be different for different demographic groups, you can assume your model has to work for adult males.

Document your modeling decisions and assumptions well and refer to the sources you used to determine the parameter settings. Show with some examples your model works well and orders the patient logically. In order to do that, create the data of three patients with varying health statuses, and show that your model orders them properly.

To summarize, for the first part of the Assignment you must:

<ul>

 <li>Implement a fuzzy inference system (FIS) to support the clinical decisions using the Simpful python library (2 point);</li>

 <li>Define and implement the fuzzy sets and show them in graphs (2 points);</li>

 <li>Justify the choice of your parameters (2 points);</li>

 <li>Define the fuzzy rules with proper operator usage and explain their rationale (2 points); ● Show that the model works and does what it needs to do with some examples (2 points).</li>

</ul>

<h1>Data-driven modeling</h1>

An investment company would like to sell part of their real estate property. They would like to know what characteristics determine the house prices, and what would be a good price for the houses they wish to sell. Therefore, the management asks you to develop a model that predicts price based on historical data.

The historical data (which you can find in the file <em>previous_house_sales.csv</em>) contains data on 496 previously done transactions, of which the following variables are recorded::

<ol>

 <li><strong><em>crim: </em></strong>per capita crime rate by town.</li>

 <li><strong><em>zn: </em></strong>proportion of residential land zoned for lots over 25,000 sq.ft.</li>

 <li><strong><em>indus: </em></strong>proportion of non-retail business acres per town.</li>

 <li><strong><em>nox: </em></strong>nitrogen oxides concentration (parts per 10 million).</li>

 <li><strong><em>rm: </em></strong>average number of rooms per dwelling.</li>

 <li><strong><em>age: </em></strong>proportion of owner-occupied units built prior to 1940.</li>

 <li><strong><em>dis: </em></strong>weighted mean of distances to five Boston employment centres.</li>

 <li><strong><em>rad: </em></strong>index of accessibility to radial highways.</li>

 <li><strong><em>tax: </em></strong>full-value property-tax rate per $10,000.</li>

 <li><strong><em>ptratio: </em></strong>pupil-teacher ratio by town.</li>

 <li><strong><em>lstat: </em></strong>lower status of the population (percent).</li>

 <li><strong><em>price: </em></strong>median value of the house in $1000s.</li>

</ol>

There are 10 houses that are meant to be sold by the investment company. Their characteristics are contained in the dataset <em>houses_to_be_sold.csv</em>. What should their prices be, based on your fuzzy model?

For the second part of the Assignment you must:

<ul>

 <li>Use the data set <em>csv </em>to build a predictive Takagi-Sugeno FIS able to predict the price of houses given the other variables (3 points). Provide argumentation for your model’s setting (for example, first – or zero order model etc.);</li>

 <li>Investigate the impact to performances (rely on pyFUME’s cross-validation functionality) using 2, 3 and 4 clusters (3 points);</li>

 <li>Provide an interpretation of the rules (2 points);</li>

 <li>Predict the prices of the houses in the houses_to_be_sold.csv dataset<a href="#_ftn1" name="_ftnref1"><sup>[1]</sup></a> (1 point).</li>

</ul>

<h1>Final information</h1>

You have to produce and submit on Canvas <strong>four </strong>files:

<ul>

 <li>the <strong>python source code for the first part </strong>of the assignment (knowledge-driven modeling with Simpful);</li>

 <li>the <strong>python source code for the second part </strong>of the assignment (data-driven modeling with pyFUME);</li>

 <li>the <strong>executable file containing the Simpful model/code </strong>(as produced by pyFUME) for the second part of the assignment;</li>

 <li>a <strong>report (in .pdf-format) </strong>containing all the information and comments as required by the assignments above.</li>

</ul>

The page limit (mandatory) is <strong>6 pages</strong>. Try to aggregate multiple results in the same figure, where possible.

The source code can be <strong>either a python script or a jupyter notebook</strong>. A SINGLE python file for the first part, a TWO python files for the second part (one containing the pyFUME code, one containing the Simpful model).

<a href="#_ftnref1" name="_ftn1">[1]</a> The group that comes closest to the actual values wins some bars of Tony’s chocolate, to be picked up at TU/e’s Atlas building.