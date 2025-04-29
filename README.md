# informatics---inf2b-coursework-2-solved
**TO GET THIS SOLUTION VISIT:** [Informatics – Inf2B Coursework 2 Solved](https://www.ankitcodinghub.com/product/informatics-inf2b-coursework/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;116046&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;Informatics - Inf2B Coursework 2 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
1 Outline

The coursework consists of two tasks, Task 1 – data analysis and classification with multivariate Gaussian classifiers, Task 2 – neural networks.

https://www.inf.ed.ac.uk/teaching/courses/inf2b/coursework/cwk.html

http://web.inf.ed.ac.uk/infweb/admin/policies/academic-misconduct

For late coursework and extension requests, see the page: http://web.inf.ed.ac.uk/infweb/student-services/ ito/admin/coursework-projects/late-coursework-extension-requests

Note that any extension request must be made to the ITO, and not to the lecturer.

Programming: Write code in Matlab(R2018a)/Octave or Python(version 3.6)+Numpy+Scipy+Matplolib. Your code should run on standard DICE machines without the need of any additional software. Code templates are available from the following directory:

/afs/inf.ed.ac.uk/group/teaching/inf2b/cwk/matlab code

There are some functions that you should write the code by yourself rather than using those of standard libraries available. See section 4 for details.

This document assumes programming in Matlab. For Python, put all the specified functions into a single file for each Task, so that task1.py for Task 1, and task2.py for Task 2. Output data should be stored in Matlab’s MAT binary format.

2 Data

2.1 Data for Task 1

The coursework employs the Anuran Calls (MFCCs) Data Set introduced by J. Colonna etal..

1

Your data set file, ‘dset.mat’, which is a subset of the original data set, should be found in your coursework data directory (denoted as YourDataDir hereafter) :

/afs/inf.ed.ac.uk/group/teaching/inf2b/cwk/d/UUN/

where UUN denotes your UUN (DICE login name).

You can use Matlab’s load() function to load the data set in the following manner:

load(pathname);

where pathname denotes the absolute pathname of your data set file. Once you load the data set, you will find the following variables.

Matlab variable (Class) Description

X[N, D] (double)) feature vectors

Y family[N,1] (int32) family class labels

Y genus[N,1] (int32) genus class labels Y species[N,1] (int32) species class labels list family[4,1] (cell) family class names list genus[8,1] (cell) genus class names list species[10,1] (cell) species class names

where N and D denotes the total number of samples and the dimension of feature vector (D=24), respectively.

Among the three different levels of taxonomic rank provided in the original data set, we use ’species’ in the coursework. There are ten different species, so that the number of classes for classification is ten, i.e., C = 10. The variable, Y species(i), contains the integer number that corresponds to the species of i-th sample, whose feature vector is X(i,:). Hereafter, Y denotes Y species.

The variable, list species, holds the list of species names.

Family Genus Species # of samples

Leptodactylidae Leptodyctylus Leptodactylus fuscus 222

Adenomera Adenomera andreae 496

Adenomera hylaedactyla 3049

Hylidae Dendropsophus Hyla minuta 229

Scinax Scinax ruber 96

Osteocephalus Osteocephalus oophagus 96

Hypsiboas Hypsiboas cinerascens 429

Hypsiboas cordobae 702

Bufonidae Rhinella Rhinella granulosa 135

Dendrobatidae Ameerega Ameerega trivittata 544

The data set has not been split in two sets for training and testing. You need to split the data set according to the instructions described later.

2.2 Data for Task 2

The data for Task 2 is stored in the plain-text file named ‘task2 data.txt’ in YourDataDir. For details, see the Task 2 specifications.

3 Task specifications

(a) Write a Matlab function task1 1() that

• calculates the covariance matrix, S, and correlation matrix, R, for the data set X, using the maximum likelihood estimation (MLE),

• saves S as ‘t1 S.mat’,

• saves R as ‘t1 R.mat’.

The specifications of the variables are as follows.

