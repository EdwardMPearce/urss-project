## urss-project
Implementation of sporadic finite subgroups of SL(3,C) in _Magma_\
You can try running the code using the [_Magma_ calculator](http://magma.maths.usyd.edu.au/calc/) \
This code for Magma allows the user to construct and experiment with\
the finite subgroups E,F,G,H,I,J,K,L of SL(3,C)\
which are described in the classification given by S.Yau and Y.Yu\
in [Gorenstein Quotient Singularities in Dimension Three, 1993](https://bookstore.ams.org/memo-105-505/),\
and compute the adjacency matrix for the McKay quiver of a finite group.\
It is hoped that the user may find this useful in case they wish to further study these particular groups,\
or simply as an elementary introduction to the Magma computer algebra system.

This repository includes:
- A [file][1] containing three functions which construct the groups in question.
- A [file][2] containing sample code for experimenting with finite groups in Magma.\
  In particular, once constructed, the adjacency matrix for the McKay quiver of a group 
  (with respect to a given representation) can be computed from character table data.
- A [file][3] containing the source code from the above two all in one file
  for the purpose of improving/impeding the ease of reading and use
- [Character table outputs][4] from running the code in the Magma calculator
- A licence
- This README file

[1]: https://github.com/EdwardMPearce/urss-project/blob/master/constructorfuncs.txt
[2]: https://github.com/EdwardMPearce/urss-project/blob/master/McKay_quiver_script.txt
[3]: https://github.com/EdwardMPearce/urss-project/blob/master/all_in_one.txt
[4]: https://github.com/EdwardMPearce/urss-project/blob/master/Character%20Tables.txt

# TODO:
1. Write the McKay quiver adjacency matrix code as a function
2. Using an `if __name__ == "__main__":` type structure\ 
would eliminate the need to separate the functionality (definitions) from\
demonstrative/unit test code into two separate files.\
[Understand the main method of Python](https://stackoverflow.com/questions/22492162/understanding-the-main-method-of-python/22493194#22493194)
3. Write a script to access the Magma calculator remotely, so that the output\
can be read as text for further use (e.g. export the adjacency matrix, draw the McKay quiver)\
Idea was to use Python requests, but encountered 401 Unauthorized error, so need to learn about accessing servers?
4. Learn/remember how to write nice [Markdown](https://en.support.wordpress.com/markdown-quick-reference/)

# Acknowledgements
Thanks to Prof. Miles Reid at the University of Warwick for supervising me on this\
Undergraduate Research Support Scheme (URSS) in the summer of 2015,\
and thanks to the University of Warwick for providing the URSS bursary\
of £1000 to support this research.
