.. _coding_procedure:






################
Database Schema
################

.. topic:: Overview

    This section documents the schema of the DB.  You will find the `Reference Tables`_ and the variable level documentation within.  


    :Date: |today|
    :Author: **Justin Napolitano**


.. contents:: 
    :depth: 3


Reference Tables
################
.. topic:: Overview

    This section contains reference tables for variables coded numerically in the Turkish-Kurdish Conflict Event Database


    :Date: |today|
    :Author: **Justin Napolitano**

.. contents:: :local:
    :depth: 3

Analysis Coding View
====================

.. csv-table:: Analysis Coding View
   :file: /csv/schema_overview.csv
   :widths: 20, 70, 20
   :header-rows: 1


Aggressor Table
===============

.. csv-table:: Aggressor Table
   :file: /csv/side_a_table.csv
   :widths: 20, 20
   :header-rows: 1

Victim Table
============

.. csv-table:: Victim Table
   :file: /csv/side_b_table.csv
   :widths: 20, 20
   :header-rows: 1

Human Rights Category Table
===========================

.. csv-table:: Human Rights Category Table
   :file: /csv/human_rights_category_table.csv
   :widths: 20, 20
   :header-rows: 1

Human Rights Offense Table
===========================

.. csv-table:: Human Rights Offense Table
   :file: /csv/human_rights_offense_table.csv
   :widths: 1, 10, 1, 1, 10, 15
   :header-rows: 1   

Region Table
============

.. csv-table:: Region Table
   :file: /csv/region_code_table.csv
   :widths: 20, 20
   :header-rows: 1

Province Table
==============

.. csv-table:: Province Table
   :file: /csv/province_code_table.csv
   :widths: 20, 20
   :header-rows: 1


Definitions
################

.. topic:: Overview

    This section contains the definitions and descriptions for every variable recorded in the data set. 


    :Date: |today|
    :Author: **Justin Napolitano**

.. contents:: :local:
    :depth: 3


Year
====
    
Definition
----------

Records the Year the event occurs.

Aggressor_ID
============

Definition 
----------

Records the ID of the aggressor of an event; the agent or group that commits a human right violation.

Table
-----

`Aggressor Table`_ for reference.

Aggressor_Name
==============
    
Definition 
----------

Records the name of the aggressor of an event; the agent or group that commits a human right violation.

Table
-----

`Aggressor Table`_ for reference.

Victim_ID
=========
    
Definition   
----------

Records the ID of the victim of an event; the agent or group that is victim to a human right violation commited by the aggressor.

Table
-----

`Victim Table`_ for reference.

Victim_Name
===========

Definition  
----------

Records the name of the victim of an event; the agent or group that is victim to a human right violation commited by the aggressor.

Table
-----

`Victim Table`_ for reference.


Source_Article
==============

Definition 
----------

A record of the name, data, and title of the source from which information on an event is gathered.


Source_Date
===========

Definition
----------

The date the source material containing the information of an event record.


Source_Headline
===============

Definition
----------

The title of the source material containing the information of an event record. 


Region_Name
===========

Defintion
---------

The name of the administrative region an event was recorded.  Regions are defined according the offical provincial and administrative regions of the Turkish State.

Table
-----

`Region Table`_


Region_Code
===========

The code of the administrative region an event was recorded.  Regions are defined according the offical provincial and administrative regions of the Turkish State.

Table
-----

`Region Table`_

Kurdish_Region
==============

Definition
----------

A boolean variable that indicates whether a region is predominantly Kurdish by population.

Type
----

Boolean


Province_Name
=============

Definition
----------

The name of the provincial level administrative region an event was recorded.  Provinces are defined according the offical provincial and administrative regions of the Turkish State.

Type
----

String

Reference Table
---------------

`Province Table`_


Province Code
=============

The code of the provincial level administrative region an event was recorded.  Provinces are defined according the offical provincial and administrative regions of the Turkish State.

Type
----

Categorical Integer

Reference Table
---------------

`Province Table`_


Country
=======

Definition
----------

The state (country) where an event is recorded.

Data Type
---------

Integer

Date_Start
==========

Definition
----------
testing....
::

    A record of the day, month, and year in the DD/MM/YYYY format of when the event takes place.

    If the exact datastamp cannot be determined the best possible date is estimated.

Data Type
---------
testing..
::

    DateStamp DD/MM/YYYY.







