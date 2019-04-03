Predicting average reading time based on text data
==================================================

This is an introduction to machine learning on text data.
`The accompanying article <https://www.twipemobile.com/research-findings-using-ai-on-text/>`_
explains the different steps in preprocessing text so it becomes machine readible. Further,
the preprocessed text is used to train a
`Support Vector Machine <https://towardsdatascience.com/support-vector-machine-introduction-to-machine-learning-algorithms-934a444fca47>`_.
Thereafter, the trained model is tested and investigated. The research investigates what
the model learns and tries to visualize which words lead to higher or lower average reading
time for an article.

Example output:

.. image:: ../resources/high_reading_time_words.png
   :align: center

Installation
------------

This projects is tested on python 3.6 on a linux machine.
For the following script virtualenv is required (execute in project folder):

.. code-block:: bash

    virtualenv -p python3.6 avg_reading_time_pred_env
    source avg_reading_time_pred_env/bin/activate
    pip install -r requirements.txt
    ipython kernel install --user --name=avg_reading_time_pred_env

Use the ``avg_reading_time_pred_env`` kernel in your ipython notebook to run.

You will also need the following files:

* a csv file with your article text data ``article_content.csv`` in the data folder
* a csv file referencing the article text data, with reading time for every article
  ``article_reading_time.csv`` in the data folder

Instruction on the layout of these files are provided in the notebook. The original data
Could not be included, as this is proprietary data.


Support
-------

If you are having issues, please let us know at engineering@twipemobile.com or create
a git issue in this repository.
New ideas for research or also welcome.