S D-by-D covariance matrix (in double)

R D-by-D correlation matrix (in double)

Save the code as ‘task1 1.m’. Note that, hereafter, function and file names are case sensitive, and your code should save output files in the current working directory. The syntax of the function should be as follows.

function task1 1(X, Y)

where

X N-by-D matrix of feature vector (of floating-point numbers in double-precision format, which is the default in Matlab), where N is the number of samples, and D is the the number of elements in a sample. Note that each sample is represented as a row vector rather than a column vector.

Y N-by-1 label vector (in int32) for X. Y(i) is the class number of X(i,:).

(b) Run the following:

task1 1(X, Y);

Make sure that the two output files are created properly. It will be a good idea that you write a script to run the above.

Look into the correlation matrix, R, you obtained, and describe your findings in your report, using graphs.

(a) Write a Matlab function task1 3() that

• calculates the eigenvectors, EVecs and eigenvalues, EVals, of a covariance matrix, and calculates the cumulative variance , Cumvar,

• finds the minimum number of PCA dimensions to cover each 70%, 80%, 90%, 95% of the total variance, and store the values to a vector MinDims,

• saves the eigenvectors to a file named ‘t1 EVecs.mat’,

• saves the eigenvalues to a file named ‘t1 EVals.mat’,

• saved the cumulative variance to a file named ‘t1 Cumvar.mat’,

• saves the the numbers of minimum dimensions, MinDims, to a fle named ‘t1 MinDims.mat’,

Save the function as ‘task1 3.m’.

The syntax of the function should be as follows. function task1 3(Cov)

where Cov is a D-by-D covariance matrix (double).

The specifications of the variables are as follows.

EVecs D-by-D matrix of column-wise eigen vectors (in double)

EVals D-by-1 vector of eigen values (in double)

Cumvar D-by-1 vector of cumulative variance (in double)

MinDims 4-by-1 vector of (in int32)

The eigenvalues should be sorted in descending order, so that λ1 is the largest and λD is the smallest, and i’th column of EVecs should hold the eigenvector that corresponds to λi.

Eigenvectors are not unique by definition in terms of scale (length) and sign, but we make them unique in this coursework by putting the following additional constraints, which your program should employ.

• The first element of each eigenvector is non-negative. If it is not the case, i.e. if the first element is negative, multiply -1 to the eigenvector (i.e. v ← −v) so that it gets the opposite direction.

• Each eigenvector is a unit vector, i.e. kvk = 1, where v denotes an eigenvector. As far as you use Matlab’s eig() or Python’s numpy.linalg.eig(), you do not need to care about this, since either function ensures unit vectors.

(b) Run the following:

task1 3(S);

In your report, show a graph of cumulative variance.

(c) Plot all data on a 2D-PCA plane, clarifying data of different classes, and show the graph in your report. There is no need to submit a code file for this.

(a) Write a Matlab function task1 mgc cv() that carries out a classification experiment with multivariate Gaussian classifiers, using k-fold cross validation, and save the code as ‘task1 mgc cv.m’.

The syntax of the function is as follows function task1 mgc cv(X, Y, CovKind, epsilon, Kfolds)

For each fold, p, the function should

• estimate the mean vector and covariance matrix for each class from the samples that do not belong to partition p.

• save the mean vectors (Ms) to ‘t1 mgc &lt;Kfolds&gt;cv&lt;p&gt; Ms.mat’,

• save the regularised covariance matrices (Covs) to ‘t1 mgc &lt;Kfolds&gt;cv&lt;p&gt; ck&lt;CovKind&gt; Covs.mat’

• carry out a classification experiment using the samples of partition p, and save the confusion matrix (CM) to ‘t1 mgc &lt;Kfolds&gt;cv&lt;p&gt; ck&lt;CovKind&gt; CM.mat’,

• calculate the final confusion matrix (where each element is a relative frequency) and save it to ‘t1 mgc &lt;Kfolds&gt;cv&lt;L&gt; ck&lt;CovKind&gt; CM.mat’, where L = Kfolds + 1.

