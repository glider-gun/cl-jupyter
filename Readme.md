cl-Jupyter
==========

An enhanced interactive Shell for Common Lisp (based on the Jupyter protocol)

```
 cl-jupyter: an enhanced interactive Common Lisp Shell
(Version 0.5 - Ipython protocol v.4.1)
--> (C) 2014-2015 Frederic Peschanski (cf. LICENSE)
                                 __________       
                                /         /.      
     .-----------------.       /_________/ |      
    /                 / |      |         | |      
   /+================+\ |      | |====|  | |      
   ||cl-Jupyter      || |      |         | |      
   ||                || |      | |====|  | |      
   ||* (fact 5)      || |      |         | |      
   ||120             || |      |   ___   | |      
   ||                || |      |  |166|  | |      
   ||                ||/@@@    |   ---   | |      
   \+================+/    @   |_________|./.     
                         @           ..  ....'    
     ..................@      __.'. '  ''         
    /oooooooooooooooo//      ///                  
   /................//      /_/                   
   ------------------                          
```

**Important** : this is alpha version non-officially released software. **Use it at your own risk and peril !**

## Requirements ##

To try cl-Jupyter you need :

 - a Common lisp implementation, for now

   - either SBCL 1.2.x or above (with native threads enabled)

   - or Clozure CL 1.10 or aboce (with native threads enabled) ...

   - ECL is planned, for other implementations please fill an issue.

 - Quicklisp (cf. http://www.quicklisp.org/)

 - Python 3.2 or above

 - IPython 2.1 or above

## Quick launch ##

For simple interactions on the console, just type:

    python3 ./cl-jupyter.py     (or directly ./cl-jupyter.py if python3 is in PATH)

```
In [1]: (* 2 21)
Out[1]: 42

In [2]: 
```

By default, cl-Jupyter assumes SBCL as the default lisp implementation. Using CCL instead requires
the following command line:

    python3 ./cl-jupyter.py  --lisp=ccl


**Note**: cl-Jupyter seems to work better with CCL on MacOS  (but on Linux everything's fine with SBCL).

## Notebooks ##

The real interest of cl-Jupyter is its use conjointly
 with the Jupyter notebook frontend. For a try, type:

    python3 ./cl-jupyter.py notebook

(for SBCL)

or

    python3 ./cl-jupyter.py notebook  --lisp=ccl

(for CCL)

The file `AboutCLJupyter.ipynb` is an example of a Lisp-based notebook.

The file `AboutCLJupyter.pdf` is a printable PDF version of this notebook that can be generated by the Jupyter `nbconvert` tool.

----

 ... have fun !

