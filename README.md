# comp90038-assignment-1-solved
**TO GET THIS SOLUTION VISIT:** [COMP90038 Assignment 1 Solved](https://www.ankitcodinghub.com/product/comp90038-algorithms-and-complexity-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;120203&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;COMP90038 Assignment 1 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
This assignment is marked out of 30 and is worth 15% of your grade for COMP90038.

Objectives

To improve your understanding of the time complexity of algorithms and recurrence relations. To develop problem-solving and design skills. To improve written communication skills; in particular the ability to present algorithms clearly, precisely and unambiguously.

Problems

Let’s play a game. Or, more precisely, design and analyse some algorithms that might be used in a simple two-dimensional (2D) game.

Figure 1: A tiny example game scenario. Enemy (AI-controlled) players are shown in blue. The fixed location of the human player is marked by the red cross.

Consider a game played on an two-dimensional grid, whose Cartesian coordinates range from (−M,M)…(M,M). Figure 1 depicts a game board for which M = 4.

The game contains a fixed number N of enemy players, who are AI-controlled. Each player (including the human player and each enemy AI) is located at some arbitrary but fixed position (x,y) on the board,

i.e. for which −M ≤ x ≤ M and −M ≤ y ≤ M.

The human player can perform certain attacks, which damage all enemy players within a certain range of the human player. To avoid the need to calculate with expensive multiplication and square root operations, we will approximate the range by a square situated about the human player.

Specifically, given some fixed bound b, for which 0 ≤ b ≤ M, if the human player is located at position (px,py) then all enemy players that lie within or on the borders of the box whose bottom-left corner is (px − b,py − b) and whose top-right corner is (px + b,py + b) are affected by the attack. Figure 1 depicts an example box for the bound b = 1.5.

1. [1 mark] Implement an Θ(1) function to determine whether an enemy at position (x,y) is affected by the player’s attack, given the player’s location (px,py):

function IsAffected((px,py),(x,y),b)

…

The following function uses the divide and conquer approach to mark all enemy players affected by a player attack. Marking is implemented by the Mark function whose details are not important.

(Note: the division below is integer division, i.e. it rounds down to the nearest integer.) function MarkAffected((px,py),A,b)

MarkAffectedDC((px,py),A,0,N − 1,b)

function MarkAffectedDC((px,py),A,lo,hi,b) . assume lo ≤ hi if lo = hi then

if IsAffected((px,py),A[lo],b) then

Mark(A[lo]) else

mid ← lo + (hi − lo)/2

MarkAffectedDC((px,py),A,lo,mid,b)

MarkAffectedDC((px,py),A,mid + 1,hi,b)

Explain the purpose of the outermost “if/else” test. In particular, suppose we removed the line “if lo = hi” and the “else” line. In no more than a paragraph explain how this would affect the algorithm.

T(1)=1 T(1)=2 T(1)=0 T(1)=2 T(n)=2T(n/2) T(n)=2T(n/2) + 2 T(n)=2T(n/2) T(n)=2T(n/2)

Specifically, complete the following comparison function that would be used while sorting the array A. Here, (x1,y1) and (x2,y2) are two points from the array A. The function should return true if it considers the first point to be less than or equal to the second, and should return false otherwise. Your function can use the player’s coordinate (px,py) as global variables, i.e. you are allowed to refer to px and py in your function.

function LessOrEqualTo((x1,y1),(x2,y2))

…

Let d be the expected number of enemy AIs contained in or on the borders of a box of bound b (i.e. whose width and height are each 2b) on the board. For simplicity, we limit our attention to boxes that are contained entirely within the game baord.

Consider an algorithm that, given an array A sorted according to your comparison function, implemented the behaviour of MarkAffected above by first using your Θ(log(N)) function to determine the elements that need to be marked (of which we expect there to be d), and then marking those d elements. We might characterise its expected complexity as:

log(N) + d

Derive a formula for d in terms of b, M and N.

Implement a function that determines whether two enemy AIs can directly communicate. Include a brief description (no more than a single paragraph) of how your function works, i.e. the rationale behind its design.

function CanDirectlyCommunicate((x1,y1),(x2,y2),(px,py),b)

…

Here the nodes ni are simply the indices of enemy AIs in the array A, so each of them is simply an integer in the range 0 ≤ ni ≤ N −1. Therefore the adjacency matrix M is simply a two-dimensional array, M[0][0]…M[N − 1][N − 1].

Implement an O(N2) algorithm that, given two enemy AIs n1 and n2 determines whether there exists a path by which they might communicate via other enemy AIs. If a path exists, your algorithm should return the shortest path by which communication is possible. Otherwise, your algorithm should return the empty path. Your algorithm also takes as its input the adjacency matrix representation of the graph described above.

You should represent a path as a linked list of enemy AI indices ni. The empty path is therefore the empty linked list without any nodes.

Submission and Evaluation

• You must submit a PDF document via the LMS. Note: handwritten, scanned images, and/or Microsoft Word submissions are not acceptable — if you use Word, create a PDF version for submission.

• We expect your work to be neat – parts of your submission that are difficult to read or decipher will be deemed incorrect. Make sure that you have enough time towards the end of the assignment to present your solutions carefully. Time you put in early will usually turn out to be more productive than a last-minute effort.

Please see https://academicintegrity.unimelb.edu.au