In the above, replace &lt;p&gt;, &lt;Kfolds&gt;, &lt;CovKind&gt;, and &lt;L&gt; with the actual values. The specifications of the variables are as follows.

PMap N-by-1 vector (in int32)

Ms C-by-D matrix of mean vectors (in double)

Covs C-by-D-by-D array of covariance matrices (in double)

CM C-by-C confusion matrix (in double)

Details about the evaluation with the k-fold cross validation and the variables to save are specified in separate sheets.

(b) Run the function with epsilon=0.01 and Kfolds=5 for each CovKind=1,2,3, and report the accuracy (correct classification rate) in your report.

Using CovKind=1 (i.e. full covariance), investigate how the classification accuracy changes with respect to the regularisation parameter, epsilon. Plot a graph and describe your findings in your report.

In this task, you implement neural networks for binary classification problems, in which input feature is represented as a two-dimensional vector (x1,x2)T. We assume that decision regions are defined with polygon(s), whose specifications are given in the polygon specification file ‘task2 data.txt’ in YourDataDir. The file is a plain-text file, in which each line specifies the name of the polygon and the coordinates of its vertices in a sequential order, where P is the number of vertices. The following is an example of the file.

Polygon A: -1 -0.5 6 1.25 6 6.25 1 6

Polygon B: 2.5 3 3.5 3 3.5 3.5 2.5 3.5

Consider a single neuron with a unit function, whose output is defined as y(x) = h(wTx), where h(a) is a step function such that h(a) = 1 if a &gt; 0, and h(a) = 0 otherwise. Implement this neuron as a Matlab function:

function [Y] = task2 hNeuron(W, X)

where X is a N-by-D data matrix (double), W is a (D+1)-by-1 weight matrix (double), Y is a N-by-1 output vector (double). Save the function as ‘task2 hNeuron.m’.

Note that this function should be capable of taking more than one input vector stored in a matrix X, where each input vector is represented as a row vector rather tha:n a column one, and gives corresponding output as a vector Y.

Similar to task2 hNeuron() above, but consider another neuron which employs the logistic sigmoid function . Implement this neuron as a Matlab function:

function [Y] = task2 sNeuron(W, X) and save it as ‘task2 sNeuron.m’.

Find the structure (i.e. connection of neurons) and weights of the neural network that classifies the inside of Polygon A as Class 1 (i.e. y(x) = 1), and the outside and periphery as Class 0 (i.e. y(x) = 0), where each neuron is modelled with task2 hNeuron().

This task is meant for you to work using pen and paper (and calculator), but it is also fine that you write a piece of code to find the weights. If it is the case, save the script or function as ‘task2 find hNN A weights.m’.

Let wji` denote the weight of neuron j in layer ` from neuron i in layer `−1. Normalise your weights in such a way that maxi |wji` | = 1. Write the weights in a plain text file ‘task2 hNN A weights.txt’ in the following format.

You write each wji` in a separate line, for ` = 1,…, j = 1,…, and i = 0,1,…, so that the first line contains followed by and in the second line and the third line, respectively. The format of each line should be as follows:

