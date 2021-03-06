leleminer: get potential lele by analyzing single web page
==========================

leleminer is providing web services through RESTful API:

.. code-block:: shell

   curl -u hawkwang:1111111 -i http://localhost:5001/todo/api/v1.0/tasks

   curl -u hawkwang:1111111 -i http://localhost:5001/todo/api/v1.0/tasks/2

   curl -u hawkwang:1111111 -i -H "Content-Type: application/json" -X POST -d '{"title":"Read a book"}' http://localhost:5001/todo/api/v1.0/tasks

Package & Usage
-----------

Since *wxanalyzer* will be used in all the weixiao projects, so we just illustrate 
how to package and used in virtualenv.


Package
^^^^^

1. Prepare the requirements.txt and other stuff
2. Use ``python setup.py sdist`` to package module as follows:

dist

└── leleminer-0.1.0.tar.gz


Usage with virtualenv
^^^^^

1. ``cd leleminer``
2. ``virtualenv env``
3. Activate the virtual environment
   ``source env/bin/activate``
4. Install the required libraries
   4.1 install wxanalyzer package
   4.2 ``pip install -r requirements.txt``
5. Launch leleminer web service
   ``python leleminer.py``

