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

Definition
----------
  
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

Definition
----------
    
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

    Integer.

Date_Start
==========

Definition
----------

    A record of the day, month, and year in the DD/MM/YYYY format of when an event takes starts.

    If the exact datastamp cannot be determined the best possible date is estimated.

Data Type
---------

    DateStamp DD/MM/YYYY.


Date_End
========

Definition
----------

    A record of the day, month, and yearn in the DD/MM/YYYY format of when an event ends.

Data Type
---------

    DateStamp DD/MM/YYYY


Women_Killed
=============

Definition
----------

    The best estimate of deaths of women recorded for an event.

Data Type
---------

    Integer


Children_Killed
===============

Definition
----------

    The best estimate of the number of deaths of children recorded for an event.

Data Type
---------

    Integer


Total_Killed
===============

Definition
----------

    The sum of Women_Killed, Children_Killed, and any other deaths recorded for an event. 

Data Type
---------

    Integer

Women_Raped
===============

Definition
----------

    The recorded number of women during an event.  

Data Type
---------

    Integer

Illegal_Imprisonments
=====================

Definition
----------

    The recorded number of people illegally imprisoned during an event.  

Data Type
---------

    Integer

Illegal_Detentions
==================

Definition
----------

    The recorded number of people illegally detained by any non-governmental agent or organization during an event.  

Data Type
---------

    Integer


Illegal_Imprisonments
=====================

Definition
----------


    The recorded number of people illegally imprisoned by the Turkish State during an event.  

Data Type
---------

    Integer


Human_Rights_Category_Code
==========================

Definition
----------

    The code of the category of Human Rights violation as defined by Justin Napolitano and Demet Mousseau. Insert a reference here.

Data Type
---------

    Categorical Integer.


Reference Table
---------------

    `Human Rights Category Table`_



Human_Rights_Category_Name
==========================

Definition
----------

    The name of the category of Human Rights violation as defined by Justin Napolitano and Demet Mousseau. Insert a reference here.

Data Type
---------

    String


Reference Table
---------------

    `Human Rights Category Table`_



Human_Rights_Offense_Code
==========================

Definition
----------


    The code of the offence to Human Rights as defined by the United Nations or Comparable International Treaty Organization.


Data Type
---------

    Categorical Integer.


Reference Table
---------------

    `Human Rights Offense Table`_



Human_Rights_Offense_Name
==========================

Definition
----------

    The name of the offence to Human Rights as defined by the United Nations or Comparable International Treaty Organization.

Data Type
---------


    String


Reference Table
---------------

    `Human Rights Offense Table`_


Is_Women_Event
==============

Definition
----------

    A boolean variable that designates if an event primarily affects males or females.

    0 designates an event as affecting males.

    1 designates an event as affecting women.

Data Type
---------

    Boolean

Is_Children_Event
=================

Definition
----------


    A boolean variable that designates if an event primarily affects adults or children.  
    
    0 designates an event as affecting adults. 
    
    1 designates an event as affecting children.

Data Type
---------

  ::

    Boolean


Description
===========

Definition
----------


    A description of an event that may contain information that could not be relayed in the coding. 


Data Type
---------

    String


ID
===

Definition
----------

    A unique identifier for a coded event


    It is constructed by appending the values of: 
        #. year
        #. Aggressor_ID
        #. Victim_ID
        #. Human_Rights_Category_Code 
        #. Human_Rights_Offense_Code


    For instance, id 19981265 is an event that occurred in 1998 committed by the Turkish government against women.  It is a broad violation of Collective Developmental rights.  Specifically, the right to freedom of peaceful assembly and association



Data Type
---------

    String