W(`,j,i) : &lt;the value of wji` &gt;

where “&lt;the value of wji` &gt;” is the actual value of the weight. For example, if 35, the first line should look like this:

W(1,1,0) : 0.35

Spaces are only allowed just before and after “:”, and none in other places.p

In your report, show the structure of the network and explain how you found the weights.

Implement the neural network above as a function:

function [Y] = task2 hNN A(X)

and save it as ‘task2 hNN A.m’, where X and Y follow the same formats as the ones shown in Task 2.1, but we assume D=2 hereafter.

Using task2 hNN A(), write a script that plots the decision regions in a 2D space, and save the code as ‘task2 plot regions hNN A.m’. Save the graph as a PDF file named ‘t2 regions hNN A.pdf’.

We now consider the decision regions formed with Polygon A and Polygon B, whose classification rule is shown below:

Class 1 : A¯ ∩ B

Class 0 : A ∪ B¯

where A and B denote the inside of the corresponding polygon, A¯ denotes the complement of A.

Implement the corresponding neural network as a function:

function [Y] = task2 hNN AB(X) and save it as ‘task2 hNN AB.m’. Note that each neuron should be modelled with task2 hNeuron().

Using task2 hNN AB(), write a script that plots the decision regions in a 2D space, and save the code as ‘task2 plot regions hNN AB.m’. Save the graph as a PDF file named ‘t2 regions hNN AB.pdf’.

We now consider another network task2 sNN AB() obtained by replacing all nodes of task2 hNeuron() with those of task2 sNeuron() in task2 hNN AB(), so that each neuron is now modelled with task2 sNeuron(). Implement the neural network as a function:

function [Y] = task2 sNN AB(X)

and save it as ‘task2 sNN AB.m’. Note that you will need to modify the weights to approximate the decision regions properly.

Using task2 sNN AB(), write a script that plots the decision regions in a 2D space, and save the code as ‘task2 plot regions sNN AB.m’. Save the graph as a PDF file named ‘t2 regions sNN AB.pdf’.

Investigate and discuss the decision regions for task2 sNN AB(), clarifying how and why they are different from those for task2 hNN AB().

4 Functions that are not allowed to use

4 Functions that are not allowed to use

Description of function Typical names Suggested name to implement

Pairwise (squared) Euclidean distance pdist2() MySqDist()

Compute the mean mean() MyMean()

Compute the covariance matrix cov() MyCov()

Compute the correlation matrix corr() MyCorr()

Compute Gaussian probability densities mvnpdf()

K-NN classification fitcknn() run knn classifier()

K-means clustering kmeans() my kMeansClustering()

Compute confusion matrix

Other utilities for classification confusion() comp confmat()

Description Typical names

Sum function sum()

Cumulative sum cumsum()

Square root function sqrt()

Exponential function e, exp()

Logarithmic function log(), ln()

Matrix transpose transpose(), ‘

Matrix inverse inv()

Determinant det()

Log determinant logdet() ··· available in Inf2b cwk directory

Eigen values/vectors eig()

Sort sort()

Sample mode mode()

Vectorisation helpers bsxfun(), arrayfun()

(NB: the list is not exhaustive)

5 Submission

Since marking for each task will be done separately, you should prepare separate reports for the two tasks, and save your report files in PDF format and name them ‘report task1.pdf’ and ‘report task2.pdf’. Do not indicate your name anywhere in your reports. Your report should be concise and brief for each task.

In the following instructions, DICE environment is assumed, but it is possible to do the same more easily on a personal computer if the archiver tool, ’tar’, is available in the environment.

Step 1 – Create a directory for submission

Create a directory named LearnCW, copy all the files to submit to the directory. A list of files to submit is available from the coursework web page. In addition to the files shown on the list, you should include the functions of your own such as MyCov.m so that your submitted code runs properly on DICE without the need of additional software. Do NOT, however, include the data set files in it.

5 Submission

Step 2 – Create an archive file for submission

Run the following command in a terminal window. tar -cvzf inf2b-cw-UUN.tar.gz LearnCW

where UUN denotes your UUN (DICE login name, e.g. s1234567). The command above creates an archive file named inf2b-cw-UUN.tar.gz. Before moving to Step 3, run the following command to check the contents of the archive file you created.

tar -tvf inf2b-cw-UUN.tar.gz

Step 3 – Submit the archive file via Learn

Choose “Assessment” from the menu in Inf2b page on Learn, and choose “Assignment Submission”. Upload the archive file, inf2b-cw-UUN.tar.gz, and click the ’submit’ button at the bottom-right corner of screen. If the submission is successful, you should receive a confirmation message from the system via email. For details and for any troubles, please see the following blog post:
