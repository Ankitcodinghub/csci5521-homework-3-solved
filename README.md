# csci5521-homework-3-solved
**TO GET THIS SOLUTION VISIT:** [CSCI5521 Homework 3 Solved](https://www.ankitcodinghub.com/product/csci-5521-introduction-to-machine-solved-4/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;117036&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSCI5521 Homework 3 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
            5/5 - (2 votes)    </div>
    </div>
Questions

1. Derive the EM algorithm for estimating a mixture of Laplacian distributions (double exponential distributions). The probability density function of a Laplacian distribution for class Ci is

,

where µi and bi are referred to as the location and diversity parameters of the distribution. The mixture density of K Laplacian distributions is

,

where = 1. Given the data X = {x1,x2,…,xt,…,xN} , define the log-likelihood function and the complete log-likelihood function, and derive the EM equations including the expectation for the responsibility is the binary indicator of sample t in cluster i) and maximum likelihood learning for

{πi,µi,σi}i=1,…,K.

Important hint:

(a) There is no easy way to solve the maximum likelihood learning of µi. An approximation is to binarize γ(zit) as bti = 1 if i = argmaxjγ(zjt) and otherwise = 0 (the same as we do in k-means) before estimating µi. You should still use γ(zit) to estimate πi and σi.

(b) The absolute error is minimized if θ is the median of the N numbers).

2. In this question, we will implement the EM algorithm to estimate a mixture ofGaussian distributions for image compression. (Please read the Instructions section below before you start programming)

(a) (20 points) Implement the EM algorithm to estimate a mixture of k Gaussian distributions and run it on the image file “stadium.jpg”. Cluster the pixels into k = {4,8,12} clusters and plot the compressed images for each value of k as described below. (Note: your program might fail if Σ is singular; in this case, restart your EM again. We will fix the problem in part (d)).

(b) (10 points) Run your EM implementation on the “stadium.jpg” image for k = {4,8,12} and plot the expected complete log-likelihood function Q(Φ|Φl) after each E-step and M-step of the EM algorithm in one curve for each value of k. Use different colors to plot the log-likelihood after the E-step and M-step in the curve. Briefly explain the results.

(c) (10 points) Try to run your EM implementation on the image “goldy.jpg” with k = 7 and report your observation (Hint: If your algorithm falls here, don’t panic. Continue to the rest part.). Next, use the k-means function in cluster module of sklearn package to cluster the pixels with k = 7. Plot the compressed image given by kmeans. Explain why kmeans and EM behaved differently on the image.

(d) (20 points) Next, implement an improved version of EM to handle singular covariance matrix. In the log-likelihood function, we can add the following regularization term, , where (Σ−i 1)jj is the

(j,j)-th entry of matrix Σ−i 1 and λ &gt; 0. This regularization term encourages the diagonal of Σ−i 1 to be small such that Σi is not singular. After adding this regularization term, the expectation step is unchanged and in the maximization step, the maximum likelihood learning of µis and πis are also unchanged. Derive the maximum likelihood learning of Σis using the following result,

(hint: modify the derivation on slide 32 in parametric.pdf to solve the problem).

(e) (10 points). Implement the new model and test the new model on

“goldy.jpg”. Explain your observations.

Instructions

• Solutions to all questions must be presented in a report which includes results, explanations, all images and plots.

• All programming questions must be written in Python, no other programming languages will be accepted. And numpy, scipy, skimage, sklearn and matplotlib can be relied on to implement the algorithm (Note that you are only allowed to use KMeans function in cluster module of sklearn package in this homework). The code must be able to be executed from either terminal or PyCharm console on the cselabs machines. Each function must take the inputs in the order specified and print/display the required output to either terminal or PyCharm console. For each part, you can submit additional files/functions (as needed) which will be used by the main functions specified below. Put comments in your code so that one can follow the key parts and steps. Please follow the rules strictly. If we cannot run your code, you will receive no credit. • Question 2:

– hw3 Q2 a driver script which 1) uses kmeans to display a compressed image 2) runs your standard EM implementation finishing by outputting your own error message explaining why it fails 3) runs your improved EM implementation to display the compressed image. For loading the “goldy.jpg” image, you can use the following code:

from skimage import io img = io.imread(’./stadium.jpg’) img = img/255

– EMG(image.jpg: file path to an image, k: scalar value of the number of clusters, flag: a binary indicator variable). Function EMG implements the standard EM algorithm if flag is 0, while implements the improved EM algorithm if flag is 1. The function must print to either terminal or PyCharm console and return in variables the following for a single image and value of k: (1) h: a n × k matrix where n is the number of pixels, (2) m: a k × d matrix where d = 3 denotes the RGB values, and (3) Q: a column vector of expected complete log-likelihood values. The outputs {h,m,Q} are defined in Section 7.4 of the textbook. The function must also display: (1) a single compressed color image for a single value of k and (2) a single plot for the expected complete log-likelihood function value vs iteration number for a single value of k.

– You can use the imread() function in io module of skimage package to convert the image into a 3D matrix in Python. You will then need to convert the 3D matrix into a 2D matrix with d = 3 columns, in which each row are the three RGB values of a pixel. You can use the reshape() function in numpy package to do this .

– To decide the membership of each pixel xt, you can select argmaxhti.

i

– To visualize the compression, use the mean estimated from Ci as the color of pixels in Ci.

– In your EM implementation, you can use the function KMeans() in cluster module of sklearn package to find the initial clusters, however you can only run kmeans for at most 3 iterations.

– Your program must be efficient and finish running for a single image and value of k in at most a couple of minutes. You can set a maximum number of iterations for the EM algorithm however use no less than 100 iterations.

Submission

• Things to submit:

1. hw3 sol.pdf: A PDF document which contains the report with solutions to all questions.

2. EMG.py: Code for Question 2.

3. Any other files, except the data, which are necessary for your code.

• Submit: All materials must be zipped in one file, and submitted electronically via canvas.
