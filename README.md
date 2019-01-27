# print-for-binding

LaTeX file to produce pdf of thesis, suitable for traditional binding. Change `path/to/pdf` on line 7.  

(Note that, if you're getting the Uni to print and bind the thesis for you, this is not necessary and you can just give them a normal pdf- my Uni does 'perfect binding' of the thesis).  

Currently uses 8-page signatures (ie 8 pages per booklet thing). 

Will insert 2 blank pages for attaching binding to cover at the front. 

It does **not** insert pages at the back, so check this manually before printing! If necessary, change the `\incudepdf` command to `\includepdf[pages={{}, {}, 1-last, {}, {}},nup=1x2,landscape,signature=8]{path/to/pdf}` (you may only need one `{}`). 

