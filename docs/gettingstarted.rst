Getting started with the OMERO Python API
=========================================

**Description**
---------------

We will use a Python script showing how to analyze data stored in an OMERO server.

We will show:

- How to connect to server.

- How load images from a dataset.

- Run a simple FRAP analysis measuring the intensity within a pre-existing ellipse ROI in a named Channel.

- How to save the generated mean intensities and link them to the image(s).

**Setup**
---------

We recommend to use a Conda environment to install the OMERO Python bindings. Please read first :doc:`setup`.


**Step-by-Step**
----------------

In this section, we go through the steps required to analyze the data.
The script used in this document is :download:`simple_frap.py <../scripts/simple_frap.py>`.

Connect to the server:

.. literalinclude:: ../scripts/simple_frap.py
    :start-after: # Connect
    :end-before: # Load-images


Load the dataset:

.. literalinclude:: ../scripts/simple_frap.py
    :start-after: # Load-images
    :end-before: # Analyze-images


We are now ready to analyze the images in the dataset:

.. literalinclude:: ../scripts/simple_frap.py
    :start-after: # Analyze-images
    :end-before: # Get channel

Save the results as map annotation:

.. literalinclude:: ../scripts/simple_frap.py
    :start-after: # Save-results
    :end-before: # Delete-old-annotations

When done, close the session:

.. literalinclude:: ../scripts/simple_frap.py
    :start-after: # Disconnect
    :end-before: # main


**Exercises**
-------------
