# PageRank

## Description
Using MapReduce to handle multiplication of very large matrices and optimize computation.

- Used <b>adjacency matrix</b> to construct/describe relations between any two of all web pages, which is called <b>Transition Matrix</b>. 
- Then based on iterative computations, we use the <b>Transition Matrix</b> to compute the <b>PageRank</b> of each web page util the <b>PageRank Matrix</b> converged. NOTE: we use <b>BETA</b> to handle two edge cases - <b>Dead Ends</b> and <b>Spider Traps</b>.

## Data Information
The test data of this repo which is put in the folder `dataset` comes from [here](https://www.limfinity.com/ir/).<br/>.
- `transition.txt` each line describes one web page can link to a list of web pages.<br/>For example, one line "1 \t 2,3,4,5" means a web page whose ID is 1 can link to four web pages whose IDs are 2, 3, 4 and 5 respectly.
- `pr.txt` describes initial PageRank values of all web pages.<br/>For example, one line "57 \t 1" means the initial PageRank value of a web page whose ID is 57 is 1.<br/>Besides, PageRank values of all web pages are uniformly intialized to 1.
