# mcmc
Markov creating music chain

To do:
1.  Modify code to accept multiple different songs as input (assuming 2 track song, LHS and RHS)
    Workflow:
      1. Transpose the song to a base key signature
      2. Find transition matrix of each track in song
      3. Repeat for N songs, until you have N right hand and left hand track transition matrices
      4. Add each of the N LHS/RHS transition matrices together
      5. Normalize
      6. Remove 0 rows
      7. Now, you have the FINAL TRANSITION MATRIX FOR THIS SET OF SONGS (LHS AND RHS).
      8. Find stationary distribution (this will be our initial distribution of starting notes)

2.  Figure out how to add rests/timing into the mix (a 2nd, underlying markov chain? CTMC?)

3.  Fixing 'harmony' to be more dependent/related to 'melody':
      - DONE - MADE LH SOMEWHAT DEPENDENT ON RH. SOUNDS ALRIGHT.
      
